# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: questionnaireCreation.spec.ts >> Questionnaire Creation Tests >> TC_CR_001-Verify 'Add' button is disabled in questionnaire creation when required fields  are empty
- Location: tests/questionnaireCreation.spec.ts:42:9

# Error details

```
Error: browserType.launch: Executable doesn't exist at /home/runner/.cache/ms-playwright/chromium_headless_shell-1223/chrome-headless-shell-linux64/chrome-headless-shell
╔════════════════════════════════════════════════════════════╗
║ Looks like Playwright was just installed or updated.       ║
║ Please run the following command to download new browsers: ║
║                                                            ║
║     npx playwright install                                 ║
║                                                            ║
║ <3 Playwright Team                                         ║
╚════════════════════════════════════════════════════════════╝
```

```
TypeError: Cannot read properties of undefined (reading 'close')
```

# Test source

```ts
  1   | import { test, expect, Page } from '@playwright/test';
  2   | import { LoginPage } from '../src/pages/login.page';
  3   | import { LeftNavigation } from '../src/pages/leftNavigations.page';
  4   | import { KnowledgeDataBasePage } from '../src/pages/knowledgeDataBase.page';
  5   | import { QuestionnairePage } from '../src/pages/knowledgeDatabase/questionnaire.page';
  6   | import data from '../fixtures/questionnaireCreation.json';
  7   | 
  8   | test.describe('Questionnaire Creation Tests', () => {
  9   | 
  10  |     let page: Page;
  11  |     let leftNav: LeftNavigation;
  12  |     let kdPage: KnowledgeDataBasePage;
  13  |     let questionnairePage: QuestionnairePage;
  14  |     let username: string;
  15  |     let timeSuffix: number;
  16  | 
  17  |     test.beforeAll(async ({ browser }) => {
  18  |         page = await browser.newPage();
  19  |         const loginPage = new LoginPage(page);
  20  |         await loginPage.goto();
  21  |         await loginPage.signInWith();
  22  | 
  23  |         leftNav = new LeftNavigation(page);
  24  |         kdPage = new KnowledgeDataBasePage(page);
  25  |         questionnairePage = new QuestionnairePage(page);
  26  |         const envUsername = process.env.USER_NAME!;
  27  |         username = envUsername.split(' ')[0];
  28  |         timeSuffix = Date.now();
  29  | 
  30  |         // Navigate to questionnaire configuration
  31  |         await leftNav.clickOnKnowledgeDatabase();
  32  |         await kdPage.clickOnCompanyName('QA Automation');
  33  |         await leftNav.clickOnMaintain();
  34  |         await leftNav.clickOnQuestionnairesAndForms();
  35  |         await kdPage.clickOnNoThanksPopup();
  36  |     });
  37  | 
  38  |     test.afterAll(async () => {
> 39  |         await page.close();
      |                    ^ TypeError: Cannot read properties of undefined (reading 'close')
  40  |     });
  41  | 
  42  |     test("TC_CR_001-Verify 'Add' button is disabled in questionnaire creation when required fields  are empty", async () => {
  43  |         await questionnairePage.clickOnAddNewQuestionnaire();
  44  |         await expect(questionnairePage.addBtn).toBeDisabled();
  45  |         await questionnairePage.closeDialog();
  46  |     });
  47  | 
  48  |     test("TC_CR_002-Verify 'This field is required!' validation message appears in questionnaire creation when fields are cleared after entry", async () => {
  49  |         await questionnairePage.clickOnAddNewQuestionnaire();
  50  |         await questionnairePage.fillQuestionnaireName(data.questionnaire.name);
  51  |         await questionnairePage.fillQuestionnaireName("");
  52  |         await questionnairePage.verifyRequiredFieldError('Questionnaire name')
  53  |         await questionnairePage.fillQuestionnaireCode(data.questionnaire.code);
  54  |         await questionnairePage.fillQuestionnaireCode("");
  55  |         await questionnairePage.verifyRequiredFieldError('Questionnaire code')
  56  |         await questionnairePage.openQuestionnaireTypeDropdown();
  57  |         await questionnairePage.clickOnNewTab();
  58  |         await questionnairePage.verifyRequiredFieldError('Questionnaire type')
  59  |         await questionnairePage.closeDialog();
  60  |     });
  61  | 
  62  |     test('TC_CR_003-Verify Questionnaire type dropdown contains all four types', async () => {
  63  |         await questionnairePage.clickOnAddNewQuestionnaire();
  64  |         await questionnairePage.openQuestionnaireTypeDropdown();
  65  |         await questionnairePage.verifyDropdownOptionVisible(data.questionnaire.type);
  66  |         await questionnairePage.verifyDropdownOptionVisible(data.form.type);
  67  |         await questionnairePage.verifyDropdownOptionVisible(data.survey.type);
  68  |         await questionnairePage.verifyDropdownOptionVisible(data.audit.type);
  69  |         await questionnairePage.closeDialog();
  70  |     });
  71  |     
  72  | 
  73  |     test("TC_CR_004-Verify successful creation of a new questionnaire with type set to 'Questionnaire'", async () => {
  74  |         const uniqueName = `${data.questionnaire.name}_${timeSuffix}`;
  75  |         data.questionnaire.name = uniqueName;
  76  |         data.questionnaire.search.name = uniqueName;
  77  |         data.questionnaire.search.owner = username;
  78  |         await questionnairePage.clickOnAddNewQuestionnaire();
  79  |         await questionnairePage.createNewQuestionnaireWithData(data.questionnaire);
  80  |         await leftNav.clickOnQuestionnairesAndForms();
  81  |         await questionnairePage.searchQuestionnaire(data.questionnaire.name);
  82  |         await questionnairePage.verifySearchResult(data.questionnaire.search);
  83  |     });
  84  | 
  85  |     test("TC_CR_005-Verify successful creation of a new questionnaire with type set to 'Form'", async () => {
  86  |         const uniqueName = `${data.form.name}_${timeSuffix}`;
  87  |         data.form.name = uniqueName;
  88  |         data.form.search.name = uniqueName;
  89  |         data.form.search.owner = username;
  90  |         await questionnairePage.clickOnAddNewQuestionnaire();
  91  |         await questionnairePage.createNewQuestionnaireWithData(data.form);
  92  |         await leftNav.clickOnQuestionnairesAndForms();
  93  |         await questionnairePage.searchQuestionnaire(data.form.name);
  94  |         await questionnairePage.verifySearchResult(data.form.search);
  95  |     });
  96  | 
  97  |     test("TC_CR_006-Verify successful creation of a new questionnaire with type set to 'Survey'", async () => {
  98  |         const uniqueName = `${data.survey.name}_${timeSuffix}`;
  99  |         data.survey.name = uniqueName;
  100 |         data.survey.search.name = uniqueName;
  101 |         data.survey.search.owner = username;
  102 |         await questionnairePage.clickOnAddNewQuestionnaire();
  103 |         await questionnairePage.createNewQuestionnaireWithData(data.survey);
  104 |         await leftNav.clickOnQuestionnairesAndForms();
  105 |         await questionnairePage.searchQuestionnaire(data.survey.name);
  106 |         await questionnairePage.verifySearchResult(data.survey.search);
  107 |     });
  108 | 
  109 |     test.skip("TC_CR_007-Verify successful creation of a new questionnaire with type set to 'Audit'", async () => {
  110 |         const uniqueName = `${data.audit.name}_${timeSuffix}`;
  111 |         data.audit.name = uniqueName;
  112 |         data.audit.search.name = uniqueName;
  113 |         data.audit.search.owner = username;
  114 |         await questionnairePage.clickOnAddNewQuestionnaire();
  115 |         await questionnairePage.createNewQuestionnaireWithData(data.audit);
  116 |         await leftNav.clickOnQuestionnairesAndForms();
  117 |         await questionnairePage.searchQuestionnaire(data.audit.name);
  118 |         await questionnairePage.verifySearchResult(data.audit.search);
  119 |     });
  120 | });
```