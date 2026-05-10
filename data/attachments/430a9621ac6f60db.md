# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: questionnaireIndicators.spec.ts >> Indicators Tab Tests >> TC_IN_001-Verify Indicators tab is visible and accessible within questionnaire
- Location: tests/questionnaireIndicators.spec.ts:76:9

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByRole('button', { name: 'Knowledge Database' })
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for getByRole('button', { name: 'Knowledge Database' })

```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
  - text: ×
  - link "ticket or feedback" [ref=e2] [cursor=pointer]:
    - /url: javascript:void(0)
    - img "ticket or feedback" [ref=e3]
  - generic [ref=e12]:
    - generic [ref=e14]:
      - generic [ref=e21]:
        - generic: Qualitlabs
      - generic [ref=e22]:
        - generic [ref=e24]:
          - generic [ref=e26]: Environments
          - button [ref=e29] [cursor=pointer]:
            - img [ref=e31]:
              - img [ref=e32]
        - generic [ref=e34]:
          - generic [ref=e39]:
            - generic [ref=e41]: search
            - textbox [ref=e43]:
              - /placeholder: Type to search
          - generic [ref=e49] [cursor=pointer]:
            - generic [ref=e50]:
              - generic [ref=e51]:
                - generic [ref=e52]: No Group
                - combobox "No Group Group by" [ref=e53]: No Group
              - generic:
                - generic: Group by
            - generic [ref=e55]: arrow_drop_down
    - generic [ref=e58]:
      - button [ref=e59] [cursor=pointer]:
        - img [ref=e61]: add
      - generic [ref=e65]:
        - generic [ref=e66]: Loading...
        - text:  
        - grid [ref=e67]:
          - rowgroup [ref=e68]:
            - row [ref=e69]:
              - columnheader [ref=e70] [cursor=pointer]:
                - text: 
                - generic:    
          - rowgroup [ref=e71]:
            - row "Company name Contact Domain name Status Organization code Country Start date" [ref=e72]:
              - columnheader "Company name" [ref=e73] [cursor=pointer]:
                - generic [ref=e75]: Company name
                - text: 
                - generic:    
              - columnheader "Contact" [ref=e76] [cursor=pointer]:
                - generic [ref=e78]: Contact
                - text: 
                - generic:    
              - columnheader "Domain name" [ref=e79] [cursor=pointer]:
                - generic [ref=e81]: Domain name
                - text: 
                - generic:    
              - columnheader "Status" [ref=e82] [cursor=pointer]:
                - generic [ref=e84]: Status
                - text: 
                - generic:    
              - columnheader "Organization code" [ref=e85] [cursor=pointer]:
                - generic [ref=e87]: Organization code
                - text: 
                - generic:    
              - columnheader "Country" [ref=e88] [cursor=pointer]:
                - generic [ref=e90]: Country
                - text: 
                - generic:    
              - columnheader "Start date" [ref=e91] [cursor=pointer]:
                - generic [ref=e93]: Start date
                - text: 
                - generic:    
          - rowgroup [ref=e94]:
            - row [ref=e95]:
              - gridcell [ref=e96]:
                - img [ref=e99]
          - rowgroup [ref=e100]:
            - row "QualiTlabs Hyd mahendra j qualitlabshyd1.incontrol.zone ACTIVE qualitlabshyd 30-04-2026" [ref=e101]:
              - gridcell "QualiTlabs Hyd" [ref=e102]
              - gridcell "mahendra j" [ref=e103]
              - gridcell "qualitlabshyd1.incontrol.zone" [ref=e104]
              - gridcell "ACTIVE" [ref=e105]
              - gridcell "qualitlabshyd" [ref=e106]
              - gridcell [ref=e107]
              - gridcell "30-04-2026" [ref=e108]:
                - generic [ref=e109]: 30-04-2026
          - rowgroup
          - rowgroup
          - rowgroup
          - rowgroup
        - generic [ref=e114]:
          - tablist [ref=e115]:
            - tab "Visible data" [ref=e116] [cursor=pointer]:
              - generic [ref=e117]: 
              - generic [ref=e118]: Visible data
          - text:     
        - text:    
  - iframe [ref=e120]:
    - generic [active]:
      - generic:
        - text:  
        - button "Open chat" [ref=f4e1] [cursor=pointer]
```

