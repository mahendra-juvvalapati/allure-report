# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: questionCondition.spec.ts >> Question Condition Tests >> TC_QC_001-Verify a new condition tab can be created with name and description in question conditions
- Location: tests/questionCondition.spec.ts:77:9

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
  8   | import { QuestionConditionsPage } from '../src/pages/knowledgeDatabase/questionnaireForms/configuration/questionConditions.page';
  9   | import questionConditionsData from '../fixtures/questionConditon.json';
  10  | 
  11  | test.describe('Question Condition Tests', () => {
  12  | 
  13  |     let page: Page;
  14  |     let leftNav: LeftNavigation;
  15  |     let kdPage: KnowledgeDataBasePage;
  16  |     let questionnairePage: QuestionnairePage;
  17  |     let questionsPage: QuestionsPage;
  18  |     let editPage: QuestionnaireEditPage;
  19  |     let questionConditionsPage: QuestionConditionsPage;
  20  |     let timeSuffix: number;
  21  |     const questionnaireCreation = questionConditionsData.questionnaire;
  22  |     const questions = questionConditionsData.questions;
  23  |     const tabs = questionConditionsData.tabs;
  24  |     const conditions = questionConditionsData.conditions;
  25  |     const triggerOn = questionConditionsData.triggerOn;
  26  |     const actionType = questionConditionsData.actionType;
  27  |     const conditionOn = questionConditionsData.conditionOn;
  28  | 
  29  |     test.beforeAll(async ({ browser }) => {
  30  |         page = await browser.newPage();
  31  |         const loginPage = new LoginPage(page);
  32  |         await loginPage.goto();
  33  |         await loginPage.signInWith();
  34  | 
  35  |         leftNav = new LeftNavigation(page);
  36  |         kdPage = new KnowledgeDataBasePage(page);
  37  |         questionnairePage = new QuestionnairePage(page);
  38  |         questionsPage = new QuestionsPage(page);
  39  |         editPage = new QuestionnaireEditPage(page);
  40  |         questionConditionsPage = new QuestionConditionsPage(page);
  41  |         timeSuffix = Date.now();
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
  56  |         // Create questions
  57  |         await editPage.clickOnQuestionnaireTab();
  58  |         await questionsPage.configureQuestion(questions.Text);
  59  |         await questionsPage.configureQuestion(questions.Email);
  60  |         await questionsPage.configureQuestion(questions.User);
  61  |         await questionsPage.configureQuestion(questions.Stars);
  62  | 
  63  |         // Navigate to question condition tab
  64  |         await editPage.clickOnQuestionConditionsTab();
  65  |         await questionConditionsPage.clickAddTab();
  66  |         await questionConditionsPage.fillTabDetails("default tab", "This is a default tab");
  67  |         await questionConditionsPage.saveTab();
  68  |         await questionConditionsPage.clickAddConditionTab();
  69  |         await questionConditionsPage.enterConditionName("default");
  70  |         await questionConditionsPage.submitCondition();
  71  |     });
  72  | 
  73  |     test.afterAll(async () => {
> 74  |         await page.close();
      |                    ^ TypeError: Cannot read properties of undefined (reading 'close')
  75  |     });
  76  | 
  77  |     test('TC_QC_001-Verify a new condition tab can be created with name and description in question conditions', async () => {
  78  |         await questionConditionsPage.createNewConditionTabWithData(tabs.tab1);
  79  |         await questionConditionsPage.verifyTabCreated(tabs.tab1.tabName);
  80  |         await questionConditionsPage.verifyActiveTab(tabs.tab1.tabName);
  81  |     });
  82  | 
  83  |     test('TC_QC_002-Verify multiple condition tabs can be created and all visible in question conditions', async () => {
  84  |         await questionConditionsPage.createNewConditionTabWithData(tabs.tab2);
  85  |         await questionConditionsPage.verifyTabCreated(tabs.tab2.tabName);
  86  |         await questionConditionsPage.verifyActiveTab(tabs.tab2.tabName);
  87  |         await questionConditionsPage.createNewConditionTabWithData(tabs.tab3);
  88  |         await questionConditionsPage.verifyTabCreated(tabs.tab3.tabName);
  89  |         await questionConditionsPage.verifyActiveTab(tabs.tab3.tabName);
  90  |     });
  91  | 
  92  |     test('TC_QC_003-Verify multiple conditions can be added within a single tab in question conditions', async () => {
  93  |         await questionConditionsPage.clickOnTab('default tab');
  94  |         await questionConditionsPage.addConditionToTabWithData(conditions.condition1);
  95  |         await questionConditionsPage.verifyConditionAddedAndVisible(conditions.condition1.name);
  96  |         await questionConditionsPage.addConditionToTabWithData(conditions.condition2);
  97  |         await questionConditionsPage.verifyConditionAddedAndVisible(conditions.condition2.name);
  98  |     });
  99  | 
  100 |     test('TC_QC_004-Verify search functionality filters conditions correctly within a tab in question conditions', async () => {
  101 |         await questionConditionsPage.searchForCondition("default");
  102 |         await expect(questionConditionsPage.conditionList.getByRole('listitem')).toHaveCount(1);
  103 |         await questionConditionsPage.clearSearchInputText();
  104 |         await questionConditionsPage.searchForCondition("unknow condition");
  105 |         await expect(questionConditionsPage.conditionList.getByRole('listitem')).toHaveCount(0);
  106 |         await questionConditionsPage.clearSearchInputText();
  107 |     });
  108 | 
  109 |     test('TC_QC_005-Verify condition name and tab name can be updated in question conditions', async () => {
  110 |         await questionConditionsPage.enterConditionName('RenamedCondition');
  111 |         await questionConditionsPage.clickTriggerOnDropdown();
  112 |         await questionConditionsPage.verifyConditionAddedAndVisible('RenamedCondition');
  113 |         await questionConditionsPage.clickOnEditIcon();
  114 |         await questionConditionsPage.enterTabName('RenamedTab');
  115 |         await questionConditionsPage.saveTab();
  116 |         await questionConditionsPage.verifyTabCreated('RenamedTab');
  117 |         await questionConditionsPage.verifyActiveTab('RenamedTab');
  118 |     });
  119 | 
  120 |     test("TC_QC_006-Verify 'Trigger On' dropdown contains all three types: Entering, Change a Question, Completing Page in question conditions", async () => {
  121 |         await questionConditionsPage.clickTriggerOnDropdown();
  122 |         await questionConditionsPage.verifyDropdownOptionVisible(triggerOn.changeQuestion.value);
  123 |         await questionConditionsPage.verifyDropdownOptionVisible(triggerOn.enteringQuestionnaireFirstTime.value);
  124 |         await questionConditionsPage.verifyDropdownOptionVisible(triggerOn.completeingPage.value);
  125 |         await questionConditionsPage.clickTriggerOnDropdown();
  126 |     });
  127 | 
  128 |     test("TC_QC_007-Verify all three 'Trigger On' types can be selected and respective fields can be configured in question conditions", async () => {
  129 |         await questionConditionsPage.configureEnteringQuestionnaireFirstTimeTrigger(triggerOn.enteringQuestionnaireFirstTime);
  130 |         await questionConditionsPage.configureCompletingPageTrigger(triggerOn.completeingPage);
  131 |         await questionConditionsPage.configureChangeaQuestionTrigger(triggerOn.changeQuestion);
  132 |     });
  133 | 
  134 |     test("TC_QC_008-Verify a new condition rule can be added via 'Add Condition' button in question conditions", async () => {
  135 |         await questionConditionsPage.clickAddConditionButton();
  136 |         await expect(questionConditionsPage.conditionTypeDropdown).toBeVisible();
  137 |         await expect(questionConditionsPage.conditionTypeDropdown.locator('xpath=ancestor::label')
  138 |             .locator('.q-field__native .ellipsis')).toHaveText('Question');
  139 |     });
  140 | 
  141 |     test("TC_QC_009-Verify 'Condition On' dropdown contains: Question, Variable, Calculation in question conditions", async () => {
  142 |         await questionConditionsPage.clickConditionOnDropdown();
  143 |         await questionConditionsPage.verifyDropdownOptionVisible(conditionOn.question.value);
  144 |         await questionConditionsPage.verifyDropdownOptionVisible(conditionOn.variable.value);
  145 |         await questionConditionsPage.verifyDropdownOptionVisible(conditionOn.calculation.value);
  146 |     });
  147 | 
  148 |     test("TC_QC_010-Verify condition rule of type 'Question' can be created with page, where, operator, data in question conditions", async () => {
  149 |         await questionConditionsPage.addCondition(conditionOn.question.value);
  150 |         await questionConditionsPage.selectPageNameInCondition(conditionOn.question.pageName);
  151 |         await questionConditionsPage.selectWhereInCondition(conditionOn.question.where);
  152 |         await questionConditionsPage.selectOperatorInCondition(conditionOn.question.operator);
  153 |         await questionConditionsPage.enterValueInCondition(conditionOn.question.conditionvalue);
  154 |     });
  155 | 
  156 |     test("TC_QC_011-Verify condition rule of type 'Calculation' can be created with formula, operator, value in question conditions", async () => {
  157 |         await questionConditionsPage.addCondition(conditionOn.calculation.value);
  158 |         await questionConditionsPage.enterCalculationFormulaInCondition(conditionOn.calculation.formula);
  159 |         await questionConditionsPage.selectOperatorInCondition(conditionOn.calculation.operator);
  160 |         await questionConditionsPage.enterValueInCondition(conditionOn.calculation.conditionvalue);
  161 |     });
  162 | 
  163 |     test("TC_QC_012-Verify condition rule of type 'Variable' can be created with where, operator, value in question conditions", async () => {
  164 |         await questionConditionsPage.addCondition(conditionOn.variable.value);
  165 |         await questionConditionsPage.enterWhereInputInCondition(conditionOn.variable.where);
  166 |         await questionConditionsPage.selectOperatorInCondition(conditionOn.variable.operator);
  167 |         await questionConditionsPage.enterValueInCondition(conditionOn.variable.conditionvalue);
  168 |     });
  169 | 
  170 |     test('TC_QC_013-Verify condition rule can be deleted in question conditions', async () => {
  171 |         await questionConditionsPage.clickAddConditionButton();
  172 |         await questionConditionsPage.deleteConditionRule();
  173 |     });
  174 | 
```