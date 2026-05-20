# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: E2E_Tests/FC019_questionnaire.spec.ts >> FC_019_Questionnaire Flow >> Configure questionnaire with 'Inherit Notes and Links' and verify 'Update Current Item' action is executed when Question condition is triggered on 'Entering the questionnaire the first time' and check Questionnaire 'Enable' action
- Location: tests/E2E_Tests/FC019_questionnaire.spec.ts:33:9

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByRole('tab', { name: 'Dialogue', exact: true })
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for getByRole('tab', { name: 'Dialogue', exact: true })

```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
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
            - status "135" [ref=e42]
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
            - 'button "version: keyboard_arrow_down" [ref=e216] [cursor=pointer]':
              - generic [ref=e217]: "version:"
              - generic [ref=e218]: keyboard_arrow_down
            - generic [ref=e219]:
              - button [ref=e220] [cursor=pointer]:
                - img [ref=e222]:
                  - img [ref=e223]
              - button "Delete" [ref=e224] [cursor=pointer]:
                - img [ref=e225]: delete
              - button "Open phone interactions menu" [ref=e227] [cursor=pointer]:
                - generic [ref=e228]: more_vert
          - text: ▼
        - generic [ref=e229]:
          - generic [ref=e231]:
            - img [ref=e233]:
              - img
            - generic [ref=e234]:
              - generic [ref=e236]: "Risk:"
              - button "Copy item" [ref=e238] [cursor=pointer]:
                - img "copy item" [ref=e239]: file_copy
              - generic [ref=e240]:
                - button "previous item" [disabled] [ref=e241]:
                  - img "previous item" [ref=e242]:
                    - img
                - button "previous item" [disabled] [ref=e243]:
                  - img "previous item" [ref=e244]:
                    - img
          - generic:
            - img:
              - img
  - iframe [ref=e246]:
    - generic [active]:
      - generic:
        - text:  
        - button "Open chat" [ref=f4e1] [cursor=pointer]
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
> 8   |     await expect(element).toBeVisible();
      |                           ^ Error: expect(locator).toBeVisible() failed
  9   |     await expect(element).toBeEnabled();
  10  |     await element.click();
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
```