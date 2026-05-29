# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: questionnaireCondition.spec.ts >> Questionnaire Condition Tests >> TC_QNC_001-Verify a new condition tab can be created with name and description in questionnaire conditions
- Location: tests/questionnaireCondition.spec.ts:77:9

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
  1   | import { test, expect, Page, } from '@playwright/test';
  2   | import { LoginPage } from '../src/pages/login.page';
  3   | import { LeftNavigation } from '../src/pages/leftNavigations.page';
  4   | import { KnowledgeDataBasePage } from '../src/pages/knowledgeDataBase.page';
  5   | import { QuestionnairePage } from '../src/pages/knowledgeDatabase/questionnaire.page';
  6   | import { QuestionsPage } from '../src/pages/knowledgeDatabase/questionnaireForms/configuration/questions.page';
  7   | import { QuestionnaireEditPage } from '../src/pages/knowledgeDatabase/questionnaireForms/questionnaireEdit.page';
  8   | import { QuestionnaireConditionsPage } from '../src/pages/knowledgeDatabase/questionnaireForms/configuration/questionnaireConditions.page';
  9   | import questionnaireConditionsData from '../fixtures/questionnaireCondition.json';
  10  | 
  11  | test.describe('Questionnaire Condition Tests', () => {
  12  | 
  13  |     let page: Page;
  14  |     let leftNav: LeftNavigation;
  15  |     let kdPage: KnowledgeDataBasePage;
  16  |     let questionnairePage: QuestionnairePage;
  17  |     let questionsPage: QuestionsPage;
  18  |     let editPage: QuestionnaireEditPage;
  19  |     let questionnaireConditionsPage: QuestionnaireConditionsPage;
  20  |     let timeSuffix: number;
  21  |     const questionnaireCreation = questionnaireConditionsData.questionnaire;
  22  |     const questions = questionnaireConditionsData.questions;
  23  |     const tabs = questionnaireConditionsData.tabs;
  24  |     const conditions = questionnaireConditionsData.conditions;
  25  |     const actionType = questionnaireConditionsData.actionType;
  26  |     const conditionOn = questionnaireConditionsData.conditionOn;
  27  | 
  28  |     test.beforeAll(async ({ browser }) => {
  29  |         page = await browser.newPage();
  30  |         const loginPage = new LoginPage(page);
  31  |         await loginPage.goto();
  32  |         await loginPage.signInWith();
  33  | 
  34  |         leftNav = new LeftNavigation(page);
  35  |         kdPage = new KnowledgeDataBasePage(page);
  36  |         questionnairePage = new QuestionnairePage(page);
  37  |         questionsPage = new QuestionsPage(page);
  38  |         editPage = new QuestionnaireEditPage(page);
  39  |         questionnaireConditionsPage = new QuestionnaireConditionsPage(page);
  40  |         timeSuffix = Date.now();
  41  | 
  42  | 
  43  |         // Navigate to questionnaire configuration
  44  |         await leftNav.clickOnKnowledgeDatabase();
  45  |         await kdPage.clickOnCompanyName('QA Automation');
  46  |         await leftNav.clickOnMaintain();
  47  |         await leftNav.clickOnQuestionnairesAndForms();
  48  |         await kdPage.clickOnNoThanksPopup();
  49  | 
  50  |         // Create a Questionnaire
  51  |         const uniqueName = `${questionnaireCreation.name}_${timeSuffix}`;
  52  |         questionnaireCreation.name = uniqueName;
  53  |         await questionnairePage.clickOnAddNewQuestionnaire();
  54  |         await questionnairePage.createNewQuestionnaireWithData(questionnaireCreation);
  55  | 
  56  |         //Create questions
  57  |         await editPage.clickOnQuestionnaireTab();
  58  |         await questionsPage.configureQuestion(questions.Text);
  59  |         await questionsPage.configureQuestion(questions.Email);
  60  |         await questionsPage.configureQuestion(questions.User);
  61  |         await questionsPage.configureQuestion(questions.Stars);
  62  | 
  63  |         // Navigate to questionnaire conditions
  64  |         await editPage.clickOnQuestionnaireConditionsTab();
  65  |         await questionnaireConditionsPage.clickAddTab();
  66  |         await questionnaireConditionsPage.fillTabDetails("default tab", "This is a default tab");
  67  |         await questionnaireConditionsPage.saveTab();
  68  |         await questionnaireConditionsPage.clickAddConditionTab();
  69  |         await questionnaireConditionsPage.enterConditionName("default");
  70  |         await questionnaireConditionsPage.submitCondition();
  71  |     });
  72  | 
  73  |     test.afterAll(async () => {
> 74  |         await page.close();
      |                    ^ TypeError: Cannot read properties of undefined (reading 'close')
  75  |     });
  76  | 
  77  |     test('TC_QNC_001-Verify a new condition tab can be created with name and description in questionnaire conditions', async () => {
  78  |         await questionnaireConditionsPage.createNewConditionTabWithData(tabs.tab1);
  79  |         await questionnaireConditionsPage.verifyTabCreated(tabs.tab1.tabName);
  80  |         await questionnaireConditionsPage.verifyActiveTab(tabs.tab1.tabName);
  81  |     });
  82  | 
  83  |     test('TC_QNC_002-Verify multiple condition tabs can be created and all visible in questionnaire conditions', async () => {
  84  |         await questionnaireConditionsPage.createNewConditionTabWithData(tabs.tab2);
  85  |         await questionnaireConditionsPage.verifyTabCreated(tabs.tab2.tabName);
  86  |         await questionnaireConditionsPage.verifyActiveTab(tabs.tab2.tabName);
  87  |         await questionnaireConditionsPage.createNewConditionTabWithData(tabs.tab3);
  88  |         await questionnaireConditionsPage.verifyTabCreated(tabs.tab3.tabName);
  89  |         await questionnaireConditionsPage.verifyActiveTab(tabs.tab3.tabName);
  90  |     });
  91  | 
  92  |     test('TC_QNC_003-Verify multiple conditions can be added within a single tab in questionnaire conditions', async () => {
  93  |         await questionnaireConditionsPage.clickOnTab('default tab');
  94  |         await questionnaireConditionsPage.addConditionToTabWithData(conditions.condition1);
  95  |         await questionnaireConditionsPage.verifyConditionAddedAndVisible(conditions.condition1.name);
  96  |         await questionnaireConditionsPage.addConditionToTabWithData(conditions.condition2);
  97  |         await questionnaireConditionsPage.verifyConditionAddedAndVisible(conditions.condition2.name);
  98  |     });
  99  | 
  100 |     test('TC_QNC_004-Verify search functionality filters conditions correctly within a tab in questionnaire conditions', async () => {
  101 |         await questionnaireConditionsPage.searchForCondition("default");
  102 |         await expect(questionnaireConditionsPage.conditionList.getByRole('listitem')).toHaveCount(1);
  103 |         await questionnaireConditionsPage.clearSearchInputText();
  104 |         await questionnaireConditionsPage.searchForCondition("unknow condition");
  105 |         await expect(questionnaireConditionsPage.conditionList.getByRole('listitem')).toHaveCount(0);
  106 |         await questionnaireConditionsPage.clearSearchInputText();
  107 |     });
  108 | 
  109 |     test('TC_QNC_005-Verify condition name and tab name can be updated in questionnaire conditions', async () => {
  110 |         await questionnaireConditionsPage.enterConditionName('RenamedCondition');
  111 |         await questionnaireConditionsPage.searchForCondition('');
  112 |         await questionnaireConditionsPage.verifyConditionAddedAndVisible('RenamedCondition');
  113 |         await questionnaireConditionsPage.clickOnEditIcon();
  114 |         await questionnaireConditionsPage.enterTabName('RenamedTab');
  115 |         await questionnaireConditionsPage.saveTab();
  116 |         await questionnaireConditionsPage.verifyTabCreated('RenamedTab');
  117 |         await questionnaireConditionsPage.verifyActiveTab('RenamedTab');
  118 |     });
  119 | 
  120 |     test('TC_QNC_006-Verify pre/post toggle can be switched and state updates correctly in questionnaire conditions', async () => {
  121 |         await expect(questionnaireConditionsPage.disablePostRadioButton).toHaveAttribute('aria-checked', 'true');
  122 |         await questionnaireConditionsPage.disablePostSubmission();
  123 |         await expect(questionnaireConditionsPage.disablePostRadioButton).toHaveAttribute('aria-checked', 'false');
  124 |     });
  125 | 
  126 |     test("TC_QNC_007-Verify a new condition rule can be added via 'Add Condition' button in questionnaire conditions", async () => {
  127 |         await questionnaireConditionsPage.clickAddCondition();
  128 |         await expect(questionnaireConditionsPage.conditionOnDropdown).toBeVisible();
  129 |         await expect(questionnaireConditionsPage.conditionOnDropdown.locator('xpath=ancestor::label')
  130 |             .locator('.q-field__native .ellipsis')).toHaveText('Questionnaire');
  131 |         await questionnaireConditionsPage.deleteConditionRule('Questionnaire')
  132 |     });
  133 | 
  134 |     test("TC_QNC_008-Verify 'Condition On' dropdown contains: Question, Variable, Calculation, Always, Non-Conformity, All/Not-All Finished in questionnaire conditions", async () => {
  135 |         await questionnaireConditionsPage.clickAddCondition();
  136 |         await questionnaireConditionsPage.clickConditionOnDropdown();
  137 |         await questionnaireConditionsPage.verifyDropdownOptionVisible(conditionOn.questionnaire.value);
  138 |         await questionnaireConditionsPage.verifyDropdownOptionVisible(conditionOn.variable.value);
  139 |         await questionnaireConditionsPage.verifyDropdownOptionVisible(conditionOn.calculation.value);
  140 |         await questionnaireConditionsPage.verifyDropdownOptionVisible(conditionOn.always.value);
  141 |         await questionnaireConditionsPage.verifyDropdownOptionVisible(conditionOn.nonConfirmity.value);
  142 |         await questionnaireConditionsPage.verifyDropdownOptionVisible(conditionOn.allQuestionnaireFinished.value);
  143 |         await questionnaireConditionsPage.verifyDropdownOptionVisible(conditionOn.notAllQuestionnaireFinished.value);
  144 |     });
  145 | 
  146 |     test("TC_QNC_009-Verify condition rule of type 'Questionnaire' can be created with page, where, operator, data in questionnaire conditions", async () => {
  147 |         await questionnaireConditionsPage.clickAddCondition();
  148 |         await questionnaireConditionsPage.selectConditionOn(conditionOn.questionnaire.value);
  149 |         await questionnaireConditionsPage.selectPageNameInCondition(conditionOn.questionnaire.pageName);
  150 |         await questionnaireConditionsPage.selectWhereInCondition(conditionOn.questionnaire.where);
  151 |         await questionnaireConditionsPage.selectOperatorInCondition(conditionOn.questionnaire.operator);
  152 |         await questionnaireConditionsPage.enterValueInCondition(conditionOn.questionnaire.conditionvalue);
  153 |     });
  154 | 
  155 |     test("TC_QNC_010-Verify condition rule of type 'Calculation' can be created with formula, operator, value in questionnaire conditions", async () => {
  156 |         await questionnaireConditionsPage.clickAddCondition();
  157 |         await questionnaireConditionsPage.selectConditionOn(conditionOn.calculation.value);
  158 |         await questionnaireConditionsPage.enterCalculationFormulaInCondition(conditionOn.calculation.formula);
  159 |         await questionnaireConditionsPage.selectOperatorInCondition(conditionOn.calculation.operator);
  160 |         await questionnaireConditionsPage.enterValueInCondition(conditionOn.calculation.conditionvalue);
  161 |     });
  162 | 
  163 |     test("TC_QNC_011-Verify condition rule of type 'Variable' can be created with where, operator, value in questionnaire conditions", async () => {
  164 |         await questionnaireConditionsPage.clickAddCondition();
  165 |         await questionnaireConditionsPage.selectConditionOn(conditionOn.variable.value);
  166 |         await questionnaireConditionsPage.enterWhereInputInCondition(conditionOn.variable.where);
  167 |         await questionnaireConditionsPage.selectOperatorInCondition(conditionOn.variable.operator);
  168 |         await questionnaireConditionsPage.enterValueInCondition(conditionOn.variable.conditionvalue);
  169 |     });
  170 | 
  171 |     test("TC_QNC_012-Verify condition rule of type 'Always' can be created successfully in questionnaire conditions", async () => {
  172 |         await questionnaireConditionsPage.createCondition('Always')
  173 |         await questionnaireConditionsPage.clickAddCondition();
  174 |         await questionnaireConditionsPage.selectConditionOn(conditionOn.always.value);
```