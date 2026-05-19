# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: E2E_Tests/FC025_questionnaire.spec.ts >> FC_025_Questionnaire Flow >> Configure questionnaire with 'Disable non conformity for question' and verify 'Unlock' action is executed when Question condition is triggered on 'Entering the questionnaire the first time' and check Questionnaire 'Set item state to' action
- Location: tests/E2E_Tests/FC025_questionnaire.spec.ts:31:9

# Error details

```
TimeoutError: locator.click: Timeout 15000ms exceeded.
Call log:
  - waiting for getByRole('img', { name: 'quick-version' }).last()
    - locator resolved to <md-icon role="img" aria-label="quick-version" class="colorWhite ng-scope" md-svg-src="images/icons/quickVersion.svg">…</md-icon>
  - attempting click action
    2 × waiting for element to be visible, enabled and stable
      - element is visible, enabled and stable
      - scrolling into view if needed
      - done scrolling
      - <div tabindex="-1" class="md-dialog-container ng-scope">…</div> intercepts pointer events
    - retrying click action
    - waiting 20ms
    2 × waiting for element to be visible, enabled and stable
      - element is visible, enabled and stable
      - scrolling into view if needed
      - done scrolling
      - <div tabindex="-1" class="md-dialog-container ng-scope">…</div> intercepts pointer events
    - retrying click action
      - waiting 100ms
    20 × waiting for element to be visible, enabled and stable
       - element is visible, enabled and stable
       - scrolling into view if needed
       - done scrolling
       - <div tabindex="-1" class="md-dialog-container ng-scope">…</div> intercepts pointer events
     - retrying click action
       - waiting 500ms

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
          - status [ref=e43]: "104"
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
          - generic [ref=e216]:
            - generic [ref=e217] [cursor=pointer]:
              - generic: apps
              - generic:
                - img
            - list [ref=e218]:
              - listitem [ref=e219]:
                - generic [ref=e221]:
                  - generic:
                    - img
                  - generic [ref=e222]: Risk
          - button [ref=e225] [cursor=pointer]:
            - generic [ref=e226]: version:No repeatplan - 1 Version name
            - generic [ref=e227]: keyboard_arrow_down
            - generic [ref=e228]: "Executor: ALL"
          - button [ref=e230] [cursor=pointer]:
            - img [ref=e231]: settings
          - generic [ref=e232]:
            - button [ref=e234] [cursor=pointer]:
              - img [ref=e235]:
                - img
            - button [ref=e236] [cursor=pointer]:
              - img [ref=e238]:
                - img [ref=e239]
        - text: ▼ ▼
      - generic [ref=e240]:
        - generic [ref=e242]:
          - img [ref=e244]:
            - img
          - generic [ref=e245]:
            - generic [ref=e247]: "Risk: Risk_1779197945858"
            - button [ref=e249] [cursor=pointer]:
              - img [ref=e250]: file_copy
            - button [ref=e251] [cursor=pointer]:
              - img [ref=e252]:
                - img
            - generic [ref=e253]:
              - button [disabled] [ref=e254]:
                - img [ref=e255]:
                  - img
              - button [disabled] [ref=e256]:
                - img [ref=e257]:
                  - img
        - generic [ref=e258]:
          - img:
            - img
          - generic [ref=e259]:
            - generic [ref=e260]:
              - button [disabled] [ref=e262]:
                - img [ref=e263]:
                  - img
              - button [ref=e264] [cursor=pointer]:
                - img [ref=e265]:
                  - img
              - generic [ref=e266]:
                - tablist [ref=e267]:
                  - tab [ref=e268] [cursor=pointer]:
                    - generic [ref=e270]: Gross risk
                  - tab [ref=e271] [cursor=pointer]:
                    - generic [ref=e273]: Net risk
                  - tab [ref=e274] [cursor=pointer]:
                    - generic [ref=e276]: Bowtie
                  - tab [ref=e277] [cursor=pointer]:
                    - generic [ref=e279]: Measures
                  - tab [ref=e280] [cursor=pointer]:
                    - generic [ref=e282]: Kritieke Bedrijfsfuncties
                  - tab [selected] [ref=e283]:
                    - generic [ref=e285]: Dialogue
                  - tab [ref=e286] [cursor=pointer]:
                    - generic [ref=e288]: Chat
                  - tab [ref=e289] [cursor=pointer]:
                    - generic [ref=e291]: Information systems
                  - tab [ref=e292] [cursor=pointer]:
                    - generic [ref=e294]: Related
                  - tab [ref=e295] [cursor=pointer]:
                    - generic [ref=e297]: Tasks
                  - tab [ref=e298] [cursor=pointer]:
                    - generic [ref=e300]: Key Indicators
                  - tab [ref=e301] [cursor=pointer]:
                    - generic [ref=e303]: History
                  - tab [ref=e304] [cursor=pointer]:
                    - generic [ref=e306]: mo data
                  - tab [ref=e307] [cursor=pointer]:
                    - generic [ref=e309]: Documents
                  - tab [ref=e310] [cursor=pointer]:
                    - generic [ref=e312]: Risks
                - generic [ref=e314]:
                  - generic [ref=e317] [cursor=pointer]: Gross risk
                  - generic [ref=e320] [cursor=pointer]: Net risk
                  - generic [ref=e323] [cursor=pointer]: Bowtie
                  - generic [ref=e326] [cursor=pointer]: Measures
                  - generic [ref=e329] [cursor=pointer]: Kritieke Bedrijfsfuncties
                  - generic [ref=e332] [cursor=pointer]: Dialogue
                  - generic [ref=e335] [cursor=pointer]: Chat
                  - generic [ref=e338] [cursor=pointer]: Information systems
                  - generic [ref=e341] [cursor=pointer]: Related
                  - generic [ref=e344] [cursor=pointer]: Tasks
                  - generic [ref=e347] [cursor=pointer]: Key Indicators
                  - generic [ref=e350] [cursor=pointer]: History
                  - generic [ref=e353] [cursor=pointer]: mo data
                  - generic [ref=e356] [cursor=pointer]: Documents
                  - generic [ref=e359] [cursor=pointer]: Risks
            - tabpanel [ref=e361]:
              - button [ref=e371] [cursor=pointer]:
                - generic [ref=e372]:
                  - img [ref=e374]
                  - generic [ref=e376]: Questionnaire_1779197945858
                - img [ref=e378]
                - generic [ref=e382]: 100%
  - iframe [ref=e384]:
    - generic [active]:
      - generic:
        - text:  
        - button "Open chat" [ref=f4e1] [cursor=pointer]
  - dialog "messagePopup" [ref=e387]:
    - generic [ref=e388]:
      - generic [ref=e389]:
        - generic [ref=e390]:
          - heading "Warning" [level=2] [ref=e391]
          - button "Close dialog" [ref=e392] [cursor=pointer]:
            - img "Close dialog" [ref=e393]:
              - img
        - img:
          - img
        - paragraph [ref=e394]: Do you want to close this version and create a new one. CAUTION - After this, the questionnaire and forms in the old version can no longer be changed. You can only continue working in the new version of the item!!
      - generic [ref=e395]:
        - button "Yes" [ref=e396] [cursor=pointer]
        - button "No" [active] [ref=e397] [cursor=pointer]
```

