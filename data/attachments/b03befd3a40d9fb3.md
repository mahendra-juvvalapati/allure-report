# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: QuestionnaireQuestions.spec.ts >> Questionnaire Questions tab Tests >> TC-QQ-006-Verify a page with no questions can be deleted successfully
- Location: tests/QuestionnaireQuestions.spec.ts:92:9

# Error details

```
Error: expect(received).toBe(expected) // Object.is equality

Expected: 3
Received: 4
```

# Page snapshot

```yaml
- generic [ref=e1]:
  - text: ×
  - link "ticket or feedback" [ref=e2] [cursor=pointer]:
    - /url: javascript:void(0)
    - img "ticket or feedback" [ref=e3]
  - main [ref=e6]:
    - generic [ref=e9]:
      - generic [ref=e10]:
        - generic [ref=e12]:
          - button "leftMenuOpen" [ref=e13] [cursor=pointer]:
            - img [ref=e14]
          - img [ref=e19]
          - button "Turn off admin role" [ref=e22] [cursor=pointer]:
            - img [ref=e23]:
              - img
          - button [ref=e25] [cursor=pointer]:
            - img [ref=e27]:
              - img [ref=e28]
          - generic [ref=e33]:
            - button [ref=e34] [cursor=pointer]:
              - img [ref=e36]:
                - img [ref=e37]
            - status "97" [ref=e38]
          - button "fullscreen" [ref=e39] [cursor=pointer]:
            - generic [ref=e40]: fullscreen
          - button "Open beamer" [ref=e41] [cursor=pointer]:
            - img [ref=e42]:
              - img
            - generic [ref=e43]: "1"
          - button "freshDesk" [ref=e44] [cursor=pointer]:
            - generic [ref=e45]: info
        - generic [ref=e46]:
          - generic [ref=e47]:
            - img [ref=e48] [cursor=pointer]
            - button "dehaze" [ref=e49] [cursor=pointer]:
              - generic [ref=e50]: dehaze
          - list [ref=e51]:
            - generic [ref=e52]:
              - button "profile pic" [ref=e53]
              - generic [ref=e54]: mahendra j
            - button "keyboard_arrow_down mahendra.juvvalapati@qualitlabs.com" [ref=e55] [cursor=pointer]:
              - generic [ref=e56]: keyboard_arrow_down
              - generic [ref=e57]: mahendra.juvvalapati@qualitlabs.com
            - list [ref=e58]:
              - button "exit_to_app Logout" [ref=e59] [cursor=pointer]:
                - generic [ref=e60]: exit_to_app
                - generic [ref=e61]: Logout
          - list [ref=e63]:
            - button "home Dashboard" [ref=e64] [cursor=pointer]:
              - generic [ref=e65]: home
              - generic [ref=e66]: Dashboard
            - button "widgets Modules keyboard_arrow_down" [ref=e67] [cursor=pointer]:
              - generic [ref=e68]: widgets
              - generic [ref=e69]: Modules
              - generic [ref=e70]: keyboard_arrow_down
            - list [ref=e71]:
              - button "Strategy" [ref=e72] [cursor=pointer]:
                - img [ref=e73]:
                  - img
                - generic [ref=e74]: Strategy
              - button "Policy" [ref=e75] [cursor=pointer]:
                - img [ref=e76]:
                  - img
                - generic [ref=e77]: Policy
              - button "Programs" [ref=e78] [cursor=pointer]:
                - img [ref=e79]:
                  - img
                - generic [ref=e80]: Programs
              - button "projects" [ref=e81] [cursor=pointer]:
                - img [ref=e82]:
                  - img
                - generic [ref=e83]: projects
              - button "Dialogues" [ref=e84] [cursor=pointer]:
                - img [ref=e85]:
                  - img
                - generic [ref=e86]: Dialogues
              - button "Objectives" [ref=e87] [cursor=pointer]:
                - img [ref=e88]:
                  - img
                - generic [ref=e89]: Objectives
              - button "Processes" [ref=e90] [cursor=pointer]:
                - img [ref=e91]:
                  - img
                - generic [ref=e92]: Processes
              - button "Process steps" [ref=e93] [cursor=pointer]:
                - img [ref=e94]:
                  - img
                - generic [ref=e95]: Process steps
              - button "Organisation functions" [ref=e96] [cursor=pointer]:
                - img [ref=e97]:
                  - img
                - generic [ref=e98]: Organisation functions
              - button "KSF's - Opportunities" [ref=e99] [cursor=pointer]:
                - img [ref=e100]:
                  - img
                - generic [ref=e101]: KSF's - Opportunities
              - button "Stakeholders" [ref=e102] [cursor=pointer]:
                - img [ref=e103]:
                  - img
                - generic [ref=e104]: Stakeholders
              - button "Causes" [ref=e105] [cursor=pointer]:
                - img [ref=e106]:
                  - img
                - generic [ref=e107]: Causes
              - button "Risks" [ref=e108] [cursor=pointer]:
                - img [ref=e109]:
                  - img
                - generic [ref=e110]: Risks
              - button "Effects" [ref=e111] [cursor=pointer]:
                - img [ref=e112]:
                  - img
                - generic [ref=e113]: Effects
              - button "Opportunities" [ref=e114] [cursor=pointer]:
                - img [ref=e115]:
                  - img
                - generic [ref=e116]: Opportunities
              - button "Standards Frameworks" [ref=e117] [cursor=pointer]:
                - img [ref=e118]:
                  - img
                - generic [ref=e119]: Standards Frameworks
              - button "Laws and regulations" [ref=e120] [cursor=pointer]:
                - img [ref=e121]:
                  - img
                - generic [ref=e122]: Laws and regulations
              - button "Measures" [ref=e123] [cursor=pointer]:
                - img [ref=e124]:
                  - img
                - generic [ref=e125]: Measures
              - button "Assets" [ref=e126] [cursor=pointer]:
                - img [ref=e127]:
                  - img
                - generic [ref=e128]: Assets
              - button "Information systems" [ref=e129] [cursor=pointer]:
                - img [ref=e130]:
                  - img
                - generic [ref=e131]: Information systems
              - button "Processing" [ref=e132] [cursor=pointer]:
                - img [ref=e133]:
                  - img
                - generic [ref=e134]: Processing
              - button "Audits" [ref=e135] [cursor=pointer]:
                - img [ref=e136]:
                  - img
                - generic [ref=e137]: Audits
              - button "Audit sets" [ref=e138] [cursor=pointer]:
                - img [ref=e139]:
                  - img
                - generic [ref=e140]: Audit sets
              - button "Impact Assessments" [ref=e141] [cursor=pointer]:
                - img [ref=e142]:
                  - img
                - generic [ref=e143]: Impact Assessments
              - button "Tests" [ref=e144] [cursor=pointer]:
                - img [ref=e145]:
                  - img
                - generic [ref=e146]: Tests
              - button "Findings" [ref=e147] [cursor=pointer]:
                - img [ref=e148]:
                  - img
                - generic [ref=e149]: Findings
              - button "Problems" [ref=e150] [cursor=pointer]:
                - img [ref=e151]:
                  - img
                - generic [ref=e152]: Problems
              - button "Changes" [ref=e153] [cursor=pointer]:
                - img [ref=e154]:
                  - img
                - generic [ref=e155]: Changes
              - button "Cases" [ref=e156] [cursor=pointer]:
                - img [ref=e157]:
                  - img
                - generic [ref=e158]: Cases
              - button "Tasks" [ref=e159] [cursor=pointer]:
                - img [ref=e160]:
                  - img
                - generic [ref=e161]: Tasks
              - button "Documents" [ref=e162] [cursor=pointer]:
                - img [ref=e163]:
                  - img
                - generic [ref=e164]: Documents
              - button "News items" [ref=e165] [cursor=pointer]:
                - img [ref=e166]:
                  - img
                - generic [ref=e167]: News items
              - button "Related parties" [ref=e168] [cursor=pointer]:
                - img [ref=e169]:
                  - img
                - generic [ref=e170]: Related parties
              - button "Contracts" [ref=e171] [cursor=pointer]:
                - img [ref=e172]:
                  - img
                - generic [ref=e173]: Contracts
              - button "Vendors" [ref=e174] [cursor=pointer]:
                - img [ref=e175]:
                  - img
                - generic [ref=e176]: Vendors
              - button "Performance agreements" [ref=e177] [cursor=pointer]:
                - img [ref=e178]:
                  - img
                - generic [ref=e179]: Performance agreements
              - button "Key Figures" [ref=e180] [cursor=pointer]:
                - img [ref=e181]:
                  - img
                - generic [ref=e182]: Key Figures
              - button "Settings" [ref=e183] [cursor=pointer]:
                - img [ref=e184]:
                  - img
                - generic [ref=e185]: Settings
              - button "Critical Business Scenarios" [ref=e186] [cursor=pointer]:
                - img [ref=e187]:
                  - img
                - generic [ref=e188]: Critical Business Scenarios
              - button "BCM Plans" [ref=e189] [cursor=pointer]:
                - img [ref=e190]:
                  - img
                - generic [ref=e191]: BCM Plans
              - button "Context analysis" [ref=e192] [cursor=pointer]:
                - img [ref=e193]:
                  - img
                - generic [ref=e194]: Context analysis
              - button "Situations" [ref=e195] [cursor=pointer]:
                - img [ref=e196]:
                  - img
                - generic [ref=e197]: Situations
              - button "Planstappen" [ref=e198] [cursor=pointer]:
                - img [ref=e199]:
                  - img
                - generic [ref=e200]: Planstappen
              - button "BOBOC logs" [ref=e201] [cursor=pointer]:
                - img [ref=e202]:
                  - img
                - generic [ref=e203]: BOBOC logs
            - button "build Maintain keyboard_arrow_down" [ref=e204] [cursor=pointer]:
              - generic [ref=e205]: build
              - generic [ref=e206]: Maintain
              - generic [ref=e207]: keyboard_arrow_down
            - list [ref=e208]:
              - button "assignment_turned_in Questionnaires, forms" [ref=e209] [cursor=pointer]:
                - generic [ref=e210]: assignment_turned_in
                - generic [ref=e211]: Questionnaires, forms
              - button "Workflows & conditions" [ref=e212] [cursor=pointer]:
                - img [ref=e213]:
                  - img
                - generic [ref=e214]: Workflows & conditions
          - generic [ref=e217]:
            - button [ref=e218] [cursor=pointer]:
              - generic [ref=e220]:
                - img [ref=e222]
                - generic [ref=e224]: close
            - menu:
              - generic:
                - generic:
                  - generic:
                    - img
              - generic:
                - generic:
                  - generic:
                    - img
      - generic [ref=e228]:
        - generic [ref=e230]:
          - generic [ref=e231]:
            - generic [ref=e233]:
              - button [ref=e235] [cursor=pointer]:
                - img [ref=e237]: arrow_back
              - generic [ref=e239]:
                - generic [ref=e241] [cursor=pointer]: QualiTlabs
                - generic [ref=e243]: keyboard_arrow_right
                - generic [ref=e245] [cursor=pointer]: Templates
                - generic [ref=e247]: keyboard_arrow_right
                - generic [ref=e249] [cursor=pointer]: QA Automation
                - generic [ref=e251]: keyboard_arrow_right
                - generic [ref=e253] [cursor=pointer]: Questionnaires, forms
            - generic [ref=e255]:
              - button [ref=e256] [cursor=pointer]:
                - img [ref=e258]: content_copy
              - button "Publish" [ref=e259] [cursor=pointer]:
                - generic [ref=e260]:
                  - img [ref=e261]: file_upload
                  - generic [ref=e262]: Publish
              - button [ref=e263] [cursor=pointer]:
                - img [ref=e265]: more_vert
          - generic [ref=e266]: Questionnaire_1780297371829
        - generic [ref=e268]:
          - toolbar [ref=e270]:
            - tablist [ref=e271]:
              - generic [ref=e272]:
                - tab "Settings" [ref=e273] [cursor=pointer]:
                  - generic [ref=e275]: Settings
                - tab "Questionnaire" [selected] [ref=e277] [cursor=pointer]:
                  - generic [ref=e279]: Questionnaire
                - tab "QUESTION CONDITIONS" [ref=e281] [cursor=pointer]:
                  - generic [ref=e283]: QUESTION CONDITIONS
                - tab "QUESTIONNAIRE CONDITIONS" [ref=e285] [cursor=pointer]:
                  - generic [ref=e287]: QUESTIONNAIRE CONDITIONS
                - tab "Indicators" [ref=e289] [cursor=pointer]:
                  - generic [ref=e291]: Indicators
          - tabpanel [ref=e295]:
            - tabpanel [ref=e296]:
              - generic [ref=e297]:
                - generic [ref=e299]:
                  - toolbar [ref=e301]:
                    - generic [ref=e306] [cursor=pointer]:
                      - generic [ref=e307]:
                        - generic [ref=e308]:
                          - generic [ref=e309]: (1-4) Page name 1
                          - combobox "(1-4) Page name 1 Selected questionnaire page" [expanded] [active] [ref=e310]: (1-4) Page name 1
                        - generic:
                          - generic: Selected questionnaire page
                      - generic [ref=e312]: arrow_drop_down
                    - button [ref=e313] [cursor=pointer]:
                      - img [ref=e315]: add
                    - button [ref=e316] [cursor=pointer]:
                      - img [ref=e318]: delete
                  - generic [ref=e319]:
                    - generic [ref=e320]:
                      - generic [ref=e326]:
                        - textbox "Page Title" [ref=e327]: Page name 1
                        - generic: Page Title
                      - checkbox "Disable" [ref=e329] [cursor=pointer]:
                        - img [ref=e332]
                        - generic [ref=e334]: Disable
                    - generic [ref=e338]: Drag here to add questions
                - generic [ref=e340]:
                  - toolbar [ref=e342]:
                    - tablist [ref=e343]:
                      - generic [ref=e344]:
                        - tab "DATA" [selected] [ref=e345] [cursor=pointer]:
                          - generic [ref=e347]: DATA
                        - tab "SELECT" [ref=e349] [cursor=pointer]:
                          - generic [ref=e351]: SELECT
                        - tab "WIDGETS" [ref=e353] [cursor=pointer]:
                          - generic [ref=e355]: WIDGETS
                  - tabpanel [ref=e359]:
                    - tabpanel [ref=e360]:
                      - generic [ref=e361]:
                        - generic [ref=e363]:
                          - button [ref=e364] [cursor=pointer]:
                            - img [ref=e366]: format_color_text
                          - text: text
                        - generic [ref=e368]:
                          - button [ref=e369] [cursor=pointer]:
                            - img [ref=e371]: event
                          - text: Date and / or time
                        - generic [ref=e373]:
                          - button [ref=e374] [cursor=pointer]:
                            - img [ref=e376]: http
                          - text: URL
                        - generic [ref=e378]:
                          - button [ref=e379] [cursor=pointer]:
                            - img [ref=e381]: subtitles
                          - text: Label
                        - generic [ref=e383]:
                          - button [ref=e384] [cursor=pointer]:
                            - img [ref=e386]: person
                          - text: user
                        - generic [ref=e388]:
                          - button [ref=e389] [cursor=pointer]:
                            - img [ref=e391]: email
                          - text: email
  - generic:
    - iframe
  - listbox [ref=e392]:
    - generic [ref=e393]:
      - option "(1-4) Page name 1" [selected] [ref=e394] [cursor=pointer]:
        - generic [ref=e396]: (1-4) Page name 1
      - option "(2-4) Self Details Updated" [ref=e397] [cursor=pointer]:
        - generic [ref=e399]: (2-4) Self Details Updated
      - option "(3-4) Page name 3" [ref=e400] [cursor=pointer]:
        - generic [ref=e402]: (3-4) Page name 3
      - option "(4-4) Page name 4" [ref=e403] [cursor=pointer]:
        - generic [ref=e405]: (4-4) Page name 4
```

