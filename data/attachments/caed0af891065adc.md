# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: questionnaireCondition.spec.ts >> Questionnaire Condition Tests >> TC_QNC_001-Verify a new condition tab can be created with name and description in questionnaire conditions
- Location: tests/questionnaireCondition.spec.ts:77:9

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByRole('gridcell', { name: 'QA Automation' })
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for getByRole('gridcell', { name: 'QA Automation' })

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
          - button [ref=e29] [cursor=pointer]:
            - img [ref=e31]:
              - img [ref=e32]
          - button "fullscreen" [ref=e33] [cursor=pointer]:
            - generic [ref=e34]: fullscreen
          - button "Open beamer" [ref=e35] [cursor=pointer]:
            - img [ref=e36]:
              - img
            - generic [ref=e37]: "1"
          - button "freshDesk" [ref=e38] [cursor=pointer]:
            - generic [ref=e39]: info
        - generic [ref=e40]:
          - generic [ref=e41]:
            - img [ref=e42] [cursor=pointer]
            - button "dehaze" [ref=e43] [cursor=pointer]:
              - generic [ref=e44]: dehaze
          - list [ref=e45]:
            - generic [ref=e46]:
              - button "profile pic" [ref=e47]
              - generic [ref=e48]: mahendra j
            - button "keyboard_arrow_down mahendra.juvvalapati@qualitlabs.com" [ref=e49] [cursor=pointer]:
              - generic [ref=e50]: keyboard_arrow_down
              - generic [ref=e51]: mahendra.juvvalapati@qualitlabs.com
            - list [ref=e52]:
              - button "account_box My Data" [ref=e53] [cursor=pointer]:
                - generic [ref=e54]: account_box
                - generic [ref=e55]: My Data
              - button "settings Settings" [ref=e56] [cursor=pointer]:
                - generic [ref=e57]: settings
                - generic [ref=e58]: Settings
              - button "exit_to_app Logout" [ref=e59] [cursor=pointer]:
                - generic [ref=e60]: exit_to_app
                - generic [ref=e61]: Logout
          - list [ref=e63]:
            - button "Add new user" [ref=e64] [cursor=pointer]:
              - img [ref=e65]:
                - img
              - generic [ref=e66]: Add new user
            - button "business Environments" [ref=e67] [cursor=pointer]:
              - generic [ref=e68]: business
              - generic [ref=e69]: Environments
            - button "Knowledge Database" [ref=e70] [cursor=pointer]:
              - img [ref=e71]:
                - img
              - generic [ref=e72]: Knowledge Database
      - generic [ref=e77]:
        - generic [ref=e79]:
          - generic [ref=e86]:
            - generic: Qualitlabs
          - generic [ref=e87]:
            - generic [ref=e89]:
              - generic [ref=e91]: Environments
              - button [ref=e94] [cursor=pointer]:
                - img [ref=e96]:
                  - img [ref=e97]
            - generic [ref=e99]:
              - generic [ref=e104]:
                - generic [ref=e106]: search
                - textbox [ref=e108]:
                  - /placeholder: Type to search
              - generic [ref=e114] [cursor=pointer]:
                - generic [ref=e115]:
                  - generic [ref=e116]:
                    - generic [ref=e117]: No Group
                    - combobox "No Group Group by" [ref=e118]: No Group
                  - generic:
                    - generic: Group by
                - generic [ref=e120]: arrow_drop_down
        - generic [ref=e123]:
          - button [ref=e124] [cursor=pointer]:
            - img [ref=e126]: add
          - generic [ref=e130]:
            - generic [ref=e131]: Loading...
            - text:  
            - grid [ref=e132]:
              - rowgroup [ref=e133]:
                - row [ref=e134]:
                  - columnheader [ref=e135] [cursor=pointer]:
                    - text: 
                    - generic:    
              - rowgroup [ref=e136]:
                - row "Company name Contact Domain name Status Organization code Country Start date" [ref=e137]:
                  - columnheader "Company name" [ref=e138] [cursor=pointer]:
                    - generic [ref=e140]: Company name
                    - text: 
                    - generic:    
                  - columnheader "Contact" [ref=e141] [cursor=pointer]:
                    - generic [ref=e143]: Contact
                    - text: 
                    - generic:    
                  - columnheader "Domain name" [ref=e144] [cursor=pointer]:
                    - generic [ref=e146]: Domain name
                    - text: 
                    - generic:    
                  - columnheader "Status" [ref=e147] [cursor=pointer]:
                    - generic [ref=e149]: Status
                    - text: 
                    - generic:    
                  - columnheader "Organization code" [ref=e150] [cursor=pointer]:
                    - generic [ref=e152]: Organization code
                    - text: 
                    - generic:    
                  - columnheader "Country" [ref=e153] [cursor=pointer]:
                    - generic [ref=e155]: Country
                    - text: 
                    - generic:    
                  - columnheader "Start date" [ref=e156] [cursor=pointer]:
                    - generic [ref=e158]: Start date
                    - text: 
                    - generic:    
              - rowgroup [ref=e159]
              - rowgroup [ref=e160]
              - rowgroup
              - rowgroup
              - rowgroup
              - rowgroup
              - generic [ref=e165]: Loading...
            - generic [ref=e166]:
              - tablist [ref=e167]:
                - tab "Visible data" [ref=e168] [cursor=pointer]:
                  - generic [ref=e169]: 
                  - generic [ref=e170]: Visible data
              - text:     
            - text:    
  - iframe [ref=e172]:
    - generic [active]:
      - generic:
        - text:  
        - button "Open chat" [ref=f4e1] [cursor=pointer]
  - generic [ref=e173]:
    - generic [ref=e174]: Aankondiging
    - generic [ref=e175]: Release notes mei 2026 week 22
    - img [ref=e176]
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