# Test source

```ts
  1   | import { Locator, Page, expect } from '@playwright/test';
  2   | 
  3   | export class UIActions {
  4   |   constructor(private page: Page) { }
  5   | 
  6   |   async click(element: Locator) {
> 7   |     await expect(element).toBeVisible();
      |                           ^ Error: expect(locator).toBeVisible() failed
  8   |     await expect(element).toBeEnabled();
  9   |     await element.click();
  10  |   }
  11  | 
  12  |   async doubleClick(element: Locator) {
  13  |     await expect(element).toBeVisible();
  14  |     await element.dblclick();
  15  |   }
  16  | 
  17  |   async rightClick(element: Locator) {
  18  |     await expect(element).toBeVisible();
  19  |     await element.click({ button: 'right' });
  20  |   }
  21  | 
  22  |   async hover(element: Locator) {
  23  |     await expect(element).toBeVisible();
  24  |     await element.hover();
  25  |   }
  26  | 
  27  |   async type(element: Locator, value: string) {
  28  |     await expect(element).toBeVisible();
  29  |     await expect(element).toBeEnabled();
  30  |     await element.clear();
  31  |     await element.fill(value);
  32  |     await expect(element).toHaveValue(value);
  33  |   }
  34  | 
  35  |   async typeWithoutClearing(element: Locator, value: string) {
  36  |     await expect(element).toBeEnabled();
  37  |     await element.type(value);
  38  | 
  39  |     const currentValue = await element.inputValue();
  40  |     expect(currentValue).toContain(value);
  41  |   }
  42  | 
  43  |   async clear(element: Locator) {
  44  |     await expect(element).toBeEnabled();
  45  |     await element.clear();
  46  |     await expect(element).toHaveValue('');
  47  |   }
  48  | 
  49  |   async check(element: Locator) {
  50  |     // await expect(element).toBeVisible();
  51  |     await element.check();
  52  |     await expect(element).toBeChecked();
  53  |   }
  54  | 
  55  |   async uncheck(element: Locator) {
  56  |     await expect(element).toBeVisible();
  57  |     await element.uncheck();
  58  |     await expect(element).not.toBeChecked();
  59  |   }
  60  | 
  61  |   async selectByValue(element: Locator, value: string) {
  62  |     await element.selectOption(value);
  63  |     await expect(element).toHaveValue(value);
  64  |   }
  65  | 
  66  |   async selectByLabel(element: Locator, label: string) {
  67  |     await element.selectOption({ label });
  68  |   }
  69  | 
  70  |   async getText(element: Locator): Promise<string> {
  71  |     await expect(element).toBeVisible();
  72  |     return (await element.textContent()) ?? '';
  73  |   }
  74  | 
  75  |   async verifyText(element: Locator, expected: string) {
  76  |     await expect(element).toHaveText(expected);
  77  |   }
  78  | 
  79  |   async verifyContainsText(element: Locator, partial: string) {
  80  |     await expect(element).toContainText(partial);
  81  |   }
  82  | 
  83  |   async verifyValue(element: Locator, expected: string) {
  84  |     await expect(element).toHaveValue(expected);
  85  |   }
  86  | 
  87  |   async verifyCount(element: Locator, expected: number) {
  88  |     await expect(element).toHaveCount(expected);
  89  |   }
  90  | 
  91  |   async verifyAttribute(element: Locator, attributeName: string, expected: string) {
  92  |     await expect(element).toHaveAttribute(attributeName, expected);
  93  |   }
  94  | 
  95  |   async verifyChecked(element: Locator) {
  96  |     await expect(element).toBeChecked();
  97  |   }
  98  | 
  99  |   async verifyNotChecked(element: Locator) {
  100 |     await expect(element).not.toBeChecked();
  101 |   }
  102 | 
  103 |   async verifyAttached(element: Locator) {
  104 |     await expect(element).toBeAttached();
  105 |   }
  106 | 
  107 |   async verifyVisible(element: Locator) {
```