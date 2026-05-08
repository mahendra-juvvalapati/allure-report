# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: E2E_Tests/FC011_questionnaire.spec.ts >> FC_011_Questionnaire Flow >> Configure questionnaire with 'Disable opener for question' and verify 'Calculate all linked kpis' action is executed when Question condition is triggered on 'Change a question' and check Questionnaire 'Calculate all linktab kpis' action
- Location: tests/E2E_Tests/FC011_questionnaire.spec.ts:38:9

# Error details

```
TimeoutError: locator.check: Timeout 15000ms exceeded.
Call log:
  - waiting for getByTestId('isOpenerDisabled')

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
        - img [ref=e17]
        - button "Turn off admin role" [ref=e20] [cursor=pointer]:
          - img [ref=e21]:
            - img
        - button [ref=e23] [cursor=pointer]:
          - img [ref=e25]:
            - img [ref=e26]
        - generic [ref=e31]:
          - button [ref=e32] [cursor=pointer]:
            - img [ref=e34]:
              - img [ref=e35]
          - status "47" [ref=e36]
        - button "fullscreen" [ref=e37] [cursor=pointer]:
          - generic [ref=e38]: fullscreen
        - button "Open beamer" [ref=e39] [cursor=pointer]:
          - img [ref=e40]:
            - img
          - generic [ref=e41]: "1"
        - button "freshDesk" [ref=e42] [cursor=pointer]:
          - generic [ref=e43]: info
      - generic [ref=e44]:
        - generic [ref=e45]:
          - img [ref=e46] [cursor=pointer]
          - button "dehaze" [ref=e47] [cursor=pointer]:
            - generic [ref=e48]: dehaze
        - list [ref=e49]:
          - generic [ref=e50]:
            - button "profile pic" [ref=e51]
            - generic [ref=e52]: mahendra j
          - button "keyboard_arrow_down mahendra.juvvalapati@qualitlabs.com" [ref=e53] [cursor=pointer]:
            - generic [ref=e54]: keyboard_arrow_down
            - generic [ref=e55]: mahendra.juvvalapati@qualitlabs.com
          - list [ref=e56]:
            - button "exit_to_app Logout" [ref=e57] [cursor=pointer]:
              - generic [ref=e58]: exit_to_app
              - generic [ref=e59]: Logout
        - list [ref=e61]:
          - button "home Dashboard" [ref=e62] [cursor=pointer]:
            - generic [ref=e63]: home
            - generic [ref=e64]: Dashboard
          - button "widgets Modules keyboard_arrow_down" [ref=e65] [cursor=pointer]:
            - generic [ref=e66]: widgets
            - generic [ref=e67]: Modules
            - generic [ref=e68]: keyboard_arrow_down
          - list [ref=e69]:
            - button "Strategy" [ref=e70] [cursor=pointer]:
              - img [ref=e71]:
                - img
              - generic [ref=e72]: Strategy
            - button "Policy" [ref=e73] [cursor=pointer]:
              - img [ref=e74]:
                - img
              - generic [ref=e75]: Policy
            - button "Programs" [ref=e76] [cursor=pointer]:
              - img [ref=e77]:
                - img
              - generic [ref=e78]: Programs
            - button "projects" [ref=e79] [cursor=pointer]:
              - img [ref=e80]:
                - img
              - generic [ref=e81]: projects
            - button "Dialogues" [ref=e82] [cursor=pointer]:
              - img [ref=e83]:
                - img
              - generic [ref=e84]: Dialogues
            - button "Objectives" [ref=e85] [cursor=pointer]:
              - img [ref=e86]:
                - img
              - generic [ref=e87]: Objectives
            - button "Processes" [ref=e88] [cursor=pointer]:
              - img [ref=e89]:
                - img
              - generic [ref=e90]: Processes
            - button "Process steps" [ref=e91] [cursor=pointer]:
              - img [ref=e92]:
                - img
              - generic [ref=e93]: Process steps
            - button "Organisation functions" [ref=e94] [cursor=pointer]:
              - img [ref=e95]:
                - img
              - generic [ref=e96]: Organisation functions
            - button "KSF's - Opportunities" [ref=e97] [cursor=pointer]:
              - img [ref=e98]:
                - img
              - generic [ref=e99]: KSF's - Opportunities
            - button "Stakeholders" [ref=e100] [cursor=pointer]:
              - img [ref=e101]:
                - img
              - generic [ref=e102]: Stakeholders
            - button "Causes" [ref=e103] [cursor=pointer]:
              - img [ref=e104]:
                - img
              - generic [ref=e105]: Causes
            - button "Risks" [ref=e106] [cursor=pointer]:
              - img [ref=e107]:
                - img
              - generic [ref=e108]: Risks
            - button "Effects" [ref=e109] [cursor=pointer]:
              - img [ref=e110]:
                - img
              - generic [ref=e111]: Effects
            - button "Opportunities" [ref=e112] [cursor=pointer]:
              - img [ref=e113]:
                - img
              - generic [ref=e114]: Opportunities
            - button "Standards Frameworks" [ref=e115] [cursor=pointer]:
              - img [ref=e116]:
                - img
              - generic [ref=e117]: Standards Frameworks
            - button "Laws and regulations" [ref=e118] [cursor=pointer]:
              - img [ref=e119]:
                - img
              - generic [ref=e120]: Laws and regulations
            - button "Measures" [ref=e121] [cursor=pointer]:
              - img [ref=e122]:
                - img
              - generic [ref=e123]: Measures
            - button "Assets" [ref=e124] [cursor=pointer]:
              - img [ref=e125]:
                - img
              - generic [ref=e126]: Assets
            - button "Information systems" [ref=e127] [cursor=pointer]:
              - img [ref=e128]:
                - img
              - generic [ref=e129]: Information systems
            - button "Processing" [ref=e130] [cursor=pointer]:
              - img [ref=e131]:
                - img
              - generic [ref=e132]: Processing
            - button "Audits" [ref=e133] [cursor=pointer]:
              - img [ref=e134]:
                - img
              - generic [ref=e135]: Audits
            - button "Audit sets" [ref=e136] [cursor=pointer]:
              - img [ref=e137]:
                - img
              - generic [ref=e138]: Audit sets
            - button "Impact Assessments" [ref=e139] [cursor=pointer]:
              - img [ref=e140]:
                - img
              - generic [ref=e141]: Impact Assessments
            - button "Tests" [ref=e142] [cursor=pointer]:
              - img [ref=e143]:
                - img
              - generic [ref=e144]: Tests
            - button "Findings" [ref=e145] [cursor=pointer]:
              - img [ref=e146]:
                - img
              - generic [ref=e147]: Findings
            - button "Problems" [ref=e148] [cursor=pointer]:
              - img [ref=e149]:
                - img
              - generic [ref=e150]: Problems
            - button "Changes" [ref=e151] [cursor=pointer]:
              - img [ref=e152]:
                - img
              - generic [ref=e153]: Changes
            - button "Cases" [ref=e154] [cursor=pointer]:
              - img [ref=e155]:
                - img
              - generic [ref=e156]: Cases
            - button "Tasks" [ref=e157] [cursor=pointer]:
              - img [ref=e158]:
                - img
              - generic [ref=e159]: Tasks
            - button "Documents" [ref=e160] [cursor=pointer]:
              - img [ref=e161]:
                - img
              - generic [ref=e162]: Documents
            - button "News items" [ref=e163] [cursor=pointer]:
              - img [ref=e164]:
                - img
              - generic [ref=e165]: News items
            - button "Related parties" [ref=e166] [cursor=pointer]:
              - img [ref=e167]:
                - img
              - generic [ref=e168]: Related parties
            - button "Contracts" [ref=e169] [cursor=pointer]:
              - img [ref=e170]:
                - img
              - generic [ref=e171]: Contracts
            - button "Vendors" [ref=e172] [cursor=pointer]:
              - img [ref=e173]:
                - img
              - generic [ref=e174]: Vendors
            - button "Performance agreements" [ref=e175] [cursor=pointer]:
              - img [ref=e176]:
                - img
              - generic [ref=e177]: Performance agreements
            - button "Key Figures" [ref=e178] [cursor=pointer]:
              - img [ref=e179]:
                - img
              - generic [ref=e180]: Key Figures
            - button "Settings" [ref=e181] [cursor=pointer]:
              - img [ref=e182]:
                - img
              - generic [ref=e183]: Settings
            - button "Critical Business Scenarios" [ref=e184] [cursor=pointer]:
              - img [ref=e185]:
                - img
              - generic [ref=e186]: Critical Business Scenarios
            - button "BCM Plans" [ref=e187] [cursor=pointer]:
              - img [ref=e188]:
                - img
              - generic [ref=e189]: BCM Plans
            - button "Context analysis" [ref=e190] [cursor=pointer]:
              - img [ref=e191]:
                - img
              - generic [ref=e192]: Context analysis
            - button "Situations" [ref=e193] [cursor=pointer]:
              - img [ref=e194]:
                - img
              - generic [ref=e195]: Situations
            - button "Planstappen" [ref=e196] [cursor=pointer]:
              - img [ref=e197]:
                - img
              - generic [ref=e198]: Planstappen
            - button "BOBOC logs" [ref=e199] [cursor=pointer]:
              - img [ref=e200]:
                - img
              - generic [ref=e201]: BOBOC logs
          - button "build Maintain keyboard_arrow_down" [ref=e202] [cursor=pointer]:
            - generic [ref=e203]: build
            - generic [ref=e204]: Maintain
            - generic [ref=e205]: keyboard_arrow_down
          - list [ref=e206]:
            - button "assignment_turned_in Questionnaires, forms" [ref=e207] [cursor=pointer]:
              - generic [ref=e208]: assignment_turned_in
              - generic [ref=e209]: Questionnaires, forms
            - button "Workflows & conditions" [ref=e210] [cursor=pointer]:
              - img [ref=e211]:
                - img
              - generic [ref=e212]: Workflows & conditions
    - generic [ref=e217]:
      - generic [ref=e219]:
        - generic [ref=e225]:
          - generic [ref=e227] [cursor=pointer]: Qualitlabs
          - generic [ref=e229]: keyboard_arrow_right
          - generic [ref=e231] [cursor=pointer]: Knowledge database
          - generic [ref=e233]: keyboard_arrow_right
          - generic [ref=e235] [cursor=pointer]: Qa automation
        - generic [ref=e236]:
          - generic [ref=e238]:
            - generic [ref=e240]: Questionnaire
            - generic [ref=e241]:
              - button [ref=e243] [cursor=pointer]:
                - img [ref=e245]: more_vert
              - button [ref=e247] [cursor=pointer]:
                - img [ref=e249]:
                  - img [ref=e250]
          - generic [ref=e252]:
            - generic [ref=e257]:
              - generic [ref=e259]: search
              - textbox [ref=e261]:
                - /placeholder: Type to search
            - generic [ref=e262]:
              - generic [ref=e267] [cursor=pointer]:
                - generic [ref=e268]:
                  - generic [ref=e269]:
                    - generic [ref=e270]: No Group
                    - combobox "No Group Group by" [ref=e271]: No Group
                  - generic:
                    - generic: Group by
                - generic [ref=e273]: arrow_drop_down
              - button [ref=e275] [cursor=pointer]:
                - img [ref=e277]:
                  - img [ref=e278]
      - generic [ref=e281]:
        - button [ref=e282] [cursor=pointer]:
          - img [ref=e284]: add
        - generic [ref=e288]:
          - generic [ref=e289]: Loading...
          - text:  
          - grid [ref=e290]:
            - rowgroup [ref=e291]:
              - row "Type Status Code Questionnaire name Owner Publish status" [ref=e292]:
                - columnheader "Type" [ref=e293] [cursor=pointer]:
                  - generic [ref=e295]: Type
                  - text: 
                  - generic:    
                - columnheader "Status" [ref=e296] [cursor=pointer]:
                  - generic [ref=e298]: Status
                  - text: 
                  - generic:    
                - columnheader "Code" [ref=e299] [cursor=pointer]:
                  - generic [ref=e301]: Code
                  - text: 
                  - generic:    
                - columnheader "Questionnaire name" [ref=e302] [cursor=pointer]:
                  - generic [ref=e304]: Questionnaire name
                  - text: 
                  - generic [ref=e305]:
                    - text: 
                    - generic [ref=e306]: 
                    - text:  
                - columnheader "Owner" [ref=e307] [cursor=pointer]:
                  - generic [ref=e309]: Owner
                  - text: 
                  - generic:    
                - columnheader "Publish status" [ref=e310] [cursor=pointer]:
                  - generic [ref=e312]: Publish status
                  - text: 
                  - generic:    
            - rowgroup [ref=e313]:
              - row "Single active matrix questionnaire_matrix anusha Unpublished" [ref=e314]:
                - gridcell "Single" [ref=e315]
                - gridcell "active" [ref=e316]
                - gridcell "matrix" [ref=e317]
                - gridcell "questionnaire_matrix" [ref=e318]
                - gridcell "anusha" [ref=e319]
                - gridcell "Unpublished" [ref=e320]
              - row "Single active questionnaire_file/picture questionnaire_file/picture anusha Published" [ref=e321]:
                - gridcell "Single" [ref=e322]
                - gridcell "active" [ref=e323]
                - gridcell "questionnaire_file/picture" [ref=e324]
                - gridcell "questionnaire_file/picture" [ref=e325]
                - gridcell "anusha" [ref=e326]
                - gridcell "Published" [ref=e327]
              - row "Single active code 2 questionnaire_email_conditions anusha Unpublished" [ref=e328]:
                - gridcell "Single" [ref=e329]
                - gridcell "active" [ref=e330]
                - gridcell "code 2" [ref=e331]
                - gridcell "questionnaire_email_conditions" [ref=e332]
                - gridcell "anusha" [ref=e333]
                - gridcell "Unpublished" [ref=e334]
              - row "Single active code 1 questionnaire_email anusha Published" [ref=e335]:
                - gridcell "Single" [ref=e336]
                - gridcell "active" [ref=e337]
                - gridcell "code 1" [ref=e338]
                - gridcell "questionnaire_email" [ref=e339]
                - gridcell "anusha" [ref=e340]
                - gridcell "Published" [ref=e341]
              - row "Single active code questionnaire_attributes anusha Published" [ref=e342]:
                - gridcell "Single" [ref=e343]
                - gridcell "active" [ref=e344]
                - gridcell "code" [ref=e345]
                - gridcell "questionnaire_attributes" [ref=e346]
                - gridcell "anusha" [ref=e347]
                - gridcell "Published" [ref=e348]
              - row "Single active send email questionnaire send email anusha Unpublished" [ref=e349]:
                - gridcell "Single" [ref=e350]
                - gridcell "active" [ref=e351]
                - gridcell "send email" [ref=e352]
                - gridcell "questionnaire send email" [ref=e353]
                - gridcell "anusha" [ref=e354]
                - gridcell "Unpublished" [ref=e355]
              - row "Single active code jsjdkjs mahendra Published" [ref=e356]:
                - gridcell "Single" [ref=e357]
                - gridcell "active" [ref=e358]
                - gridcell "code" [ref=e359]
                - gridcell "jsjdkjs" [ref=e360]
                - gridcell "mahendra" [ref=e361]
                - gridcell "Published" [ref=e362]
              - row "Single active IA1 import action Priyanka Published" [ref=e363]:
                - gridcell "Single" [ref=e364]
                - gridcell "active" [ref=e365]
                - gridcell "IA1" [ref=e366]
                - gridcell "import action" [ref=e367]
                - gridcell "Priyanka" [ref=e368]
                - gridcell "Published" [ref=e369]
              - row "Single active Coe Today mahendra Published" [ref=e370]:
                - gridcell "Single" [ref=e371]
                - gridcell "active" [ref=e372]
                - gridcell "Coe" [ref=e373]
                - gridcell "Today" [ref=e374]
                - gridcell "mahendra" [ref=e375]
                - gridcell "Published" [ref=e376]
              - row "Survey active S1 Survey_1778247532305 mahendra Unpublished" [ref=e377]:
                - gridcell "Survey" [ref=e378]
                - gridcell "active" [ref=e379]
                - gridcell "S1" [ref=e380]
                - gridcell "Survey_1778247532305" [ref=e381]
                - gridcell "mahendra" [ref=e382]
                - gridcell "Unpublished" [ref=e383]
              - row "Survey active S1 Survey_1778242554089 mahendra Unpublished" [ref=e384]:
                - gridcell "Survey" [ref=e385]
                - gridcell "active" [ref=e386]
                - gridcell "S1" [ref=e387]
                - gridcell "Survey_1778242554089" [ref=e388]
                - gridcell "mahendra" [ref=e389]
                - gridcell "Unpublished" [ref=e390]
              - row "Survey active S1 Survey_1778220893264 mahendra Unpublished" [ref=e391]:
                - gridcell "Survey" [ref=e392]
                - gridcell "active" [ref=e393]
                - gridcell "S1" [ref=e394]
                - gridcell "Survey_1778220893264" [ref=e395]
                - gridcell "mahendra" [ref=e396]
                - gridcell "Unpublished" [ref=e397]
              - row "Survey active S1 Survey_1778217560160 mahendra Unpublished" [ref=e398]:
                - gridcell "Survey" [ref=e399]
                - gridcell "active" [ref=e400]
                - gridcell "S1" [ref=e401]
                - gridcell "Survey_1778217560160" [ref=e402]
                - gridcell "mahendra" [ref=e403]
                - gridcell "Unpublished" [ref=e404]
              - row "Survey active S1 Survey_1778181953957 mahendra Unpublished" [ref=e405]:
                - gridcell "Survey" [ref=e406]
                - gridcell "active" [ref=e407]
                - gridcell "S1" [ref=e408]
                - gridcell "Survey_1778181953957" [ref=e409]
                - gridcell "mahendra" [ref=e410]
                - gridcell "Unpublished" [ref=e411]
              - row "Survey active S1 Survey_1778177916383 mahendra Unpublished" [ref=e412]:
                - gridcell "Survey" [ref=e413]
                - gridcell "active" [ref=e414]
                - gridcell "S1" [ref=e415]
                - gridcell "Survey_1778177916383" [ref=e416]
                - gridcell "mahendra" [ref=e417]
                - gridcell "Unpublished" [ref=e418]
              - row "Survey active S1 Survey_1778169109046 mahendra Unpublished" [ref=e419]:
                - gridcell "Survey" [ref=e420]
                - gridcell "active" [ref=e421]
                - gridcell "S1" [ref=e422]
                - gridcell "Survey_1778169109046" [ref=e423]
                - gridcell "mahendra" [ref=e424]
                - gridcell "Unpublished" [ref=e425]
              - row "Survey active S1 Survey_1778162682648 mahendra Unpublished" [ref=e426]:
                - gridcell "Survey" [ref=e427]
                - gridcell "active" [ref=e428]
                - gridcell "S1" [ref=e429]
                - gridcell "Survey_1778162682648" [ref=e430]
                - gridcell "mahendra" [ref=e431]
                - gridcell "Unpublished" [ref=e432]
              - row "Survey active S1 Survey_1778157496659 mahendra Unpublished" [ref=e433]:
                - gridcell "Survey" [ref=e434]
                - gridcell "active" [ref=e435]
                - gridcell "S1" [ref=e436]
                - gridcell "Survey_1778157496659" [ref=e437]
                - gridcell "mahendra" [ref=e438]
                - gridcell "Unpublished" [ref=e439]
              - row "Survey active S1 Survey_1778144373227 mahendra Unpublished" [ref=e440]:
                - gridcell "Survey" [ref=e441]
                - gridcell "active" [ref=e442]
                - gridcell "S1" [ref=e443]
                - gridcell "Survey_1778144373227" [ref=e444]
                - gridcell "mahendra" [ref=e445]
                - gridcell "Unpublished" [ref=e446]
            - rowgroup
            - rowgroup
            - rowgroup
          - generic [ref=e453]:
            - tablist [ref=e454]:
              - tab "Visible data" [ref=e455] [cursor=pointer]:
                - generic [ref=e456]: 
                - generic [ref=e457]: Visible data
            - text:     
          - text:    
  - iframe [ref=e459]:
    - generic [active]:
      - generic:
        - text:  
        - button "Open chat" [ref=f6e1] [cursor=pointer]
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
> 51  |     await element.check();
      |                   ^ TimeoutError: locator.check: Timeout 15000ms exceeded.
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
  129 |   }
  130 | 
  131 |   async waitForHidden(element: Locator) {
  132 |     await element.waitFor({ state: 'hidden' });
  133 |   }
  134 | 
  135 |   async waitForURL(url: RegExp | string) {
  136 |     await this.page.waitForURL(url);
  137 |   }
  138 | 
  139 |   async waitForLoad() {
  140 |     await this.page.waitForLoadState('load');
  141 |   }
  142 | 
  143 |   async scrollIntoView(element: Locator) {
  144 |     await element.scrollIntoViewIfNeeded();
  145 |   }
  146 | 
  147 |   async pressKey(element: Locator, key: string) {
  148 |     await element.press(key);
  149 |   }
  150 | 
  151 |   async pressOnPage(key: string) {
```