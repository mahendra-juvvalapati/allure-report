# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: questionnaireSettings.spec.ts >> Questionnaire settings tab Tests >> TC-SE-001-Verify Settings tab is selected by default and all required fields are visible
- Location: tests/questionnaireSettings.spec.ts:53:9

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
  1   | import {  test } from '@playwright/test';
  2   | import { LoginPage } from '../src/pages/login.page';
  3   | import { LeftNavigation } from '../src/pages/leftNavigations.page';
  4   | import { KnowledgeDataBasePage } from '../src/pages/knowledgeDataBase.page';
  5   | import { QuestionnairePage } from '../src/pages/knowledgeDatabase/questionnaire.page';
  6   | import { SettingsPage } from '../src/pages/knowledgeDatabase/questionnaireForms/configuration/settings.page';
  7   | import SETTINGS from '../fixtures/settings.json';
  8   | 
  9   | const COMPANY_NAME = 'QA Automation';
  10  | const CATEGORY = 'Questionnaire';
  11  | const TIME_SUFFIX = Date.now();
  12  | const QUESTIONNAIRE_NAME = `Questionnaire_${TIME_SUFFIX}`;
  13  | const QUESTIONNAIRE_TITLE = `Title_${TIME_SUFFIX}`;
  14  | 
  15  | 
  16  | let loginPage: LoginPage;
  17  | let leftNav: LeftNavigation;
  18  | let kdPage: KnowledgeDataBasePage;
  19  | let questionnairePage: QuestionnairePage;
  20  | let settingsPage: SettingsPage;
  21  | let settings = SETTINGS;
  22  | let page: any;
  23  | 
  24  | test.describe('Questionnaire settings tab Tests', () => {
  25  |     test.beforeAll(async ({ browser }) => {
  26  |         page = await browser.newPage();
  27  |         loginPage = new LoginPage(page);
  28  |         leftNav = new LeftNavigation(page);
  29  |         kdPage = new KnowledgeDataBasePage(page);
  30  |         questionnairePage = new QuestionnairePage(page);
  31  |         settingsPage = new SettingsPage(page);
  32  | 
  33  |         await loginPage.goto();
  34  |         await loginPage.signInWith();
  35  |         test.setTimeout(180000);
  36  |         await leftNav.clickOnKnowledgeDatabase();
  37  |         await kdPage.clickOnCompanyName(COMPANY_NAME);
  38  |         await leftNav.clickOnMaintain();
  39  |         await leftNav.clickOnQuestionnairesAndForms();
  40  |         await kdPage.clickOnNoThanksPopup();
  41  | 
  42  |         await questionnairePage.createNewQuestionnaire(
  43  |             QUESTIONNAIRE_NAME,
  44  |             QUESTIONNAIRE_TITLE,
  45  |             CATEGORY,
  46  |         );
  47  |     });
  48  |     
  49  |     test.afterAll(async () => {
> 50  |         await page.close();
      |                    ^ TypeError: Cannot read properties of undefined (reading 'close')
  51  |     });
  52  | 
  53  |     test('TC-SE-001-Verify Settings tab is selected by default and all required fields are visible', async () => {
  54  |         await settingsPage.verifySettingsTabIsSelected();
  55  |         await settingsPage.verifyAllFieldsAreVisible(settings)
  56  |     });
  57  | 
  58  |     test('TC-SE-002-Verify all 11 settings options are displayed under the Settings tab', async () => {
  59  |         await settingsPage.verifyAllSettingsOptions();
  60  |     });
  61  | 
  62  |     test('TC-SE-003-Verify each Questionnaire settings checkbox can be checked and unchecked ', async () => {
  63  |         for (const [label, value] of Object.entries(settings.settingsOptions)) {
  64  |             await settingsPage.checkTheQuestionnaireSetting(label);
  65  |         }
  66  |         for (const [label, value] of Object.entries(settings.settingsOptions)) {
  67  |             await settingsPage.uncheckTheQuestionnaireSetting(label);
  68  |         }
  69  |     });
  70  | 
  71  |     test('TC-SE-004-Verify questionnaire type can be changed from Settings tab', async () => {
  72  |         for (const option of settings.dropdowns[0].questionnaireType.Options) {
  73  |             await settingsPage.ChangeQuestionnaireType(option);
  74  |         }
  75  |     });
  76  | 
  77  |     test('TC-SE-005-Verify questionnaire status can be changed from the Settings tab', async () => {
  78  |         for (const option of settings.dropdowns[0].questionnaireStatus.Options) {
  79  |             await settingsPage.ChangeQuestionnaireStatus(option);
  80  |         }
  81  |     });
  82  | 
  83  |     test('TC-SE-006-Verify description field accepts input and saves successfully', async () => {
  84  |         await settingsPage.addDescriptionToQuestionnaire(settings.inputs.description);
  85  |     });
  86  | 
  87  |     test('TC-SE-007-Verify questionnaire name and code fields can be updated and saved in Settings page', async () => {
  88  |         await settingsPage.updateQuestionnaireName(settings.inputs.QuestionnaireName);
  89  |         await settingsPage.updateQuestionnaireCode(settings.inputs.QuestionnaireCode);
  90  |     });
  91  | 
  92  |     test('TC-SE-008-Verify Owner and Created By and updated  fields shows correct user in Settings page', async () => {
  93  |         await settingsPage.verifyOwnerAndCreatedByFields();
  94  |         await settingsPage.ChangeOwnerAndVerify();
  95  |         await settingsPage.verifycreatedByFieldIsDisabled();
  96  |         await settingsPage.verifyupdatedByFieldIsDisabled();
  97  |     });
  98  | 
  99  |     test('TC-SE-009-Verify creation and updated date displays in dd-mm-yyyy format and matches creation date', async () => {
  100 |         await settingsPage.verifyCreationDateFormatAndValue();
  101 |     });
  102 | 
  103 |     test('TC-SE-010-Verify questionnaire Expiry Time defaults to 30 days and can be updated in settings tab', async () => {
  104 |         await settingsPage.verifyTheQuestionnaireExpiryTime(settings.inputs.QuestionnaireExpiryTime);
  105 |         await settingsPage.updateQuestionnaireExpiryTime('60');
  106 |         await settingsPage.updateQuestionnaireExpiryTime('20');
  107 |     });
  108 | 
  109 |     test('TC-SE-011-Verify Card Photo is displayed and can be upload pictures in settings tab', async () => {
  110 |         await settingsPage.verifyCardPhotoIsDisplayed();
  111 |         await settingsPage.uploadCardPhoto('fic_image.jpg');
  112 |     });
  113 | 
  114 | });
  115 | 
```