# Test source

```ts
  1   | import { expect, test } from '@playwright/test';
  2   | import { LoginPage } from '../src/pages/login.page';
  3   | import { LeftNavigation } from '../src/pages/leftNavigations.page';
  4   | import { KnowledgeDataBasePage } from '../src/pages/knowledgeDataBase.page';
  5   | import { QuestionnairePage } from '../src/pages/knowledgeDatabase/questionnaire.page';
  6   | 
  7   | import { QuestionsPage } from '../src/pages/knowledgeDatabase/questionnaireForms/configuration/questions.page';
  8   | import { QuestionnaireEditPage } from '../src/pages/knowledgeDatabase/questionnaireForms/questionnaireEdit.page';
  9   | import QUESTIONS from '../fixtures/questions.json';
  10  | 
  11  | const COMPANY_NAME = 'QA Automation';
  12  | const CATEGORY = 'Questionnaire';
  13  | const TIME_SUFFIX = Date.now();
  14  | const QUESTIONNAIRE_NAME = `Questionnaire_${TIME_SUFFIX}`;
  15  | const QUESTIONNAIRE_TITLE = `Title_${TIME_SUFFIX}`;
  16  | 
  17  | 
  18  | let loginPage: LoginPage;
  19  | let leftNav: LeftNavigation;
  20  | let kdPage: KnowledgeDataBasePage;
  21  | let questionnairePage: QuestionnairePage;
  22  | let questions = QUESTIONS;
  23  | let questionsPage: QuestionsPage;
  24  | let page: any;
  25  | let editPage: QuestionnaireEditPage;
  26  | 
  27  | 
  28  | test.describe('Questionnaire Questions tab Tests', () => {
  29  |     test.beforeAll(async ({ browser }) => {
  30  |         page = await browser.newPage();
  31  |         loginPage = new LoginPage(page);
  32  |         leftNav = new LeftNavigation(page);
  33  |         kdPage = new KnowledgeDataBasePage(page);
  34  |         questionnairePage = new QuestionnairePage(page);
  35  |         questionsPage = new QuestionsPage(page);
  36  |         editPage = new QuestionnaireEditPage(page);
  37  | 
  38  |         await loginPage.goto();
  39  |         await loginPage.signInWith();
  40  |         test.setTimeout(180000);
  41  |         await leftNav.clickOnKnowledgeDatabase();
  42  |         await kdPage.clickOnCompanyName(COMPANY_NAME);
  43  |         await leftNav.clickOnMaintain();
  44  |         await leftNav.clickOnQuestionnairesAndForms();
  45  |         await kdPage.clickOnNoThanksPopup();
  46  |         await questionnairePage.createNewQuestionnaire(
  47  |             QUESTIONNAIRE_NAME,
  48  |             QUESTIONNAIRE_TITLE,
  49  |             CATEGORY,
  50  |         );
  51  | 
  52  |     });
  53  | 
  54  |     test('TC-QQ-001-Verify Questions tab is visible and can be opened successfully', async () => {
  55  |         await editPage.verifyQuestionnaireTabIsVisible();
  56  |         await editPage.clickOnQuestionnaireTab();
  57  |     });
  58  | 
  59  |     test('TC-QQ-002-Verify all page fields (page selector, title, drag-drop area, Data/Select/Widgets tabs) are displayed', async () => {
  60  |         await editPage.clickOnQuestionnaireTab();
  61  |         await questionsPage.verifyPageSelectorIsVisible();
  62  |         await questionsPage.verifyPageTitleIsVisible();
  63  |         await questionsPage.verifyDragAndDropAreaIsVisible();
  64  |         await questionsPage.verifyDataTabIsVisible();
  65  |         await questionsPage.verifySelectTabIsVisible();
  66  |         await questionsPage.verifyWidgetsTabIsVisible();
  67  |     });
  68  | 
  69  |     test('TC-QQ-003-Verify a new page can be added and appears in the page selector dropdown', async () => {
  70  |         await editPage.clickOnQuestionnaireTab();
  71  |         const initialCount = await questionsPage.getPageSelectorOptionCount();
  72  |         await questionsPage.clickAddNewPage();
  73  |         const updatedCount = await questionsPage.getPageSelectorOptionCount();
  74  |         expect(updatedCount).toBe(initialCount + 1);
  75  |     });
  76  | 
  77  |     test('TC-QQ-004-Verify questionnaire page title can be updated and changes are reflected', async () => {
  78  |         await editPage.clickOnQuestionnaireTab();
  79  |         const newTitle = questions.pageTitle + ' Updated';
  80  |         await questionsPage.updateQuestionnaireTitle(newTitle);
  81  |         await questionsPage.verifyQuestionnaireTitle(newTitle);
  82  |     });
  83  |     test('TC-QQ-005-Verify a page can be enabled and disabled ', async () => {
  84  |         await editPage.clickOnQuestionnaireTab();
  85  |         await questionsPage.clickAddNewPage();
  86  |         await questionsPage.updatePageState(true);
  87  |         await questionsPage.verifyPageState('disabled');
  88  |         await questionsPage.updatePageState(false);
  89  |         await questionsPage.verifyPageState('enabled');
  90  |     });
  91  | 
  92  |     test('TC-QQ-006-Verify a page with no questions can be deleted successfully', async () => {
  93  |         await editPage.clickOnQuestionnaireTab();
  94  |         const initialCount = await questionsPage.getPageSelectorOptionCount();
  95  |         await questionsPage.clickAddNewPage();
  96  |         await questionsPage.deleteCurrentPage();
  97  |         const finalCount = await questionsPage.getPageSelectorOptionCount();
> 98  |         expect(finalCount).toBe(initialCount);
      |                            ^ Error: expect(received).toBe(expected) // Object.is equality
  99  |     });
  100 | 
  101 |     test('TC-QQ-007-Verify delete button is not visible for a page that contains questions', async () => {
  102 |         await editPage.clickOnQuestionnaireTab();
  103 |         await questionsPage.dragAndDropQuestionnaire('Text');
  104 |         const config = questions.questionTypes.DATA['Text'];
  105 |         await questionsPage.updateTextQuestionDetails(config);
  106 |         await questionsPage.closeQuestionnaire();
  107 |         await questionsPage.verifyDeleteButtonNotVisible();
  108 |     });
  109 | 
  110 |     test('TC-QQ-008-Verify all question types are listed under Data, Select, and Widgets tabs', async () => {
  111 |         await editPage.clickOnQuestionnaireTab();
  112 |         const dataTypes = Object.keys(questions.questionTypes.DATA);
  113 |         const selectTypes = Object.keys(questions.questionTypes.SELECT);
  114 |         const widgetTypes = Object.keys(questions.questionTypes.WIDGETS);
  115 | 
  116 |         await questionsPage.verifyQuestionTypesInTab(questionsPage.dataTab, dataTypes);
  117 |         await questionsPage.verifyQuestionTypesInTab(questionsPage.selectTab, selectTypes);
  118 |         await questionsPage.verifyQuestionTypesInTab(questionsPage.widgetsTab, widgetTypes);
  119 |     });
  120 | 
  121 | 
  122 | 
  123 |     test('TC-QQ-010-Verify all action controls (avatar, title, display, disable, lock, copy, delete) are visible on a dropped question', async () => {
  124 |         await editPage.clickOnQuestionnaireTab();
  125 |         await questionsPage.clickAddNewPage();
  126 |         await questionsPage.dragAndDropQuestionnaire('Text');
  127 |         await questionsPage.verifyQuestionActionsVisible('TEXT Question');
  128 |     });
  129 | 
  130 |     test('TC-QQ-009-Verify all questions can be dragged and dropped onto the questionnaire page', async () => {
  131 |         await editPage.clickOnQuestionnaireTab();
  132 |         await questionsPage.clickAddNewPage();
  133 | 
  134 |         const allQuestionTypes = [
  135 |             ...Object.keys(questions.questionTypes.DATA),
  136 |             ...Object.keys(questions.questionTypes.SELECT),
  137 |             ...Object.keys(questions.questionTypes.WIDGETS),
  138 |         ];
  139 |         for (let index = 0; index < allQuestionTypes.length; index++) {
  140 |             const questionType = allQuestionTypes[index];
  141 |             await questionsPage.dragAndDropQuestionnaire(questionType);
  142 |             await questionsPage.assertDroppedItemsCount(index + 1);
  143 |         }
  144 |     });
  145 | 
  146 |     test('TC-QQ-011-Verify display setting button and all the display options are visible', async () => {
  147 |         await editPage.clickOnQuestionnaireTab();
  148 |         await questionsPage.clickAddNewPage();
  149 |         await questionsPage.dragAndDropQuestionnaire('Text');
  150 |         await questionsPage.clickQuestionDisplay('TEXT Question');
  151 |         await questionsPage.verifyAllDisplaySettingsAreVisible();
  152 |         for (const displaySetting of questions.displaySettings) {
  153 |             await questionsPage.clickOnDisplaySetting(displaySetting);
  154 |             await questionsPage.clickQuestionDisplay('TEXT Question');
  155 |         }
  156 |     });
  157 | 
  158 |     test('TC-QQ-012-Verify a question can be enabled and disabled via checkbox', async () => {
  159 |         await editPage.clickOnQuestionnaireTab();
  160 |         await questionsPage.clickAddNewPage();
  161 |         await questionsPage.dragAndDropQuestionnaire('Text');
  162 |         await questionsPage.toggleQuestionDisable('TEXT Question');
  163 |         await questionsPage.verifyQuestionDisableState('TEXT Question', false);
  164 |         await questionsPage.toggleQuestionDisable('TEXT Question');
  165 |         await questionsPage.verifyQuestionDisableState('TEXT Question', true);
  166 |     });
  167 | 
  168 |     test('TC-QQ-013-Verify a question can be locked and unlocked and editability changes accordingly', async () => {
  169 |         await editPage.clickOnQuestionnaireTab();
  170 |         await questionsPage.clickAddNewPage();
  171 |         await questionsPage.dragAndDropQuestionnaire('Text');
  172 |         await questionsPage.lockTheQuestion('TEXT Question');
  173 |         await questionsPage.verifyQuestionLockState('TEXT Question', false);
  174 |         await questionsPage.unlockTheQuestions('TEXT Question');
  175 |         await questionsPage.verifyQuestionLockState('TEXT Question', true);
  176 |     });
  177 | 
  178 |     test('TC-QQ-014-Verify a question can be copied and the duplicate is added to the page', async () => {
  179 |         await editPage.clickOnQuestionnaireTab();
  180 |         await questionsPage.clickAddNewPage();
  181 |         await questionsPage.dragAndDropQuestionnaire('Text');
  182 |         const initialCount = await questionsPage.getDroppedItemsCount();
  183 |         await questionsPage.copyQuestion('TEXT Question');
  184 |         await questionsPage.assertDroppedItemsCount(initialCount + 1);
  185 |     });
  186 | 
  187 |     test('TC-QQ-015-Verify a question can be deleted and is removed from the page', async () => {
  188 |         await editPage.clickOnQuestionnaireTab();
  189 |         await questionsPage.clickAddNewPage();
  190 |         await questionsPage.dragAndDropQuestionnaire('Text');
  191 |         await questionsPage.deleteQuestion('TEXT Question');
  192 |         await questionsPage.verifyQuestionDeleted('TEXT Question');
  193 |     });
  194 | 
  195 |     //DATA tab- Text Question
  196 |     test('TC-QQ-016-Verify all fields in TEXT question\'s Question tab are visible and editable', async () => {
  197 |         await editPage.clickOnQuestionnaireTab();
  198 |         await questionsPage.clickAddNewPage();
```