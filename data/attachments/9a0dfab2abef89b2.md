# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: E2E_Tests/FC020_questionnaire.spec.ts >> FC_020_Questionnaire Flow >> Configure questionnaire with 'Visible only for consultant' and verify 'Hide' action is executed when Question condition is triggered on 'Change a question' and check Questionnaire 'Import from' action
- Location: tests/E2E_Tests/FC020_questionnaire.spec.ts:31:9

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: locator('[data-test-mo-question-name="Email Question With Standard Answer"]')
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for locator('[data-test-mo-question-name="Email Question With Standard Answer"]')

```

# Page snapshot

```yaml
- generic [ref=e1]:
  - text: ×
  - link "ticket or feedback" [ref=e2] [cursor=pointer]:
    - /url: javascript:void(0)
    - img "ticket or feedback" [ref=e3]
  - generic [ref=e7]:
    - generic [ref=e8]:
      - generic [ref=e10]:
        - button "leftMenuOpen" [ref=e11] [cursor=pointer]:
          - img [ref=e12]
        - generic [ref=e13]:
          - img [ref=e17]
          - heading "QualiTlabs Hyd" [level=2] [ref=e21]
        - generic [ref=e25] [cursor=pointer]: search
        - button "Turn off admin role" [ref=e26] [cursor=pointer]:
          - img [ref=e27]:
            - img
        - button [ref=e29] [cursor=pointer]:
          - img [ref=e31]:
            - img [ref=e32]
        - generic [ref=e37]:
          - button [ref=e38] [cursor=pointer]:
            - img [ref=e40]:
              - img [ref=e41]
          - status "76" [ref=e42]
        - button "fullscreen" [ref=e43] [cursor=pointer]:
          - generic [ref=e44]: fullscreen
        - button "Open beamer" [ref=e45] [cursor=pointer]:
          - img [ref=e46]:
            - img
          - generic [ref=e47]: "1"
        - button "freshDesk" [ref=e48] [cursor=pointer]:
          - generic [ref=e49]: info
      - generic [ref=e50]:
        - generic [ref=e51]:
          - img [ref=e52] [cursor=pointer]
          - button "dehaze" [ref=e53] [cursor=pointer]:
            - generic [ref=e54]: dehaze
        - list [ref=e55]:
          - generic [ref=e56]:
            - button "profile pic" [ref=e57]
            - generic [ref=e58]: mahendra j
          - button "keyboard_arrow_down mahendra.juvvalapati@qualitlabs.com" [ref=e59] [cursor=pointer]:
            - generic [ref=e60]: keyboard_arrow_down
            - generic [ref=e61]: mahendra.juvvalapati@qualitlabs.com
          - list [ref=e62]:
            - button "account_box My Data" [ref=e63] [cursor=pointer]:
              - generic [ref=e64]: account_box
              - generic [ref=e65]: My Data
            - button "settings Settings" [ref=e66] [cursor=pointer]:
              - generic [ref=e67]: settings
              - generic [ref=e68]: Settings
            - button "exit_to_app Logout" [ref=e69] [cursor=pointer]:
              - generic [ref=e70]: exit_to_app
              - generic [ref=e71]: Logout
        - list [ref=e73]:
          - button "Add new user" [ref=e74] [cursor=pointer]:
            - img [ref=e75]:
              - img
            - generic [ref=e76]: Add new user
          - button "business Environments" [ref=e77] [cursor=pointer]:
            - generic [ref=e78]: business
            - generic [ref=e79]: Environments
          - button "home Dashboard" [ref=e80] [cursor=pointer]:
            - generic [ref=e81]: home
            - generic [ref=e82]: Dashboard
          - button "widgets Modules keyboard_arrow_down" [ref=e83] [cursor=pointer]:
            - generic [ref=e84]: widgets
            - generic [ref=e85]: Modules
            - generic [ref=e86]: keyboard_arrow_down
          - list [ref=e87]:
            - button "Strategy" [ref=e88] [cursor=pointer]:
              - img [ref=e89]:
                - img
              - generic [ref=e90]: Strategy
            - button "Policy" [ref=e91] [cursor=pointer]:
              - img [ref=e92]:
                - img
              - generic [ref=e93]: Policy
            - button "Programs" [ref=e94] [cursor=pointer]:
              - img [ref=e95]:
                - img
              - generic [ref=e96]: Programs
            - button "projects" [ref=e97] [cursor=pointer]:
              - img [ref=e98]:
                - img
              - generic [ref=e99]: projects
            - button "Dialogues" [ref=e100] [cursor=pointer]:
              - img [ref=e101]:
                - img
              - generic [ref=e102]: Dialogues
            - button "Objectives" [ref=e103] [cursor=pointer]:
              - img [ref=e104]:
                - img
              - generic [ref=e105]: Objectives
            - button "Processes" [ref=e106] [cursor=pointer]:
              - img [ref=e107]:
                - img
              - generic [ref=e108]: Processes
            - button "Organisation functions" [ref=e109] [cursor=pointer]:
              - img [ref=e110]:
                - img
              - generic [ref=e111]: Organisation functions
            - button "KSF's - Opportunities" [ref=e112] [cursor=pointer]:
              - img [ref=e113]:
                - img
              - generic [ref=e114]: KSF's - Opportunities
            - button "Stakeholders" [ref=e115] [cursor=pointer]:
              - img [ref=e116]:
                - img
              - generic [ref=e117]: Stakeholders
            - button "Risks" [ref=e118] [cursor=pointer]:
              - img [ref=e119]:
                - img
              - generic [ref=e120]: Risks
            - button "Opportunities" [ref=e121] [cursor=pointer]:
              - img [ref=e122]:
                - img
              - generic [ref=e123]: Opportunities
            - button "Standards Frameworks" [ref=e124] [cursor=pointer]:
              - img [ref=e125]:
                - img
              - generic [ref=e126]: Standards Frameworks
            - button "Laws and regulations" [ref=e127] [cursor=pointer]:
              - img [ref=e128]:
                - img
              - generic [ref=e129]: Laws and regulations
            - button "Measures" [ref=e130] [cursor=pointer]:
              - img [ref=e131]:
                - img
              - generic [ref=e132]: Measures
            - button "Assets" [ref=e133] [cursor=pointer]:
              - img [ref=e134]:
                - img
              - generic [ref=e135]: Assets
            - button "Information systems" [ref=e136] [cursor=pointer]:
              - img [ref=e137]:
                - img
              - generic [ref=e138]: Information systems
            - button "Processing" [ref=e139] [cursor=pointer]:
              - img [ref=e140]:
                - img
              - generic [ref=e141]: Processing
            - button "Audits" [ref=e142] [cursor=pointer]:
              - img [ref=e143]:
                - img
              - generic [ref=e144]: Audits
            - button "Audit sets" [ref=e145] [cursor=pointer]:
              - img [ref=e146]:
                - img
              - generic [ref=e147]: Audit sets
            - button "Impact Assessments" [ref=e148] [cursor=pointer]:
              - img [ref=e149]:
                - img
              - generic [ref=e150]: Impact Assessments
            - button "Tests" [ref=e151] [cursor=pointer]:
              - img [ref=e152]:
                - img
              - generic [ref=e153]: Tests
            - button "Findings" [ref=e154] [cursor=pointer]:
              - img [ref=e155]:
                - img
              - generic [ref=e156]: Findings
            - button "Problems" [ref=e157] [cursor=pointer]:
              - img [ref=e158]:
                - img
              - generic [ref=e159]: Problems
            - button "Changes" [ref=e160] [cursor=pointer]:
              - img [ref=e161]:
                - img
              - generic [ref=e162]: Changes
            - button "Cases" [ref=e163] [cursor=pointer]:
              - img [ref=e164]:
                - img
              - generic [ref=e165]: Cases
            - button "Tasks" [ref=e166] [cursor=pointer]:
              - img [ref=e167]:
                - img
              - generic [ref=e168]: Tasks
            - button "Documents" [ref=e169] [cursor=pointer]:
              - img [ref=e170]:
                - img
              - generic [ref=e171]: Documents
            - button "News items" [ref=e172] [cursor=pointer]:
              - img [ref=e173]:
                - img
              - generic [ref=e174]: News items
            - button "Related parties" [ref=e175] [cursor=pointer]:
              - img [ref=e176]:
                - img
              - generic [ref=e177]: Related parties
            - button "Contracts" [ref=e178] [cursor=pointer]:
              - img [ref=e179]:
                - img
              - generic [ref=e180]: Contracts
            - button "Vendors" [ref=e181] [cursor=pointer]:
              - img [ref=e182]:
                - img
              - generic [ref=e183]: Vendors
            - button "Performance agreements" [ref=e184] [cursor=pointer]:
              - img [ref=e185]:
                - img
              - generic [ref=e186]: Performance agreements
            - button "Key Figures" [ref=e187] [cursor=pointer]:
              - img [ref=e188]:
                - img
              - generic [ref=e189]: Key Figures
            - button "Settings" [ref=e190] [cursor=pointer]:
              - img [ref=e191]:
                - img
              - generic [ref=e192]: Settings
            - button "Critical Business Scenarios" [ref=e193] [cursor=pointer]:
              - img [ref=e194]:
                - img
              - generic [ref=e195]: Critical Business Scenarios
            - button "BCM Plans" [ref=e196] [cursor=pointer]:
              - img [ref=e197]:
                - img
              - generic [ref=e198]: BCM Plans
            - button "Context analysis" [ref=e199] [cursor=pointer]:
              - img [ref=e200]:
                - img
              - generic [ref=e201]: Context analysis
            - button "Situations" [ref=e202] [cursor=pointer]:
              - img [ref=e203]:
                - img
              - generic [ref=e204]: Situations
    - generic [ref=e210]:
      - generic [ref=e212]:
        - generic [ref=e213]:
          - generic [ref=e215]:
            - generic [ref=e216] [cursor=pointer]:
              - generic: apps
              - generic:
                - img
            - list [ref=e217]:
              - listitem [ref=e218]:
                - generic [ref=e220]:
                  - generic:
                    - img
                  - generic [ref=e221]: Risk
          - 'button "version:No repeatplan - 1 Version name keyboard_arrow_down Executor: ALL" [ref=e224] [cursor=pointer]':
            - generic [ref=e225]: version:No repeatplan - 1 Version name
            - generic [ref=e226]: keyboard_arrow_down
            - generic [ref=e227]: "Executor: ALL"
          - button "settings" [ref=e229] [cursor=pointer]:
            - img [ref=e230]: settings
          - generic [ref=e231]:
            - button "add mo to projects" [ref=e233] [cursor=pointer]:
              - img [ref=e234]:
                - img
            - button [ref=e235] [cursor=pointer]:
              - img [ref=e237]:
                - img [ref=e238]
        - text: ▼ ▼
      - generic [ref=e239]:
        - generic [ref=e241]:
          - img [ref=e243]:
            - img
          - generic [ref=e244]:
            - generic [ref=e246]: "Risk: Risk_1778783044594"
            - button "Copy item" [ref=e248] [cursor=pointer]:
              - img "copy item" [ref=e249]: file_copy
            - button "Close current version and start new version" [ref=e250] [cursor=pointer]:
              - img "quick-version" [ref=e251]:
                - img
            - generic [ref=e252]:
              - button "previous item" [disabled] [ref=e253]:
                - img "previous item" [ref=e254]:
                  - img
              - button "previous item" [disabled] [ref=e255]:
                - img "previous item" [ref=e256]:
                  - img
        - generic [ref=e257]:
          - img:
            - img
          - generic [ref=e258]:
            - generic [ref=e259]:
              - button "Previous Page" [disabled] [ref=e261]:
                - img [ref=e262]:
                  - img
              - button "Next Page" [ref=e263] [cursor=pointer]:
                - img [ref=e264]:
                  - img
              - generic [ref=e265]:
                - tablist "Use the left and right arrow keys to navigate between tabs" [ref=e266]:
                  - tab "Gross risk" [ref=e267] [cursor=pointer]:
                    - generic [ref=e269]: Gross risk
                  - tab "Net risk" [ref=e270] [cursor=pointer]:
                    - generic [ref=e272]: Net risk
                  - tab "Bowtie" [ref=e273] [cursor=pointer]:
                    - generic [ref=e275]: Bowtie
                  - tab "Measures" [ref=e276] [cursor=pointer]:
                    - generic [ref=e278]: Measures
                  - tab "Kritieke Bedrijfsfuncties" [ref=e279] [cursor=pointer]:
                    - generic [ref=e281]: Kritieke Bedrijfsfuncties
                  - tab "Dialogue" [selected] [ref=e282]:
                    - generic [ref=e284]: Dialogue
                  - tab "Chat" [ref=e285] [cursor=pointer]:
                    - generic [ref=e287]: Chat
                  - tab "Information systems" [ref=e288] [cursor=pointer]:
                    - generic [ref=e290]: Information systems
                  - tab "Related" [ref=e291] [cursor=pointer]:
                    - generic [ref=e293]: Related
                  - tab "Tasks" [ref=e294] [cursor=pointer]:
                    - generic [ref=e296]: Tasks
                  - tab "Key Indicators" [ref=e297] [cursor=pointer]:
                    - generic [ref=e299]: Key Indicators
                  - tab "History" [ref=e300] [cursor=pointer]:
                    - generic [ref=e302]: History
                  - tab "mo data" [ref=e303] [cursor=pointer]:
                    - generic [ref=e305]: mo data
                  - tab "Documents" [ref=e306] [cursor=pointer]:
                    - generic [ref=e308]: Documents
                  - tab "Risks" [ref=e309] [cursor=pointer]:
                    - generic [ref=e311]: Risks
                - generic [ref=e313]:
                  - generic [ref=e316] [cursor=pointer]: Gross risk
                  - generic [ref=e319] [cursor=pointer]: Net risk
                  - generic [ref=e322] [cursor=pointer]: Bowtie
                  - generic [ref=e325] [cursor=pointer]: Measures
                  - generic [ref=e328] [cursor=pointer]: Kritieke Bedrijfsfuncties
                  - generic [ref=e331] [cursor=pointer]: Dialogue
                  - generic [ref=e334] [cursor=pointer]: Chat
                  - generic [ref=e337] [cursor=pointer]: Information systems
                  - generic [ref=e340] [cursor=pointer]: Related
                  - generic [ref=e343] [cursor=pointer]: Tasks
                  - generic [ref=e346] [cursor=pointer]: Key Indicators
                  - generic [ref=e349] [cursor=pointer]: History
                  - generic [ref=e352] [cursor=pointer]: mo data
                  - generic [ref=e355] [cursor=pointer]: Documents
                  - generic [ref=e358] [cursor=pointer]: Risks
            - tabpanel "Dialogue" [ref=e360]:
              - button "executer Questionnaire_1778783044594 Card image %" [ref=e370] [cursor=pointer]:
                - generic [ref=e371]:
                  - img "executer" [ref=e373]
                  - generic "Questionnaire_1778783044594" [ref=e374]:
                    - generic [ref=e375]: Questionnaire_1778783044594
                - img "Card image" [ref=e377]
                - generic [ref=e379]:
                  - generic [ref=e380]:
                    - generic: "%"
                  - button [ref=e382]:
                    - img
  - iframe [ref=e384]:
    - generic [active]:
      - generic:
        - text:  
        - button "Open chat" [ref=f6e1] [cursor=pointer]
  - generic:
    - dialog:
      - generic [ref=e392]:
        - banner [ref=e393]:
          - generic [ref=e395]:
            - listitem [ref=e396]:
              - generic [ref=e398]: Questionnaire_1778783044594
              - generic [ref=e399]:
                - button [ref=e401] [cursor=pointer]:
                  - img [ref=e403]:
                    - img [ref=e404]
                - button [ref=e406] [cursor=pointer]:
                  - img [ref=e408]: mail
                - button [ref=e410] [cursor=pointer]:
                  - img [ref=e412]: close
            - listitem [ref=e413]:
              - generic [ref=e415]: "|"
              - generic [ref=e417]: input
              - generic [ref=e422] [cursor=pointer]:
                - generic [ref=e423]:
                  - generic [ref=e424]:
                    - generic [ref=e425]: (1-2) Page name 1
                    - combobox "(1-2) Page name 1 Go to page" [ref=e426]: Page name 1
                  - generic:
                    - generic: Go to page
                - generic [ref=e428]: arrow_drop_down
              - button [ref=e430] [cursor=pointer]:
                - img [ref=e432]: keyboard_arrow_right
        - main [ref=e434]:
          - generic [ref=e437]:
            - generic [ref=e438]:
              - generic [ref=e440]: "Risk : Risk_1778783044594"
              - generic [ref=e442]: Page name 1
            - listitem [ref=e448]:
              - generic [ref=e452]:
                - generic [ref=e456]: Email Question With Mandatory and In herit answer *
                - combobox [ref=e463] [cursor=pointer]
                - generic [ref=e464] [cursor=pointer]: keyboard_arrow_down
        - contentinfo [ref=e465]:
          - generic [ref=e468]:
            - button "Next" [ref=e469] [cursor=pointer]:
              - generic [ref=e470]:
                - generic [ref=e471]: Next
                - img [ref=e472]: keyboard_arrow_right
            - button "Complete & Next" [ref=e473] [cursor=pointer]:
              - generic [ref=e474]:
                - generic [ref=e475]: Complete & Next
                - img [ref=e476]: keyboard_arrow_right
        - complementary [ref=e477]