# Test source

```ts
  1   | import { Locator, Page, expect } from '@playwright/test';
  2   | import fs from 'fs';
  3   | 
  4   | export class UIActions {
  5   |   constructor(private page: Page) { }
  6   | 
  7   |   async click(element: Locator) {
  8   |     await expect(element).toBeVisible();
  9   |     await expect(element).toBeEnabled();
> 10  |     await element.click();
      |                   ^ TimeoutError: locator.click: Timeout 15000ms exceeded.
  11  |   }
  12  | 
  13  |   async doubleClick(element: Locator) {
  14  |     await expect(element).toBeVisible();
  15  |     await element.dblclick();
  16  |   }
  17  | 
  18  |   async rightClick(element: Locator) {
  19  |     await expect(element).toBeVisible();
  20  |     await element.click({ button: 'right' });
  21  |   }
  22  | 
  23  |   async hover(element: Locator) {
  24  |     await expect(element).toBeVisible();
  25  |     await element.hover();
  26  |   }
  27  | 
  28  |   async type(element: Locator, value: string) {
  29  |     await expect(element).toBeVisible();
  30  |     await expect(element).toBeEnabled();
  31  |     await element.clear();
  32  |     await element.fill(value);
  33  |     await expect(element).toHaveValue(value);
  34  |   }
  35  | 
  36  |   async typeWithoutClearing(element: Locator, value: string) {
  37  |     await expect(element).toBeEnabled();
  38  |     await element.type(value);
  39  | 
  40  |     const currentValue = await element.inputValue();
  41  |     expect(currentValue).toContain(value);
  42  |   }
  43  | 
  44  |   async clear(element: Locator) {
  45  |     await expect(element).toBeEnabled();
  46  |     await element.clear();
  47  |     await expect(element).toHaveValue('');
  48  |   }
  49  | 
  50  |   async check(element: Locator) {
  51  |     // await expect(element).toBeVisible();
  52  |     await element.check();
  53  |     await expect(element).toBeChecked();
  54  |   }
  55  | 
  56  |   async uncheck(element: Locator) {
  57  |     await expect(element).toBeVisible();
  58  |     await element.uncheck();
  59  |     await expect(element).not.toBeChecked();
  60  |   }
  61  | 
  62  |   async selectByValue(element: Locator, value: string) {
  63  |     await element.selectOption(value);
  64  |     await expect(element).toHaveValue(value);
  65  |   }
  66  | 
  67  |   async selectByLabel(element: Locator, label: string) {
  68  |     await element.selectOption({ label });
  69  |   }
  70  | 
  71  |   async getText(element: Locator): Promise<string> {
  72  |     await expect(element).toBeVisible();
  73  |     return (await element.textContent()) ?? '';
  74  |   }
  75  | 
  76  |   async verifyText(element: Locator, expected: string) {
  77  |     await expect(element).toHaveText(expected);
  78  |   }
  79  | 
  80  |   async verifyContainsText(element: Locator, partial: string) {
  81  |     await expect(element).toContainText(partial);
  82  |   }
  83  | 
  84  |   async verifyValue(element: Locator, expected: string) {
  85  |     await expect(element).toHaveValue(expected);
  86  |   }
  87  | 
  88  |   async verifyCount(element: Locator, expected: number) {
  89  |     await expect(element).toHaveCount(expected);
  90  |   }
  91  | 
  92  |   async verifyAttribute(element: Locator, attributeName: string, expected: string) {
  93  |     await expect(element).toHaveAttribute(attributeName, expected);
  94  |   }
  95  | 
  96  |   async verifyChecked(element: Locator) {
  97  |     await expect(element).toBeChecked();
  98  |   }
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
```