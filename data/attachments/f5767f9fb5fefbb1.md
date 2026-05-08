# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: E2E_Tests/FC005_questionnaire.spec.ts >> FC_005_Questionnaire Flow >> Configure questionnaire with 'External user can finish the questionnaire' and verify 'Lock' action is executed when Question condition is triggered on 'Change a question' and check Questionnaire 'Set version result state to' action
- Location: tests/E2E_Tests/FC005_questionnaire.spec.ts:31:9

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: locator('[data-testid="user-mail"]')
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for locator('[data-testid="user-mail"]')

```

# Test source

```ts
  1   | import { Locator, Page, expect } from '@playwright/test';
  2   | 
  3   | export class UIActions {
  4   |   constructor(private page: Page) { }
  5   | 
  6   |   async click(element: Locator) {
  7   |     await expect(element).toBeVisible();
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
> 28  |     await expect(element).toBeVisible();
      |                           ^ Error: expect(locator).toBeVisible() failed
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
  108 |     await expect(element).toBeVisible();
  109 |   }
  110 | 
  111 |   async verifyNotVisible(element: Locator) {
  112 |     await expect(element).not.toBeVisible();
  113 |   }
  114 | 
  115 |   async verifyHidden(element: Locator) {
  116 |     await expect(element).toBeHidden();
  117 |   }
  118 | 
  119 |   async verifyEnabled(element: Locator) {
  120 |     await expect(element).toBeEnabled();
  121 |   }
  122 | 
  123 |   async verifyDisabled(element: Locator) {
  124 |     await expect(element).toBeDisabled();
  125 |   }
  126 | 
  127 |   async waitForVisible(element: Locator) {
  128 |     await element.waitFor({ state: 'visible' });
```