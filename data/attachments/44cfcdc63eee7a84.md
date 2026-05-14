# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: E2E_Tests/FC010_questionnaire.spec.ts >> FC_010_Questionnaire Flow >> Configure questionnaire with 'Questionnaire email text for invitation' and verify 'Set quality state to' action is executed when Question condition is triggered on 'Entering the questionnaire the first time' and check Questionnaire 'Set version state to closed' action
- Location: tests/E2E_Tests/FC010_questionnaire.spec.ts:31:9

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByText('Questionnaire_1778752123418 Link').getByRole('checkbox', { name: 'ql._id' })
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for getByText('Questionnaire_1778752123418 Link').getByRole('checkbox', { name: 'ql._id' })

```

# Page snapshot

```yaml
- generic [ref=e1]:
  - text: ×
  - link [ref=e3] [cursor=pointer]:
    - /url: javascript:void(0)
    - img [ref=e4]
  - generic [ref=e8]:
    - generic [ref=e9]:
      - generic [ref=e11]:
        - button [ref=e12] [cursor=pointer]:
          - img [ref=e13]
        - generic [ref=e14]:
          - img [ref=e18]
          - heading [level=2] [ref=e22]: QualiTlabs Hyd
        - generic [ref=e26] [cursor=pointer]: search
        - button [ref=e27] [cursor=pointer]:
          - img [ref=e28]:
            - img
        - button [ref=e30] [cursor=pointer]:
          - img [ref=e32]:
            - img [ref=e33]
        - generic [ref=e38]:
          - button [ref=e39] [cursor=pointer]:
            - img [ref=e41]:
              - img [ref=e42]
          - status [ref=e43]: "82"
        - button [ref=e44] [cursor=pointer]:
          - generic [ref=e45]: fullscreen
        - button [ref=e46] [cursor=pointer]:
          - img [ref=e47]:
            - img
          - generic [ref=e48]: "1"
        - button [ref=e49] [cursor=pointer]:
          - generic [ref=e50]: info
      - generic [ref=e51]:
        - generic [ref=e52]:
          - img [ref=e53] [cursor=pointer]
          - button [ref=e54] [cursor=pointer]:
            - generic [ref=e55]: dehaze
        - list [ref=e56]:
          - generic [ref=e57]:
            - button [ref=e58]
            - generic [ref=e59]: mahendra j
          - button [ref=e60] [cursor=pointer]:
            - generic [ref=e61]: keyboard_arrow_down
            - generic [ref=e62]: mahendra.juvvalapati@qualitlabs.com
          - list [ref=e63]:
            - button [ref=e64] [cursor=pointer]:
              - generic [ref=e65]: account_box
              - generic [ref=e66]: My Data
            - button [ref=e67] [cursor=pointer]:
              - generic [ref=e68]: settings
              - generic [ref=e69]: Settings
            - button [ref=e70] [cursor=pointer]:
              - generic [ref=e71]: exit_to_app
              - generic [ref=e72]: Logout
        - list [ref=e74]:
          - button [ref=e75] [cursor=pointer]:
            - img [ref=e76]:
              - img
            - generic [ref=e77]: Add new user
          - button [ref=e78] [cursor=pointer]:
            - generic [ref=e79]: business
            - generic [ref=e80]: Environments
          - button [ref=e81] [cursor=pointer]:
            - generic [ref=e82]: home
            - generic [ref=e83]: Dashboard
          - button [ref=e84] [cursor=pointer]:
            - generic [ref=e85]: widgets
            - generic [ref=e86]: Modules
            - generic [ref=e87]: keyboard_arrow_down
          - list [ref=e88]:
            - button [ref=e89] [cursor=pointer]:
              - img [ref=e90]:
                - img
              - generic [ref=e91]: Strategy
            - button [ref=e92] [cursor=pointer]:
              - img [ref=e93]:
                - img
              - generic [ref=e94]: Policy
            - button [ref=e95] [cursor=pointer]:
              - img [ref=e96]:
                - img
              - generic [ref=e97]: Programs
            - button [ref=e98] [cursor=pointer]:
              - img [ref=e99]:
                - img
              - generic [ref=e100]: projects
            - button [ref=e101] [cursor=pointer]:
              - img [ref=e102]:
                - img
              - generic [ref=e103]: Dialogues
            - button [ref=e104] [cursor=pointer]:
              - img [ref=e105]:
                - img
              - generic [ref=e106]: Objectives
            - button [ref=e107] [cursor=pointer]:
              - img [ref=e108]:
                - img
              - generic [ref=e109]: Processes
            - button [ref=e110] [cursor=pointer]:
              - img [ref=e111]:
                - img
              - generic [ref=e112]: Organisation functions
            - button [ref=e113] [cursor=pointer]:
              - img [ref=e114]:
                - img
              - generic [ref=e115]: KSF's - Opportunities
            - button [ref=e116] [cursor=pointer]:
              - img [ref=e117]:
                - img
              - generic [ref=e118]: Stakeholders
            - button [ref=e119] [cursor=pointer]:
              - img [ref=e120]:
                - img
              - generic [ref=e121]: Risks
            - button [ref=e122] [cursor=pointer]:
              - img [ref=e123]:
                - img
              - generic [ref=e124]: Opportunities
            - button [ref=e125] [cursor=pointer]:
              - img [ref=e126]:
                - img
              - generic [ref=e127]: Standards Frameworks
            - button [ref=e128] [cursor=pointer]:
              - img [ref=e129]:
                - img
              - generic [ref=e130]: Laws and regulations
            - button [ref=e131] [cursor=pointer]:
              - img [ref=e132]:
                - img
              - generic [ref=e133]: Measures
            - button [ref=e134] [cursor=pointer]:
              - img [ref=e135]:
                - img
              - generic [ref=e136]: Assets
            - button [ref=e137] [cursor=pointer]:
              - img [ref=e138]:
                - img
              - generic [ref=e139]: Information systems
            - button [ref=e140] [cursor=pointer]:
              - img [ref=e141]:
                - img
              - generic [ref=e142]: Processing
            - button [ref=e143] [cursor=pointer]:
              - img [ref=e144]:
                - img
              - generic [ref=e145]: Audits
            - button [ref=e146] [cursor=pointer]:
              - img [ref=e147]:
                - img
              - generic [ref=e148]: Audit sets
            - button [ref=e149] [cursor=pointer]:
              - img [ref=e150]:
                - img
              - generic [ref=e151]: Impact Assessments
            - button [ref=e152] [cursor=pointer]:
              - img [ref=e153]:
                - img
              - generic [ref=e154]: Tests
            - button [ref=e155] [cursor=pointer]:
              - img [ref=e156]:
                - img
              - generic [ref=e157]: Findings
            - button [ref=e158] [cursor=pointer]:
              - img [ref=e159]:
                - img
              - generic [ref=e160]: Problems
            - button [ref=e161] [cursor=pointer]:
              - img [ref=e162]:
                - img
              - generic [ref=e163]: Changes
            - button [ref=e164] [cursor=pointer]:
              - img [ref=e165]:
                - img
              - generic [ref=e166]: Cases
            - button [ref=e167] [cursor=pointer]:
              - img [ref=e168]:
                - img
              - generic [ref=e169]: Tasks
            - button [ref=e170] [cursor=pointer]:
              - img [ref=e171]:
                - img
              - generic [ref=e172]: Documents
            - button [ref=e173] [cursor=pointer]:
              - img [ref=e174]:
                - img
              - generic [ref=e175]: News items
            - button [ref=e176] [cursor=pointer]:
              - img [ref=e177]:
                - img
              - generic [ref=e178]: Related parties
            - button [ref=e179] [cursor=pointer]:
              - img [ref=e180]:
                - img
              - generic [ref=e181]: Contracts
            - button [ref=e182] [cursor=pointer]:
              - img [ref=e183]:
                - img
              - generic [ref=e184]: Vendors
            - button [ref=e185] [cursor=pointer]:
              - img [ref=e186]:
                - img
              - generic [ref=e187]: Performance agreements
            - button [ref=e188] [cursor=pointer]:
              - img [ref=e189]:
                - img
              - generic [ref=e190]: Key Figures
            - button [ref=e191] [cursor=pointer]:
              - img [ref=e192]:
                - img
              - generic [ref=e193]: Settings
            - button [ref=e194] [cursor=pointer]:
              - img [ref=e195]:
                - img
              - generic [ref=e196]: Critical Business Scenarios
            - button [ref=e197] [cursor=pointer]:
              - img [ref=e198]:
                - img
              - generic [ref=e199]: BCM Plans
            - button [ref=e200] [cursor=pointer]:
              - img [ref=e201]:
                - img
              - generic [ref=e202]: Context analysis
            - button [ref=e203] [cursor=pointer]:
              - img [ref=e204]:
                - img
              - generic [ref=e205]: Situations
    - generic [ref=e211]:
      - generic [ref=e213]:
        - generic [ref=e214]:
          - button [ref=e217] [cursor=pointer]:
            - generic [ref=e218]: version:No repeatplan - 1 Version name
            - generic [ref=e219]: keyboard_arrow_down
          - generic [ref=e220]:
            - button [ref=e221] [cursor=pointer]:
              - img [ref=e222]:
                - generic [ref=e223]: featured_play_list
            - button [ref=e224] [cursor=pointer]:
              - img [ref=e225]:
                - generic [ref=e226]: clear
          - generic [ref=e227]:
            - button [ref=e229] [cursor=pointer]:
              - img [ref=e230]:
                - img
            - button [ref=e231] [cursor=pointer]:
              - img [ref=e233]:
                - img [ref=e234]
        - text: ▼
      - generic [ref=e235]:
        - generic [ref=e237]:
          - img [ref=e239]
          - generic [ref=e240]:
            - generic [ref=e242]: "Risk: Risk_1778752123418"
            - button [ref=e244] [cursor=pointer]:
              - img [ref=e245]: file_copy
            - button [ref=e246] [cursor=pointer]:
              - img [ref=e247]:
                - img
            - generic [ref=e248]:
              - button [disabled] [ref=e249]:
                - img [ref=e250]:
                  - img
              - button [disabled] [ref=e251]:
                - img [ref=e252]:
                  - img
        - generic [ref=e253]:
          - img
          - generic [ref=e254]:
            - generic [ref=e255]:
              - button [disabled] [ref=e257]:
                - img [ref=e258]:
                  - img
              - button [ref=e259] [cursor=pointer]:
                - img [ref=e260]:
                  - img
              - generic [ref=e261]:
                - tablist [ref=e262]:
                  - tab [ref=e263] [cursor=pointer]:
                    - generic [ref=e265]: Gross risk
                  - tab [ref=e266] [cursor=pointer]:
                    - generic [ref=e268]: Net risk
                  - tab [ref=e269] [cursor=pointer]:
                    - generic [ref=e271]: Bowtie
                  - tab [ref=e272] [cursor=pointer]:
                    - generic [ref=e274]: Measures
                  - tab [ref=e275] [cursor=pointer]:
                    - generic [ref=e277]: Kritieke Bedrijfsfuncties
                  - tab [selected] [ref=e278]:
                    - generic [ref=e280]: Dialogue
                  - tab [ref=e281] [cursor=pointer]:
                    - generic [ref=e283]: Chat
                  - tab [ref=e284] [cursor=pointer]:
                    - generic [ref=e286]: Information systems
                  - tab [ref=e287] [cursor=pointer]:
                    - generic [ref=e289]: Related
                  - tab [ref=e290] [cursor=pointer]:
                    - generic [ref=e292]: Tasks
                  - tab [ref=e293] [cursor=pointer]:
                    - generic [ref=e295]: Key Indicators
                  - tab [ref=e296] [cursor=pointer]:
                    - generic [ref=e298]: History
                  - tab [ref=e299] [cursor=pointer]:
                    - generic [ref=e301]: mo data
                  - tab [ref=e302] [cursor=pointer]:
                    - generic [ref=e304]: Documents
                  - tab [ref=e305] [cursor=pointer]:
                    - generic [ref=e307]: Risks
                - generic [ref=e309]:
                  - generic [ref=e312] [cursor=pointer]: Gross risk
                  - generic [ref=e315] [cursor=pointer]: Net risk
                  - generic [ref=e318] [cursor=pointer]: Bowtie
                  - generic [ref=e321] [cursor=pointer]: Measures
                  - generic [ref=e324] [cursor=pointer]: Kritieke Bedrijfsfuncties
                  - generic [ref=e327] [cursor=pointer]: Dialogue
                  - generic [ref=e330] [cursor=pointer]: Chat
                  - generic [ref=e333] [cursor=pointer]: Information systems
                  - generic [ref=e336] [cursor=pointer]: Related
                  - generic [ref=e339] [cursor=pointer]: Tasks
                  - generic [ref=e342] [cursor=pointer]: Key Indicators
                  - generic [ref=e345] [cursor=pointer]: History
                  - generic [ref=e348] [cursor=pointer]: mo data
                  - generic [ref=e351] [cursor=pointer]: Documents
                  - generic [ref=e354] [cursor=pointer]: Risks
            - tabpanel [ref=e356]
      - button [ref=e364] [cursor=pointer]:
        - generic [ref=e365]: add
  - iframe [ref=e367]:
    - generic [active]:
      - generic:
        - text:  
        - button "Open chat" [ref=f4e1] [cursor=pointer]
  - dialog "wef" [active] [ref=e370]:
    - generic [ref=e371]:
      - generic [ref=e372]:
        - heading "Link questionnaires" [level=2] [ref=e373]
        - button "Close dialog" [ref=e374] [cursor=pointer]:
          - img "Close dialog" [ref=e375]:
            - img
      - generic [ref=e377]:
        - generic: Knowledge Database
        - button "select country QA Automation" [ref=e378]:
          - generic [ref=e379]:
            - generic [ref=e380]: QA Automation
            - generic [ref=e381]: ▼
      - generic [ref=e382]:
        - textbox "Enter search" [ref=e385]: Questionnaire_1778752123418
        - generic [ref=e387]: search
    - progressbar [ref=e388]
    - generic [ref=e394]:
      - button "Cancel" [ref=e395] [cursor=pointer]
      - button "OK" [disabled] [ref=e396]
