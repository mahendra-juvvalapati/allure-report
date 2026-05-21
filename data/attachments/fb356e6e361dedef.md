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

Locator: locator('span').filter({ hasText: 'Risk:' }).last()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for locator('span').filter({ hasText: 'Risk:' }).last()

```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
  - text: ×
  - link "ticket or feedback" [ref=e2] [cursor=pointer]:
    - /url: javascript:void(0)
    - img "ticket or feedback" [ref=e3]
  - main [ref=e6]:
    - generic [ref=e10]:
      - generic [ref=e12]:
        - button "leftMenuOpen" [ref=e13] [cursor=pointer]:
          - img [ref=e14]
        - generic [ref=e15]:
          - img [ref=e19]
          - heading "QualiTlabs Hyd" [level=2] [ref=e23]
        - generic [ref=e27] [cursor=pointer]: search
        - button "Turn off admin role" [ref=e28] [cursor=pointer]:
          - img [ref=e29]:
            - img
        - button [ref=e31] [cursor=pointer]:
          - img [ref=e33]:
            - img [ref=e34]
        - generic [ref=e39]:
          - button [ref=e40] [cursor=pointer]:
            - img [ref=e42]:
              - img [ref=e43]
          - status "31" [ref=e44]
        - button "fullscreen" [ref=e45] [cursor=pointer]:
          - generic [ref=e46]: fullscreen
        - button "Open beamer" [ref=e47] [cursor=pointer]:
          - img [ref=e48]:
            - img
          - generic [ref=e49]: "1"
        - button "freshDesk" [ref=e50] [cursor=pointer]:
          - generic [ref=e51]: info
      - generic [ref=e52]:
        - generic [ref=e53]:
          - img [ref=e54] [cursor=pointer]
          - button "dehaze" [ref=e55] [cursor=pointer]:
            - generic [ref=e56]: dehaze
        - list [ref=e57]:
          - generic [ref=e58]:
            - button "profile pic" [ref=e59]
            - generic [ref=e60]: mahendra j
          - button "keyboard_arrow_down mahendra.juvvalapati@qualitlabs.com" [ref=e61] [cursor=pointer]:
            - generic [ref=e62]: keyboard_arrow_down
            - generic [ref=e63]: mahendra.juvvalapati@qualitlabs.com
          - list [ref=e64]:
            - button "account_box My Data" [ref=e65] [cursor=pointer]:
              - generic [ref=e66]: account_box
              - generic [ref=e67]: My Data
            - button "settings Settings" [ref=e68] [cursor=pointer]:
              - generic [ref=e69]: settings
              - generic [ref=e70]: Settings
            - button "exit_to_app Logout" [ref=e71] [cursor=pointer]:
              - generic [ref=e72]: exit_to_app
              - generic [ref=e73]: Logout
        - list [ref=e75]:
          - button "Add new user" [ref=e76] [cursor=pointer]:
            - img [ref=e77]:
              - img
            - generic [ref=e78]: Add new user
          - button "business Environments" [ref=e79] [cursor=pointer]:
            - generic [ref=e80]: business
            - generic [ref=e81]: Environments
          - button "home Dashboard" [ref=e82] [cursor=pointer]:
            - generic [ref=e83]: home
            - generic [ref=e84]: Dashboard
          - button "widgets Modules keyboard_arrow_down" [ref=e85] [cursor=pointer]:
            - generic [ref=e86]: widgets
            - generic [ref=e87]: Modules
            - generic [ref=e88]: keyboard_arrow_down
          - list [ref=e89]:
            - button "Strategy" [ref=e90] [cursor=pointer]:
              - img [ref=e91]:
                - img
              - generic [ref=e92]: Strategy
            - button "Policy" [ref=e93] [cursor=pointer]:
              - img [ref=e94]:
                - img
              - generic [ref=e95]: Policy
            - button "Programs" [ref=e96] [cursor=pointer]:
              - img [ref=e97]:
                - img
              - generic [ref=e98]: Programs
            - button "projects" [ref=e99] [cursor=pointer]:
              - img [ref=e100]:
                - img
              - generic [ref=e101]: projects
            - button "Dialogues" [ref=e102] [cursor=pointer]:
              - img [ref=e103]:
                - img
              - generic [ref=e104]: Dialogues
            - button "Objectives" [ref=e105] [cursor=pointer]:
              - img [ref=e106]:
                - img
              - generic [ref=e107]: Objectives
            - button "Processes" [ref=e108] [cursor=pointer]:
              - img [ref=e109]:
                - img
              - generic [ref=e110]: Processes
            - button "Organisation functions" [ref=e111] [cursor=pointer]:
              - img [ref=e112]:
                - img
              - generic [ref=e113]: Organisation functions
            - button "KSF's - Opportunities" [ref=e114] [cursor=pointer]:
              - img [ref=e115]:
                - img
              - generic [ref=e116]: KSF's - Opportunities
            - button "Stakeholders" [ref=e117] [cursor=pointer]:
              - img [ref=e118]:
                - img
              - generic [ref=e119]: Stakeholders
            - button "Risks" [ref=e120] [cursor=pointer]:
              - img [ref=e121]:
                - img
              - generic [ref=e122]: Risks
            - button "Opportunities" [ref=e123] [cursor=pointer]:
              - img [ref=e124]:
                - img
              - generic [ref=e125]: Opportunities
            - button "Standards Frameworks" [ref=e126] [cursor=pointer]:
              - img [ref=e127]:
                - img
              - generic [ref=e128]: Standards Frameworks
            - button "Laws and regulations" [ref=e129] [cursor=pointer]:
              - img [ref=e130]:
                - img
              - generic [ref=e131]: Laws and regulations
            - button "Measures" [ref=e132] [cursor=pointer]:
              - img [ref=e133]:
                - img
              - generic [ref=e134]: Measures
            - button "Assets" [ref=e135] [cursor=pointer]:
              - img [ref=e136]:
                - img
              - generic [ref=e137]: Assets
            - button "Information systems" [ref=e138] [cursor=pointer]:
              - img [ref=e139]:
                - img
              - generic [ref=e140]: Information systems
            - button "Processing" [ref=e141] [cursor=pointer]:
              - img [ref=e142]:
                - img
              - generic [ref=e143]: Processing
            - button "Audits" [ref=e144] [cursor=pointer]:
              - img [ref=e145]:
                - img
              - generic [ref=e146]: Audits
            - button "Audit sets" [ref=e147] [cursor=pointer]:
              - img [ref=e148]:
                - img
              - generic [ref=e149]: Audit sets
            - button "Impact Assessments" [ref=e150] [cursor=pointer]:
              - img [ref=e151]:
                - img
              - generic [ref=e152]: Impact Assessments
            - button "Tests" [ref=e153] [cursor=pointer]:
              - img [ref=e154]:
                - img
              - generic [ref=e155]: Tests
            - button "Findings" [ref=e156] [cursor=pointer]:
              - img [ref=e157]:
                - img
              - generic [ref=e158]: Findings
            - button "Problems" [ref=e159] [cursor=pointer]:
              - img [ref=e160]:
                - img
              - generic [ref=e161]: Problems
            - button "Changes" [ref=e162] [cursor=pointer]:
              - img [ref=e163]:
                - img
              - generic [ref=e164]: Changes
            - button "Cases" [ref=e165] [cursor=pointer]:
              - img [ref=e166]:
                - img
              - generic [ref=e167]: Cases
            - button "Tasks" [ref=e168] [cursor=pointer]:
              - img [ref=e169]:
                - img
              - generic [ref=e170]: Tasks
            - button "Documents" [ref=e171] [cursor=pointer]:
              - img [ref=e172]:
                - img
              - generic [ref=e173]: Documents
            - button "News items" [ref=e174] [cursor=pointer]:
              - img [ref=e175]:
                - img
              - generic [ref=e176]: News items
            - button "Related parties" [ref=e177] [cursor=pointer]:
              - img [ref=e178]:
                - img
              - generic [ref=e179]: Related parties
            - button "Contracts" [ref=e180] [cursor=pointer]:
              - img [ref=e181]:
                - img
              - generic [ref=e182]: Contracts
            - button "Vendors" [ref=e183] [cursor=pointer]:
              - img [ref=e184]:
                - img
              - generic [ref=e185]: Vendors
            - button "Performance agreements" [ref=e186] [cursor=pointer]:
              - img [ref=e187]:
                - img
              - generic [ref=e188]: Performance agreements
            - button "Key Figures" [ref=e189] [cursor=pointer]:
              - img [ref=e190]:
                - img
              - generic [ref=e191]: Key Figures
            - button "Settings" [ref=e192] [cursor=pointer]:
              - img [ref=e193]:
                - img
              - generic [ref=e194]: Settings
            - button "Critical Business Scenarios" [ref=e195] [cursor=pointer]:
              - img [ref=e196]:
                - img
              - generic [ref=e197]: Critical Business Scenarios
            - button "BCM Plans" [ref=e198] [cursor=pointer]:
              - img [ref=e199]:
                - img
              - generic [ref=e200]: BCM Plans
            - button "Context analysis" [ref=e201] [cursor=pointer]:
              - img [ref=e202]:
                - img
              - generic [ref=e203]: Context analysis
            - button "Situations" [ref=e204] [cursor=pointer]:
              - img [ref=e205]:
                - img
              - generic [ref=e206]: Situations
  - iframe [ref=e209]:
    - generic [active]:
      - generic:
        - text:  
        - button "Open chat" [ref=f6e1] [cursor=pointer]
```

