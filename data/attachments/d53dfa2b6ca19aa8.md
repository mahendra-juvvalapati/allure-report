# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: E2E_Tests/FC003_Questionnaire.spec.ts >> FC_003_Questionnaire Flow >> Configure questionnaire with 'MO-Items links in question details tab' and verify 'Enable' action is executed when Question condition is triggered on 'Completing the page' and check Questionnaire 'Import from' action
- Location: tests/E2E_Tests/FC003_Questionnaire.spec.ts:37:7

# Error details

```
Error: Column "Name" not found
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
          - status "26" [ref=e42]
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
          - button "version:No repeatplan - 1 Version name keyboard_arrow_down" [ref=e224] [cursor=pointer]:
            - generic [ref=e225]: version:No repeatplan - 1 Version name
            - generic [ref=e226]: keyboard_arrow_down
          - button "toggle archived" [ref=e229] [cursor=pointer]:
            - img [ref=e230]:
              - img
          - generic [ref=e231]:
            - button "add mo to projects" [ref=e233] [cursor=pointer]:
              - img [ref=e234]:
                - img
            - button [ref=e235] [cursor=pointer]:
              - img [ref=e237]:
                - img [ref=e238]
        - text: ▼
      - generic [ref=e239]:
        - generic [ref=e241]:
          - img [ref=e243]:
            - img
          - generic [ref=e244]:
            - generic [ref=e246]: "Risk: Risk 1779188975172"
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
              - button "Previous Page" [ref=e261] [cursor=pointer]:
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
                  - tab "Dialogue" [ref=e282] [cursor=pointer]:
                    - generic [ref=e284]: Dialogue
                  - tab "Chat" [ref=e285] [cursor=pointer]:
                    - generic [ref=e287]: Chat
                  - tab "Information systems" [ref=e288] [cursor=pointer]:
                    - generic [ref=e290]: Information systems
                  - tab "Related" [active] [selected] [ref=e291]:
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
            - tabpanel "Related" [ref=e360]:
              - generic [ref=e366]:
                - generic [ref=e368]:
                  - img [ref=e370]
                  - heading "There are no items added and/or linked yet" [level=2] [ref=e514]
                  - text: Click on the (+) button in the lower right corner to add and/or link new item
                - text: more_vert
      - button [ref=e515] [cursor=pointer]:
        - img [ref=e517]: add
  - iframe [ref=e519]:
    - generic [active]:
      - generic:
        - text:  
        - button "Open chat" [ref=f6e1] [cursor=pointer]
```

# Test source

