# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: questionnaireUiActions.spec.ts >> Questionnaire UI Action Tests >> TC_QNA_001-Verify copy action works in questionnaire
- Location: tests/questionnaireUiActions.spec.ts:55:9

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
  1  | import { test, expect, Page, } from '@playwright/test';
  2  | import { LoginPage } from '../src/pages/login.page';
  3  | import { LeftNavigation } from '../src/pages/leftNavigations.page';
  4  | import { KnowledgeDataBasePage } from '../src/pages/knowledgeDataBase.page';
  5  | import { QuestionnairePage } from '../src/pages/knowledgeDatabase/questionnaire.page';
  6  | import { QuestionnaireEditPage } from '../src/pages/knowledgeDatabase/questionnaireForms/questionnaireEdit.page';
  7  | 
  8  | test.describe('Questionnaire UI Action Tests', () => {
  9  | 
  10 |     let page: Page;
  11 |     let leftNav: LeftNavigation;
  12 |     let kdPage: KnowledgeDataBasePage;
  13 |     let questionnairePage: QuestionnairePage;
  14 |     let editPage: QuestionnaireEditPage;
  15 |     let timeSuffix: number;
  16 |     let questionnaireCreationData = {
  17 |         "name": "Questionnaire",
  18 |         "code": "Q1",
  19 |         "type": "Questionnaire"
  20 |     }
  21 | 
  22 |     test.beforeAll(async ({ browser }) => {
  23 |         page = await browser.newPage();
  24 |         const loginPage = new LoginPage(page);
  25 |         await loginPage.goto();
  26 |         await loginPage.signInWith();
  27 | 
  28 |         leftNav = new LeftNavigation(page);
  29 |         kdPage = new KnowledgeDataBasePage(page);
  30 |         questionnairePage = new QuestionnairePage(page);
  31 |         editPage = new QuestionnaireEditPage(page);
  32 |         timeSuffix = Date.now();
  33 | 
  34 | 
  35 |         // Navigate to questionnaire configuration
  36 |         await leftNav.clickOnKnowledgeDatabase();
  37 |         await kdPage.clickOnCompanyName('QA Automation');
  38 |         await leftNav.clickOnMaintain();
  39 |         await leftNav.clickOnQuestionnairesAndForms();
  40 |         await kdPage.clickOnNoThanksPopup();
  41 | 
  42 |         // Create a Questionnaire
  43 |         const uniqueName = `${questionnaireCreationData.name}_${timeSuffix}`;
  44 |         questionnaireCreationData.name = uniqueName;
  45 |         await questionnairePage.clickOnAddNewQuestionnaire();
  46 |         await questionnairePage.createNewQuestionnaireWithData(questionnaireCreationData);
  47 |         await page.waitForTimeout(1000);
  48 |         await editPage.clickOnBeamer();
  49 |     });
  50 | 
  51 |     test.afterAll(async () => {
> 52 |         await page.close();
     |                    ^ TypeError: Cannot read properties of undefined (reading 'close')
  53 |     });
  54 | 
  55 |     test('TC_QNA_001-Verify copy action works in questionnaire', async () => {
  56 |         await editPage.clickCopyQuestionnaire();
  57 |         await expect(page.getByText('Copy -')).toBeVisible();
  58 |     });
  59 | 
  60 |     test('TC_QNA_002-Verify Publish action works in questionnaire', async () => {
  61 |         await editPage.clickOnPublishOrEdit();
  62 |         await editPage.verifyQuestionnaireIsPublished();
  63 |     });
  64 | 
  65 |     test('TC_QNA_003-Verify edit action works in questionnaire', async () => {
  66 |         await editPage.clickEditButton();
  67 |         await expect(editPage.publishOrEditButton.filter({ hasText: 'Publish' })).toBeVisible();
  68 |     });
  69 | });
```