# Test source

```ts
  3   | 
  4   | export class RisksPage extends BasePage {
  5   |   readonly addNewRiskButton: Locator;
  6   |   readonly newItemButton: Locator;
  7   |   readonly moStatesDropdown: Locator;
  8   |   readonly nameInput: Locator;
  9   |   readonly descriptionInput: Locator;
  10  |   readonly saveButton: Locator;
  11  |   readonly dialogueTab: Locator;
  12  |   readonly closeBtn: Locator;
  13  |   readonly settingsIcon: Locator;
  14  |   readonly addBtnToLinkQuestionnaire: Locator;
  15  |   readonly knowledgeDataBaseDropdown: Locator;
  16  |   readonly searchQuestionnaireInput: Locator;
  17  |   readonly okBtn: Locator;
  18  |   readonly crossBtnToTurnoffSettings: Locator;
  19  |   readonly searchIcon: Locator;
  20  |   readonly searchInput: Locator;
  21  |   readonly closeDialogButton: Locator;
  22  |   readonly historyTab: Locator;
  23  |   readonly latestHistoryLog: Locator;
  24  |   readonly variableIcon: Locator;
  25  |   readonly risksHeading: Locator;
  26  |   readonly indicatorsTab: Locator;
  27  |   readonly grossRiskTab: Locator;
  28  |   readonly relatedtab: Locator;
  29  |   readonly grossRiskColumns: Locator;
  30  |   readonly moDataTab: Locator;
  31  |   readonly moQualityStateDropdown: Locator;
  32  |   readonly moQualityState: Locator;
  33  |   readonly prevButton: Locator;
  34  |   readonly riskStatus: Locator;
  35  |   readonly executorDropdown: Locator;
  36  |   readonly ownerDropdown: Locator;
  37  |   readonly nextButton: Locator;
  38  | 
  39  | 
  40  |   constructor(page: Page) {
  41  |     super(page);
  42  | 
  43  |     this.addNewRiskButton = page.getByRole('button').filter({ hasText: /^add$/ });
  44  |     this.newItemButton = page.getByTestId('newItem').first();
  45  |     this.moStatesDropdown = page.getByTestId('moStates').last();
  46  |     this.nameInput = page.getByTestId('name').last();
  47  |     this.descriptionInput = page.getByTestId('description').last();
  48  |     this.saveButton = page.getByTestId('Save');
  49  |     this.dialogueTab = page.getByRole('tab', { name: 'Dialogue', exact: true });
  50  |     this.historyTab = page.getByRole('tab', { name: 'History' });
  51  |     this.latestHistoryLog = page.locator('.audit-trail-log').first();
  52  |     this.closeDialogButton = page.locator('i').filter({ hasText: 'close' }).last();
  53  |     this.risksHeading = page.locator('.q-toolbar__title:has-text("Risks")');
  54  |     this.indicatorsTab = page.getByRole('tab', { name: 'Key Indicators' });
  55  |     this.grossRiskTab = page.getByRole('tab', { name: 'Gross risk' });
  56  |     this.closeBtn = page.getByRole('button', { name: 'CLOSE' }).last();
  57  |     this.relatedtab = page.getByRole('tab', { name: 'Related' });
  58  |     this.grossRiskColumns = page.locator('.q-field__control-container.col.relative-position.row.no-wrap.q-anchor--skip');
  59  |     this.riskStatus = page.getByTestId('moStates');
  60  |     this.executorDropdown = page.getByTestId('executor');
  61  |     this.ownerDropdown = page.getByTestId('owner');
  62  |     this.nextButton = this.page.locator('[data-testid="moqnr-next-button"]');
  63  | 
  64  |     this.moDataTab = page.getByRole('tab', { name: 'mo data' });
  65  |     this.settingsIcon = page
  66  |       .locator('[data-testid="mo-toolbar"]')
  67  |       .getByRole('button', { name: 'settings' });
  68  | 
  69  |     this.addBtnToLinkQuestionnaire = page.getByRole('button', {
  70  |       name: 'add',
  71  |       exact: true,
  72  |     });
  73  | 
  74  |     this.knowledgeDataBaseDropdown = page.getByRole('button', {
  75  |       name: 'select country',
  76  |     });
  77  | 
  78  |     this.searchQuestionnaireInput = page.getByRole('textbox', {
  79  |       name: 'Enter search',
  80  |     });
  81  | 
  82  |     this.okBtn = page.getByRole('button', { name: 'OK' });
  83  | 
  84  |     this.crossBtnToTurnoffSettings = page.getByRole('button', { name: 'clear' });
  85  | 
  86  |     this.searchIcon = page.locator("div[id*='search-icon']");
  87  | 
  88  |     this.searchInput = page.locator('div[isfilteractive="false"] [placeholder="Type to Search"]');
  89  | 
  90  |     this.variableIcon = page.getByRole('button', { name: 'variables' });
  91  |     this.moQualityState = page.getByTestId('MoQualityState');
  92  |     this.moQualityStateDropdown = page.getByTestId('MoQualityStateDropdown');
  93  |     this.moQualityState = page.locator('select[name="MoQualityState"]');
  94  |     this.prevButton = page.locator('[aria-label="Previous Page"]');
  95  |   }
  96  | 
  97  |   async createNewRisk(name: string, description: string, status: string) {
  98  |     await this.selectNewItemOption();
  99  |     await this.setMoState(status);
  100 |     await this.fillRiskName(name);
  101 |     await this.fillRiskDescription(description);
  102 |     await this.saveRisk();
> 103 |     await expect(this.page.locator('span').filter({ hasText: 'Risk:' }).last()).toBeVisible();
      |                                                                                 ^ Error: expect(locator).toBeVisible() failed
  104 |   }
  105 | 
  106 |   async createNewRiskWithData(data: any) {
  107 |     await this.createNewRisk(data.name, data.description, data.status);
  108 |   }
  109 | 
  110 |   private async selectNewItemOption() {
  111 |     await this.actions.click(this.newItemButton);
  112 |   }
  113 | 
  114 |   private async setMoState(state: string) {
  115 |     await this.actions.click(this.moStatesDropdown);
  116 | 
  117 |     const option = this.page.getByRole('option', { name: state });
  118 |     await this.actions.click(option);
  119 |   }
  120 | 
  121 |   private async fillRiskName(name: string) {
  122 |     await this.actions.click(this.nameInput);
  123 |     await this.actions.type(this.nameInput, name);
  124 |   }
  125 | 
  126 |   private async fillRiskDescription(description: string) {
  127 |     await this.actions.click(this.descriptionInput);
  128 |     await this.actions.type(this.descriptionInput, description);
  129 |   }
  130 | 
  131 |   private async saveRisk() {
  132 |     await this.actions.click(this.saveButton);
  133 |   }
  134 | 
  135 |   async clickDialogueTab() {
  136 |     await this.page.waitForTimeout(2000);
  137 |     await this.actions.click(this.dialogueTab);
  138 |   }
  139 | 
  140 |   async clickHistoryTab() {
  141 |     await this.actions.click(this.historyTab);
  142 |     // await this.page.waitForLoadState('networkidle');
  143 |   }
  144 | 
  145 |   async clickOnAddNewRiskBtn() {
  146 |     await this.page.waitForTimeout(1500);
  147 |     try {
  148 |       await this.actions.verifyVisible(this.risksHeading);
  149 |       await this.actions.click(this.addNewRiskButton);
  150 |       await expect(this.newItemButton).toBeVisible({ timeout: 15000 });
  151 |     } catch (error) {
  152 |       // console.error('Error occurred while clicking on Add New Risk button:', error);
  153 |       await this.actions.click(this.addNewRiskButton);
  154 | 
  155 |     }
  156 |   }
  157 | 
  158 |   async clickOnSettingsIcon() {
  159 |     await this.actions.click(this.settingsIcon);
  160 |   }
  161 | 
  162 |   async clickOnAddBtnToLinkQuestionnaire() {
  163 |     await this.actions.click(this.addBtnToLinkQuestionnaire);
  164 |   }
  165 | 
  166 |   async clickOnKnowledgeDatabaseDropdown() {
  167 |     await this.actions.click(this.knowledgeDataBaseDropdown);
  168 |   }
  169 | 
  170 |   async selectKnowledgeDatabaseOption(option: string) {
  171 |     await this.actions.click(this.knowledgeDataBaseDropdown);
  172 | 
  173 |     const dropdownOption = this.page.getByRole('option', { name: option });
  174 |     await this.actions.click(dropdownOption);
  175 |   }
  176 | 
  177 |   async searchQuestionnaire(questionnaireName: string) {
  178 |     await this.actions.type(this.searchQuestionnaireInput, questionnaireName);
  179 |   }
  180 | 
  181 |   async linkQuestionnaire(questionnaireName: string) {
  182 |     await this.searchQuestionnaire(questionnaireName);
  183 |     const checkbox = this.page
  184 |       .getByText(`${questionnaireName} Link`)
  185 |       .getByRole('checkbox', { name: 'ql._id' });
  186 |     await this.page.locator('.MOQPopupHeight > .layout-wrap').click();
  187 |     await expect(checkbox).toBeVisible({ timeout: 15000 });
  188 |     await this.actions.waitForVisible(checkbox);
  189 |     await this.actions.check(checkbox);
  190 |   }
  191 | 
  192 |   async clickOkButton() {
  193 |     await this.actions.click(this.okBtn);
  194 |   }
  195 | 
  196 |   async linkQuestionnaireToRisk(questionnaireName: string, knowledgeDatabaseOption: string) {
  197 |     await this.clickOnSettingsIcon();
  198 |     await this.clickOnAddBtnToLinkQuestionnaire();
  199 |     await this.selectKnowledgeDatabaseOption(knowledgeDatabaseOption);
  200 |     await this.page.waitForTimeout(3000);
  201 |     await this.linkQuestionnaire(questionnaireName);
  202 |     await expect(this.okBtn).toBeEnabled({ timeout: 10000 });
  203 |     await this.clickOkButton();
```