```ts
  99  | 
  100 |   async verifyNotChecked(element: Locator) {
  101 |     await expect(element).not.toBeChecked();
  102 |   }
  103 | 
  104 |   async verifyAttached(element: Locator) {
  105 |     await expect(element).toBeAttached();
  106 |   }
  107 | 
  108 |   async verifyVisible(element: Locator) {
  109 |     await expect(element).toBeVisible();
  110 |   }
  111 | 
  112 |   async verifyNotVisible(element: Locator) {
  113 |     await expect(element).not.toBeVisible();
  114 |   }
  115 | 
  116 |   async verifyHidden(element: Locator) {
  117 |     await expect(element).toBeHidden();
  118 |   }
  119 | 
  120 |   async verifyEnabled(element: Locator) {
  121 |     await expect(element).toBeEnabled();
  122 |   }
  123 | 
  124 |   async verifyDisabled(element: Locator) {
  125 |     await expect(element).toBeDisabled();
  126 |   }
  127 | 
  128 |   async waitForVisible(element: Locator) {
  129 |     await element.waitFor({ state: 'visible' });
  130 |   }
  131 | 
  132 |   async waitForHidden(element: Locator) {
  133 |     await element.waitFor({ state: 'hidden' });
  134 |   }
  135 | 
  136 |   async waitForURL(url: RegExp | string) {
  137 |     await this.page.waitForURL(url);
  138 |   }
  139 | 
  140 |   async waitForLoad() {
  141 |     await this.page.waitForLoadState('load');
  142 |   }
  143 | 
  144 |   async scrollIntoView(element: Locator) {
  145 |     await element.scrollIntoViewIfNeeded();
  146 |   }
  147 | 
  148 |   async pressKey(element: Locator, key: string) {
  149 |     await element.press(key);
  150 |   }
  151 | 
  152 |   async pressOnPage(key: string) {
  153 |     await this.page.keyboard.press(key);
  154 |   }
  155 | 
  156 |   async uploadFile(element: Locator, filePath: string) {
  157 |     await element.setInputFiles(filePath);
  158 |   }
  159 | 
  160 |   async toggleSwitch(locator: Locator, expectedState: boolean) {
  161 |     const currentState = await locator.getAttribute("aria-checked");
  162 |     const isChecked = currentState === "true";
  163 |     if (isChecked !== expectedState) {
  164 |       await locator.click();
  165 |     }
  166 |     const updatedState = await locator.getAttribute("aria-checked");
  167 |     expect(updatedState).toBe(expectedState ? "true" : "false");
  168 |   }
  169 | 
  170 |   async toggleCheckbox(locator: Locator, expectedState: boolean) {
  171 |     let isChecked: boolean;
  172 |     try {
  173 |       isChecked = await locator.isChecked();
  174 |     } catch {
  175 |       const ariaChecked = await locator.getAttribute("aria-checked");
  176 |       isChecked = ariaChecked === "true";
  177 |     }
  178 |     if (isChecked !== expectedState) {
  179 |       await locator.click();
  180 |     }
  181 |     try {
  182 |       await expect(locator).toBeChecked({ checked: expectedState });
  183 |     } catch {
  184 |       const updatedState = await locator.getAttribute("aria-checked");
  185 |       expect(updatedState).toBe(expectedState ? "true" : "false");
  186 |     }
  187 |   }
  188 | 
  189 |   async getColumnIndex(columnName: string) {
  190 |     const headers = this.page.locator('.ui-grid-header-cell');
  191 |     const count = await headers.count();
  192 |     for (let i = 0; i < count; i++) {
  193 |       const text = await headers.nth(i).innerText();
  194 |       if (text.trim() === columnName) {
  195 |         return i;
  196 |       }
  197 |     }
  198 | 
> 199 |     throw new Error(`Column "${columnName}" not found`);
      |           ^ Error: Column "Name" not found
  200 |   }
  201 | 
  202 |   async verifyCellValue(rowLocator: Locator, columnName: string, expectedValue: string) {
  203 |     const colIndex = await this.getColumnIndex(columnName);
  204 |     const cell = rowLocator.locator('[role="gridcell"]').nth(colIndex);
  205 |     await expect(cell).toContainText(expectedValue);
  206 |   }
  207 | 
  208 |   async setPageZoom(percentage: number): Promise<void> {
  209 |     if (percentage <= 0) {
  210 |       throw new Error('Zoom percentage must be greater than 0');
  211 |     }
  212 | 
  213 |     await this.page.evaluate((zoom) => {
  214 |       document.body.style.zoom = `${zoom}%`;
  215 |     }, percentage);
  216 |   }
  217 | 
  218 |   async verifyFileDownload(downloadButton: Locator, expectedFileName: string) {
  219 |     const [download] = await Promise.all([
  220 |       this.page.waitForEvent('download'),
  221 |       downloadButton.click(),
  222 |     ]);
  223 | 
  224 |     const downloadedFileName = download.suggestedFilename();
  225 |     expect(downloadedFileName).toContain(expectedFileName);
  226 |     const filePath = await download.path();
  227 |     expect(filePath).not.toBeNull();
  228 |     expect(fs.existsSync(filePath!)).toBeTruthy();
  229 |     console.log(`Downloaded File: ${downloadedFileName}`);
  230 |   }
  231 | 
  232 | }
  233 | 
```