# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: questionnaireIndicators.spec.ts >> Indicators Tab Tests >> TC_IN_001-Verify Indicators tab is visible and accessible within questionnaire
- Location: tests/questionnaireIndicators.spec.ts:76:9

# Error details

```
"beforeAll" hook timeout of 600000ms exceeded.
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
  8   | import { IndicatorsPage } from '../src/pages/knowledgeDatabase/questionnaireForms/configuration/indicators.page';
  9   | import indicatorsData from '../fixtures/indicators.json';
  10  | 
  11  | test.describe('Indicators Tab Tests', () => {
  12  | 
  13  |     let page: Page;
  14  |     let leftNav: LeftNavigation;
  15  |     let kdPage: KnowledgeDataBasePage;
  16  |     let questionnairePage: QuestionnairePage;
  17  |     let questionsPage: QuestionsPage;
  18  |     let editPage: QuestionnaireEditPage;
  19  |     let indicatorsPage: IndicatorsPage;
  20  |     let timeSuffix: number;
  21  |     const questionnaireCreation = indicatorsData.questionnaire;
  22  |     const questions = indicatorsData.questions;
  23  |     const indicators = indicatorsData.indicators;
  24  |     const perspective = indicatorsData.indicators.perspective;
  25  |     const group = indicatorsData.indicators.group;
  26  |     const classification = indicatorsData.indicators.classification;
  27  |     const trendType = indicatorsData.indicators.trendType;
  28  |     const widgetType = indicatorsData.indicators.widgetType;
  29  | 
> 30  |     test.beforeAll(async ({ browser }) => {
      |          ^ "beforeAll" hook timeout of 600000ms exceeded.
  31  |         page = await browser.newPage();
  32  |         const loginPage = new LoginPage(page);
  33  |         await loginPage.goto();
  34  |         await loginPage.signInWith();
  35  | 
  36  |         leftNav = new LeftNavigation(page);
  37  |         kdPage = new KnowledgeDataBasePage(page);
  38  |         questionnairePage = new QuestionnairePage(page);
  39  |         questionsPage = new QuestionsPage(page);
  40  |         editPage = new QuestionnaireEditPage(page);
  41  |         indicatorsPage = new IndicatorsPage(page);
  42  |         timeSuffix = Date.now();
  43  | 
  44  | 
  45  |         // Navigate to questionnaire configuration
  46  |         await leftNav.clickOnKnowledgeDatabase();
  47  |         await kdPage.clickOnCompanyName('QA Automation');
  48  |         await leftNav.clickOnMaintain();
  49  |         await leftNav.clickOnQuestionnairesAndForms();
  50  |         await kdPage.clickOnNoThanksPopup();
  51  | 
  52  |         // Create a Questionnaire
  53  |         const uniqueName = `${questionnaireCreation.name}_${timeSuffix}`;
  54  |         questionnaireCreation.name = uniqueName;
  55  |         await questionnairePage.clickOnAddNewQuestionnaire();
  56  |         await questionnairePage.createNewQuestionnaireWithData(questionnaireCreation);
  57  | 
  58  |         //Create questions
  59  |         await editPage.clickOnQuestionnaireTab();
  60  |         await questionsPage.configureQuestion(questions.Text);
  61  |         await questionsPage.configureQuestion(questions.Email);
  62  | 
  63  |         // Navigate to indicators page and create default indicator
  64  |         await editPage.clickOnIndicatorsTab();
  65  |         await page.waitForTimeout(1000);
  66  |         await indicatorsPage.clickAddNewKpi();
  67  |         await indicatorsPage.enterIndicatorName('Default KPI');
  68  |         await indicatorsPage.selectIndicatorType('Key Risk Indicator (KRI)');
  69  |         await indicatorsPage.clickCreate();
  70  |     });
  71  | 
  72  |     test.afterAll(async () => {
  73  |         await page.close();
  74  |     });
  75  | 
  76  |     test('TC_IN_001-Verify Indicators tab is visible and accessible within questionnaire', async () => {
  77  |         await editPage.clickOnIndicatorsTab();
  78  |         await expect(editPage.indicatorsTab).toHaveAttribute('aria-selected', 'true');
  79  |     });
  80  | 
  81  |     test('TC_IN_002-Verify create button is disabled when no data entered', async () => {
  82  |         await indicatorsPage.clickAddNewKpi();
  83  |         await expect(indicatorsPage.createButton).toBeDisabled();
  84  |         await indicatorsPage.closeDialog();
  85  |     });
  86  | 
  87  |     test('TC_IN_003-Verify name field is mandatory to create new KPI', async () => {
  88  |         await indicatorsPage.clickAddNewKpi();
  89  |         await indicatorsPage.enterIndicatorName('');
  90  |         await indicatorsPage.clickIndicatorTypeDropdown();
  91  |         await indicatorsPage.verifyRequiredFieldError('Name');
  92  |         await indicatorsPage.closeDialog();
  93  |     });
  94  | 
  95  |     test('TC_IN_004-Verify all fields are displayed in the KPI creation modal', async () => {
  96  |         await indicatorsPage.clickAddNewKpi();
  97  |         await expect(indicatorsPage.nameInput).toBeVisible();
  98  |         await expect(indicatorsPage.typeIndicatorDropdown).toBeVisible();
  99  |         await expect(indicatorsPage.createButton).toBeVisible();
  100 |         await indicatorsPage.closeDialog();
  101 |     });
  102 | 
  103 |     test('TC_IN_005-Verify KPI type options (KRI, KCI, KPI) are  visible under indicators type dropdown', async () => {
  104 |         await indicatorsPage.clickAddNewKpi();
  105 |         await indicatorsPage.clickIndicatorTypeDropdown();
  106 |         await indicatorsPage.verifyDropdownOptionVisible(indicators.keyRiskIndicator.type);
  107 |         await indicatorsPage.verifyDropdownOptionVisible(indicators.keyControlIndicator.type);
  108 |         await indicatorsPage.verifyDropdownOptionVisible(indicators.keyPerformanceIndicator.type);
  109 |         await indicatorsPage.closeDialog();
  110 |     });
  111 | 
  112 |     test("TC_IN_006-Verify a Key Risk Indicator (KRI) can be created successfully", async () => {
  113 |         await indicatorsPage.createKpiWithData(indicators.keyRiskIndicator);
  114 |         await indicatorsPage.verifyIndicatorAddedAndVisible(indicators.keyRiskIndicator.name);
  115 |     });
  116 | 
  117 |     test("TC_IN_007-Verify a Key Control Indicator (KCI) can be created successfully", async () => {
  118 |         await indicatorsPage.createKpiWithData(indicators.keyControlIndicator);
  119 |         await indicatorsPage.verifyIndicatorAddedAndVisible(indicators.keyControlIndicator.name);
  120 |     });
  121 | 
  122 |     test("TC_IN_008-Verify a Key Performance Indicator (KPI) can be created successfully", async () => {
  123 |         await indicatorsPage.createKpiWithData(indicators.keyPerformanceIndicator);
  124 |         await indicatorsPage.verifyIndicatorAddedAndVisible(indicators.keyPerformanceIndicator.name);
  125 |     });
  126 | 
  127 |     test("TC_IN_009-Verify all fields in the KPI Indicator tab are displayed correctly", async () => {
  128 |         await expect(indicatorsPage.indicatorTypeDropdown).toBeVisible();
  129 |         await expect(indicatorsPage.perspectiveDropdown).toBeVisible();
  130 |         await expect(indicatorsPage.groupDropdown).toBeVisible();
```