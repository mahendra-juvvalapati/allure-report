# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: E2E_Tests/FC013_questionnaire.spec.ts >> FC_013_Questionnaire Flow >> Configure questionnaire with 'No Settings' and verify 'Set item state to' action is executed when Question condition is triggered on 'Entering the questionnaire the first time' and check Questionnaire 'Generate report and send to service' action
- Location: tests/E2E_Tests/FC013_questionnaire.spec.ts:37:9

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByRole('button', { name: 'build Maintain' })
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for getByRole('button', { name: 'build Maintain' })

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
          - button "Turn off admin role" [ref=e22] [cursor=pointer]:
            - img [ref=e23]:
              - img
          - generic [ref=e28]:
            - button [ref=e29] [cursor=pointer]:
              - img [ref=e31]:
                - img [ref=e32]
            - status "27" [ref=e33]
          - button "fullscreen" [ref=e34] [cursor=pointer]:
            - generic [ref=e35]: fullscreen
          - button "Open beamer" [ref=e36] [cursor=pointer]:
            - img [ref=e37]:
              - img
            - generic [ref=e38]: "1"
          - button "freshDesk" [ref=e39] [cursor=pointer]:
            - generic [ref=e40]: info
        - generic [ref=e41]:
          - generic [ref=e42]:
            - img [ref=e43] [cursor=pointer]
            - button "dehaze" [ref=e44] [cursor=pointer]:
              - generic [ref=e45]: dehaze
          - list [ref=e46]:
            - generic [ref=e47]:
              - button "profile pic" [ref=e48]
              - generic [ref=e49]: mahendra j
            - button "keyboard_arrow_down mahendra.juvvalapati@qualitlabs.com" [ref=e50] [cursor=pointer]:
              - generic [ref=e51]: keyboard_arrow_down
              - generic [ref=e52]: mahendra.juvvalapati@qualitlabs.com
            - list [ref=e53]:
              - button "account_box My Data" [ref=e54] [cursor=pointer]:
                - generic [ref=e55]: account_box
                - generic [ref=e56]: My Data
              - button "settings Settings" [ref=e57] [cursor=pointer]:
                - generic [ref=e58]: settings
                - generic [ref=e59]: Settings
              - button "exit_to_app Logout" [ref=e60] [cursor=pointer]:
                - generic [ref=e61]: exit_to_app
                - generic [ref=e62]: Logout
          - list [ref=e64]:
            - button "Add new user" [ref=e65] [cursor=pointer]:
              - img [ref=e66]:
                - img
              - generic [ref=e67]: Add new user
            - button "business Environments" [ref=e68] [cursor=pointer]:
              - generic [ref=e69]: business
              - generic [ref=e70]: Environments
            - button "Knowledge Database" [ref=e71] [cursor=pointer]:
              - img [ref=e72]:
                - img
              - generic [ref=e73]: Knowledge Database
      - generic [ref=e78]:
        - generic [ref=e80]:
          - generic [ref=e88] [cursor=pointer]: Qualitlabs
          - generic [ref=e89]:
            - generic [ref=e91]:
              - generic [ref=e93]: Knowledge Database
              - button [ref=e96] [cursor=pointer]:
                - img [ref=e98]:
                  - img [ref=e99]
            - generic [ref=e101]:
              - generic [ref=e106]:
                - generic [ref=e108]: search
                - textbox [ref=e110]:
                  - /placeholder: Type to search
              - generic [ref=e116] [cursor=pointer]:
                - generic [ref=e117]:
                  - generic [ref=e118]:
                    - generic [ref=e119]: No Group
                    - combobox "No Group Group by" [ref=e120]: No Group
                  - generic:
                    - generic: Group by
                - generic [ref=e122]: arrow_drop_down
        - generic [ref=e125]:
          - button [ref=e126] [cursor=pointer]:
            - img [ref=e128]: add
          - generic [ref=e132]:
            - generic [ref=e133]: Loading...
            - text:  
            - grid [ref=e134]:
              - rowgroup [ref=e135]:
                - row "Company name Status" [ref=e136]:
                  - columnheader "Company name" [ref=e137] [cursor=pointer]:
                    - generic [ref=e139]: Company name
                    - text: 
                    - generic:    
                  - columnheader "Status" [ref=e140] [cursor=pointer]:
                    - generic [ref=e142]: Status
                    - text: 
                    - generic:    
              - rowgroup [ref=e143]:
                - row "QA Automation ACTIVE" [ref=e144]:
                  - gridcell "QA Automation" [ref=e145]
                  - gridcell "ACTIVE" [ref=e146]
              - rowgroup
              - rowgroup
              - rowgroup
            - text:    
  - iframe [ref=e148]:
    - generic [active]:
      - generic:
        - text:  
        - button "Open chat" [ref=f4e1] [cursor=pointer]
  - generic [ref=e149]:
    - generic [ref=e150]: weetje
    - generic [ref=e151]: Gebruikerstatus en datum laatste status zichtbaar
    - img [ref=e152]
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