```

# Test source

```ts
  66  |             await questionsPage.configureQuestion(questions.Email1);
  67  |             await questionsPage.configureQuestion(questions.Email2);
  68  |             await questionsPage.clickAddNewPage();
  69  |             await questionsPage.configureQuestion(questions.Email3);
  70  |             await questionsPage.configureQuestion(questions.Text1);
  71  | 
  72  |         });
  73  | 
  74  |         await test.step('Configure question conditions', async () => {
  75  |             await editPage.clickOnQuestionConditionsTab();
  76  |             await questionConditionsPage.createNewConditionTabWithData(questionConditions.tabs.tab1);
  77  |             await questionConditionsPage.addConditionToTabWithData(questionConditions.conditions.condition1);
  78  |             await questionConditionsPage.configureTriggerOn(questionConditions.triggerOn.changeQuestion);
  79  |             await questionConditionsPage.createConditionRules(questionConditions.conditionOn);
  80  |             await questionConditionsPage.createActionRules(questionConditions.actionType);
  81  |         });
  82  | 
  83  |         await test.step('Configure questionnaire conditions', async () => {
  84  |             await editPage.clickOnQuestionnaireConditionsTab();
  85  |             await questionnaireConditionsPage.createNewConditionTabWithData(questionnaireConditions.tabs.tab1);
  86  |             await questionnaireConditionsPage.addConditionToTabWithData(questionnaireConditions.conditions.condition1);
  87  |             await questionnaireConditionsPage.createConditionRules(questionnaireConditions.conditionOn);
  88  |             await questionnaireConditionsPage.createActionRules(questionnaireConditions.actionType);
  89  |         });
  90  | 
  91  |         await test.step('Configure indicators', async () => {
  92  |             await editPage.clickOnIndicatorsTab();
  93  |             await indicatorsPage.configureIndicators(indicators);
  94  |         });
  95  | 
  96  |         await test.step('Publish questionnaire', async () => {
  97  |             await editPage.clickOnPublishOrEdit();
  98  |             await editPage.verifyQuestionnaireIsPublished();
  99  |         });
  100 | 
  101 |         await test.step('Navigate to risk management', async () => {
  102 |             await leftNav.clickOnDashboard();
  103 |             await leftNav.hoverOnNotifications();
  104 |             await navigationHelper.navigateToCompanyDashboard('Qualitlabs');
  105 |             await environmentsPage.clickOnEnvironment("QualiTlabs Hyd");
  106 |             await leftNav.clickOnModules();
  107 |             await leftNav.clickOnRisksModule();
  108 |         });
  109 | 
  110 |         await test.step('Verify visible only for consultant setting is applied', async () => {
  111 |             await risksPage.clickOnAddNewRiskBtn();
  112 |             fc020Data.risk.name = uniqueRiskName;
  113 |             await risksPage.createNewRiskWithData(fc020Data.risk);
  114 |             await risksPage.clickDialogueTab();
  115 |             await risksPage.clickOnSettingsIcon();
  116 |             await risksPage.clickOnAddBtnToLinkQuestionnaire();
  117 |             await risksPage.selectKnowledgeDatabaseOption('QA Automation');
  118 |             await risksPage.searchQuestionnaire(uniqueName);
  119 |             await page.waitForTimeout(4000);
  120 |             await expect(page
  121 |                 .getByText(`${uniqueName} Link`)
  122 |                 .getByRole('checkbox', { name: 'ql._id' })).not.toBeVisible();  //visible only for consultant
  123 |             await risksPage.clickCloseDialogButton();
  124 |         });
  125 | 
  126 |         await test.step('Uncheck visible only for consultant setting and re-publish questionnaire', async () => {
  127 |             await leftNav.clickOnEnvironments();
  128 |             await leftNav.clickOnKnowledgeDatabase();
  129 |             await kdPage.clickOnCompanyName('QA Automation');
  130 |             await leftNav.clickOnMaintain();
  131 |             await leftNav.clickOnQuestionnairesAndForms();
  132 |             await kdPage.clickOnNoThanksPopup();
  133 |             await questionnairePage.searchQuestionnaire(uniqueName);
  134 |             await questionnairePage.clickOnSearchResult();
  135 |             await editPage.clickEditButton();
  136 |             await settingsPage.unCheckVisibleForConsultant();
  137 |             await editPage.clickOnPublishOrEdit();
  138 |         })
  139 | 
  140 |         await test.step('Navigate to risk and link questionnaire', async () => {
  141 |             await leftNav.clickOnDashboard();
  142 |             await leftNav.hoverOnNotifications();
  143 |             await navigationHelper.navigateToCompanyDashboard('Qualitlabs');
  144 |             await environmentsPage.clickOnEnvironment("QualiTlabs Hyd");
  145 |             await leftNav.clickOnModules();
  146 |             await leftNav.clickOnRisksModule();
  147 |         });
  148 | 
  149 |         await test.step('Search risk and link questionnaire', async () => {
  150 |             await risksPage.searchRisk(uniqueRiskName);
  151 |             await risksPage.openRiskByName(uniqueRiskName);
  152 |             await risksPage.clickDialogueTab();
  153 |             await risksPage.linkQuestionnaireToRisk(uniqueName, 'QA Automation');
  154 |             await risksPage.verifyAddedQuestionnaireLinked(uniqueName);
  155 |         });
  156 | 
  157 |         const question1Locator = page.locator(`[data-test-mo-question-name="${questions.Email1.Question.questionName}"]`);
  158 |         const question2Locator = page.locator(`[data-test-mo-question-name="${questions.Email2.Question.questionName}"]`);
  159 |         const question3Locator = page.locator(`[data-test-mo-question-name="${questions.Email3.Question.questionName}"]`);
  160 |         const question4Locator = page.locator(`[data-test-mo-question-name="${questions.Text1.Question.questionName}"]`);
  161 | 
  162 |         await test.step('Open questionnaire and verify all questions visible', async () => {
  163 |             await risksPage.clickDialogueTab();
  164 |             await risksPage.clickOnQuestionnaire(uniqueName);
  165 | 
> 166 |             await expect(question1Locator).toBeVisible();
      |                                            ^ Error: expect(locator).toBeVisible() failed
  167 |             await expect(question2Locator).toBeVisible();
  168 |         });
  169 | 
  170 |         await test.step('Verify next button is enabled', async () => {
  171 |             await risksPage.verifyNextButtonIsEnabled();
  172 |         });
  173 | 
  174 |         await test.step('Verify Standard answer is set', async () => {
  175 |             await expect(question1Locator.locator('span.ellipsis')).toContainText(questions.Email1.Question.standardAnswer);
  176 |         });
  177 | 
  178 |         await test.step('Verify explanation icon is visible', async () => {
  179 |             await risksPage.verifyExplanationOfQuestion(question1Locator, questions.Email1.explanationText);
  180 |         });
  181 | 
  182 |         await test.step('Verify mandatory field state', async () => {
  183 |             await risksPage.clickCompleteAndNextButton();
  184 |             await risksPage.verifyMandatoryFieldsErrorMessageDisplayed();
  185 |             await risksPage.clickCloseDialogButton();
  186 |             await expect(question2Locator.getByText('This field is required!')).toBeVisible();
  187 |             await question2Locator.locator('input').first().fill('qualitlabs@example.com');
  188 |             await question2Locator.locator('input').first().blur();
  189 |         });
  190 | 
  191 |         await test.step('Verify Readonly field state', async () => {
  192 |             await risksPage.clickCompleteAndNextButton();
  193 |             await expect(question3Locator).toBeVisible();
  194 |             await expect(question4Locator).toBeVisible();
  195 |             await expect(question3Locator.locator('input')).toBeDisabled();
  196 |         });
  197 | 
  198 |         await test.step('verify hide action executed when question condition is met', async () => {
  199 |             await question4Locator.getByRole('textbox').fill('mahendra');
  200 |             await page.waitForTimeout(1000);
  201 |             await risksPage.clickOnRiskHeading(uniqueRiskName);
  202 |             await expect(question3Locator).not.toBeVisible();
  203 |         });
  204 | 
  205 |         await test.step('Finish questionnaire', async () => {
  206 |             await risksPage.clickCompleteButton();
  207 |             await risksPage.verifyFinishMessageDisplayed();
  208 |             await risksPage.clickYesButton();
  209 |             await risksPage.verifyQuestionnaireIsFinished(uniqueName);
  210 |         });
  211 | 
  212 |         await test.step('verify import from action executed when questionnaire condition is met', async () => {
  213 |             await risksPage.clickOnRelatedTab();
  214 |             await risksPage.verifyRelatedTabHasRisk(questionnaireConditions.actionType[0]);
  215 |         });
  216 | 
  217 |         await test.step('Verify Indicators added Succesfully', async () => {
  218 |             await risksPage.clickKeyIndicatorTab();
  219 |             await risksPage.verifyIndicatorIsNotDisplayedInIndicatorTab(indicators[0].name);
  220 | 
  221 |             await risksPage.clickGrossRiskTab();
  222 |             await risksPage.verifyIndicatorIsNotDisplayedInGrossRiskTab(indicators[0].name);
  223 |         });
  224 | 
  225 |         await test.step.skip('Verify Inherit answer from previous Version', async () => {
  226 |             await risksPage.clickDialogueTab();
  227 |             await risksPage.createNewVersion();
  228 |             await risksPage.clickOnQuestionnaire(uniqueName);
  229 |             await expect(question1Locator.locator('input').first()).toHaveValue('mahendra');
  230 |         })
  231 | 
  232 |     });
  233 | });
```