```

# Test source

```ts
  88  | 
  89  |     this.searchInput = page.locator('div[isfilteractive="false"] [placeholder="Type to Search"]');
  90  | 
  91  |     this.variableIcon = page.getByRole('button', { name: 'variables' });
  92  |     this.moQualityState = page.getByTestId('MoQualityState');
  93  |     this.moQualityStateDropdown = page.getByTestId('MoQualityStateDropdown');
  94  |     this.moQualityState = page.locator('select[name="MoQualityState"]');
  95  |     this.prevButton = page.locator('[aria-label="Previous Page"]');
  96  |   }
  97  | 
  98  |   async createNewRisk(name: string, description: string, status: string) {
  99  |     await this.selectNewItemOption();
  100 |     await this.setMoState(status);
  101 |     await this.fillRiskName(name);
  102 |     await this.fillRiskDescription(description);
  103 |     await this.saveRisk();
  104 |     await expect(this.page.locator('span').filter({ hasText: 'Risk:' }).last()).toBeVisible();
  105 |   }
  106 | 
  107 |   async createNewRiskWithData(data: any) {
  108 |     await this.createNewRisk(data.name, data.description, data.status);
  109 |   }
  110 | 
  111 |   private async selectNewItemOption() {
  112 |     await this.actions.click(this.newItemButton);
  113 |   }
  114 | 
  115 |   private async setMoState(state: string) {
  116 |     await this.actions.click(this.moStatesDropdown);
  117 | 
  118 |     const option = this.page.getByRole('option', { name: state });
  119 |     await this.actions.click(option);
  120 |   }
  121 | 
  122 |   private async fillRiskName(name: string) {
  123 |     await this.actions.click(this.nameInput);
  124 |     await this.actions.type(this.nameInput, name);
  125 |   }
  126 | 
  127 |   private async fillRiskDescription(description: string) {
  128 |     await this.actions.click(this.descriptionInput);
  129 |     await this.actions.type(this.descriptionInput, description);
  130 |   }
  131 | 
  132 |   private async saveRisk() {
  133 |     await this.actions.click(this.saveButton);
  134 |   }
  135 | 
  136 |   async clickDialogueTab() {
  137 |     await this.page.waitForTimeout(2000);
  138 |     await this.actions.click(this.dialogueTab);
  139 |   }
  140 | 
  141 |   async clickHistoryTab() {
  142 |     await this.actions.click(this.historyTab);
  143 |     // await this.page.waitForLoadState('networkidle');
  144 |   }
  145 | 
  146 |   async clickOnAddNewRiskBtn() {
  147 |     await this.page.waitForTimeout(1500);
  148 |     try {
  149 |       await this.actions.verifyVisible(this.risksHeading);
  150 |       await this.actions.click(this.addNewRiskButton);
  151 |       await expect(this.newItemButton).toBeVisible({ timeout: 15000 });
  152 |     } catch (error) {
  153 |       // console.error('Error occurred while clicking on Add New Risk button:', error);
  154 |       await this.actions.click(this.addNewRiskButton);
  155 | 
  156 |     }
  157 |   }
  158 | 
  159 |   async clickOnSettingsIcon() {
  160 |     await this.actions.click(this.settingsIcon);
  161 |   }
  162 | 
  163 |   async clickOnAddBtnToLinkQuestionnaire() {
  164 |     await this.actions.click(this.addBtnToLinkQuestionnaire);
  165 |   }
  166 | 
  167 |   async clickOnKnowledgeDatabaseDropdown() {
  168 |     await this.actions.click(this.knowledgeDataBaseDropdown);
  169 |   }
  170 | 
  171 |   async selectKnowledgeDatabaseOption(option: string) {
  172 |     await this.actions.click(this.knowledgeDataBaseDropdown);
  173 | 
  174 |     const dropdownOption = this.page.getByRole('option', { name: option });
  175 |     await this.actions.click(dropdownOption);
  176 |   }
  177 | 
  178 |   async searchQuestionnaire(questionnaireName: string) {
  179 |     await this.actions.type(this.searchQuestionnaireInput, questionnaireName);
  180 |   }
  181 | 
  182 |   async linkQuestionnaire(questionnaireName: string) {
  183 |     await this.searchQuestionnaire(questionnaireName);
  184 |     const checkbox = this.page
  185 |       .getByText(`${questionnaireName} Link`)
  186 |       .getByRole('checkbox', { name: 'ql._id' });
  187 |     await this.page.locator('.MOQPopupHeight > .layout-wrap').click();
> 188 |     await expect(checkbox).toBeVisible({ timeout: 15000 });
      |                            ^ Error: expect(locator).toBeVisible() failed
  189 |     await this.actions.waitForVisible(checkbox);
  190 |     await this.actions.check(checkbox);
  191 |   }
  192 | 
  193 |   async clickOkButton() {
  194 |     await this.actions.click(this.okBtn);
  195 |   }
  196 | 
  197 |   async linkQuestionnaireToRisk(questionnaireName: string, knowledgeDatabaseOption: string) {
  198 |     await this.clickOnSettingsIcon();
  199 |     await this.clickOnAddBtnToLinkQuestionnaire();
  200 |     await this.selectKnowledgeDatabaseOption(knowledgeDatabaseOption);
  201 |     await this.page.waitForTimeout(3000);
  202 |     await this.linkQuestionnaire(questionnaireName);
  203 |     await expect(this.okBtn).toBeEnabled({ timeout: 10000 });
  204 |     await this.clickOkButton();
  205 |     await this.turnOffSettings();
  206 |   }
  207 | 
  208 |   async turnOffSettings() {
  209 |     await this.actions.click(this.crossBtnToTurnoffSettings);
  210 |   }
  211 | 
  212 |   async verifyAddedQuestionnaireLinked(questionnaireName: string) {
  213 |     const linkedItem = this.page.locator(`[data-testid="${questionnaireName}"]`);
  214 | 
  215 |     await expect(linkedItem).toBeVisible();
  216 |   }
  217 | 
  218 |   async clickOnQuestionnaire(questionnaireName: string) {
  219 |     const questionnaire = this.page.locator(`[data-testid="${questionnaireName}"]`);
  220 |     await expect(questionnaire).toBeVisible({ timeout: 10000 });
  221 |     await this.actions.click(questionnaire);
  222 |   }
  223 | 
  224 |   async openRiskByName(riskName: string) {
  225 |     const riskCell = this.page.getByRole('gridcell', { name: riskName });
  226 | 
  227 |     await this.actions.click(riskCell);
  228 |   }
  229 | 
  230 |   async verifyQuestionnaireIsFinished(questionnaireName: string) {
  231 |     const finishedIcon = this.page.locator(`[data-testid="${questionnaireName}"] [alt="finished"]`);
  232 | 
  233 |     await this.actions.waitForVisible(finishedIcon);
  234 | 
  235 |     const progress = this.page.locator(`[data-testid="${questionnaireName}"] div[progressvalue]`);
  236 | 
  237 |     await expect(progress).toContainText('100%');
  238 |   }
  239 | 
  240 |   async searchRisk(riskName: string) {
  241 |     await this.actions.click(this.searchIcon);
  242 |     await this.actions.type(this.searchInput, riskName);
  243 |     await this.searchInput.press('Enter');
  244 |   }
  245 | 
  246 |   async clickCloseDialogButton() {
  247 |     if (await this.closeDialogButton.isVisible()) {
  248 |       await this.actions.click(this.closeDialogButton);
  249 |     }
  250 |     else {
  251 |       const closeDialogueNew = this.page.getByRole('button', { name: 'Close dialog' });
  252 |       await this.actions.click(closeDialogueNew);
  253 |     }
  254 |   }
  255 | 
  256 |   async clickCloseQuestionnaireButton() {
  257 |     const closeQuestionnaireButton = this.page.locator('[data-testid="moqnr-close-icon"]');
  258 |     await this.actions.click(closeQuestionnaireButton);
  259 |   }
  260 | 
  261 |   async verifyAuditLogFieldValue(fieldName: string, expectedValue: string) {
  262 |     await this.actions.click(this.latestHistoryLog);
  263 | 
  264 |     const field = this.page.getByRole('textbox', { name: fieldName });
  265 |     await expect(field).toHaveValue(expectedValue);
  266 | 
  267 |     await this.clickCloseDialogButton();
  268 |   }
  269 | 
  270 |   async clickOnVariableIcon() {
  271 |     await this.actions.click(this.variableIcon);
  272 |   }
  273 | 
  274 |   async clickOnMoreOptionsInCard(cardName: string) {
  275 |     const moreOption = this.page
  276 |       .locator(`[data-testid="${cardName}"]`)
  277 |       .getByRole('button', { name: 'more_vert' });
  278 | 
  279 |     await this.actions.click(moreOption);
  280 |   }
  281 | 
  282 |   async clickConditionSettingMenuItem() {
  283 |     const conditionSettingsMenuItem = this.page.getByRole('menuitem', { name: 'Condition settings' });
  284 |     await this.actions.click(conditionSettingsMenuItem);
  285 |   }
  286 | 
  287 |   async clickQuestionnaireConditionsTab() {
  288 |     const questionnaireConditionsTab = this.page.getByRole('tab', { name: 'QUESTIONNAIRE CONDITIONS' }).last();
```