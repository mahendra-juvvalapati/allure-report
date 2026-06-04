# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: E2E_Tests/FC019_questionnaire.spec.ts >> FC_019_Questionnaire Flow >> Configure questionnaire with 'Inherit Notes and Links' and verify 'Update Current Item' action is executed when Question condition is triggered on 'Entering the questionnaire the first time' and check Questionnaire 'Enable' action
- Location: tests/E2E_Tests/FC019_questionnaire.spec.ts:33:9

# Error details

```
TimeoutError: locator.click: Timeout 15000ms exceeded.
Call log:
  - waiting for getByText('USER Question').last()
    - locator resolved to <span class="ellipsis">(1-1) User Questions</span>
  - attempting click action
    2 × waiting for element to be visible, enabled and stable
      - element is visible, enabled and stable
      - scrolling into view if needed
      - done scrolling
      - <input readonly tabindex="0" role="combobox" aria-readonly="false" aria-expanded="false" aria-autocomplete="none" value="(1-1) User Questions" class="q-select__focus-target" id="f_08e22322-bd6b-45d9-b171-1c5642521955" aria-controls="f_08e22322-bd6b-45d9-b171-1c5642521955_lb"/> intercepts pointer events
    - retrying click action
    - waiting 20ms
    2 × waiting for element to be visible, enabled and stable
      - element is visible, enabled and stable
      - scrolling into view if needed
      - done scrolling
      - <input readonly tabindex="0" role="combobox" aria-readonly="false" aria-expanded="false" aria-autocomplete="none" value="(1-1) User Questions" class="q-select__focus-target" id="f_08e22322-bd6b-45d9-b171-1c5642521955" aria-controls="f_08e22322-bd6b-45d9-b171-1c5642521955_lb"/> intercepts pointer events
    - retrying click action
      - waiting 100ms
    26 × waiting for element to be visible, enabled and stable
       - element is visible, enabled and stable
       - scrolling into view if needed
       - done scrolling
       - <input readonly tabindex="0" role="combobox" aria-readonly="false" aria-expanded="false" aria-autocomplete="none" value="(1-1) User Questions" class="q-select__focus-target" id="f_08e22322-bd6b-45d9-b171-1c5642521955" aria-controls="f_08e22322-bd6b-45d9-b171-1c5642521955_lb"/> intercepts pointer events
     - retrying click action
       - waiting 500ms

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
          - button [ref=e25] [cursor=pointer]:
            - img [ref=e27]:
              - img [ref=e28]
          - generic [ref=e33]:
            - button [ref=e34] [cursor=pointer]:
              - img [ref=e36]:
                - img [ref=e37]
            - status "42" [ref=e38]
          - button "fullscreen" [ref=e39] [cursor=pointer]:
            - generic [ref=e40]: fullscreen
          - button "Open beamer" [ref=e41] [cursor=pointer]:
            - img [ref=e42]:
              - img
            - generic [ref=e43]: "1"
          - button "freshDesk" [ref=e44] [cursor=pointer]:
            - generic [ref=e45]: info
        - generic [ref=e46]:
          - generic [ref=e47]:
            - img [ref=e48] [cursor=pointer]
            - button "dehaze" [ref=e49] [cursor=pointer]:
              - generic [ref=e50]: dehaze
          - list [ref=e51]:
            - generic [ref=e52]:
              - button "profile pic" [ref=e53]
              - generic [ref=e54]: mahendra j
            - button "keyboard_arrow_down mahendra.juvvalapati@qualitlabs.com" [ref=e55] [cursor=pointer]:
              - generic [ref=e56]: keyboard_arrow_down
              - generic [ref=e57]: mahendra.juvvalapati@qualitlabs.com
            - list [ref=e58]:
              - button "exit_to_app Logout" [ref=e59] [cursor=pointer]:
                - generic [ref=e60]: exit_to_app
                - generic [ref=e61]: Logout
          - list [ref=e63]:
            - button "home Dashboard" [ref=e64] [cursor=pointer]:
              - generic [ref=e65]: home
              - generic [ref=e66]: Dashboard
            - button "widgets Modules keyboard_arrow_down" [ref=e67] [cursor=pointer]:
              - generic [ref=e68]: widgets
              - generic [ref=e69]: Modules
              - generic [ref=e70]: keyboard_arrow_down
            - list [ref=e71]:
              - button "Strategy" [ref=e72] [cursor=pointer]:
                - img [ref=e73]:
                  - img
                - generic [ref=e74]: Strategy
              - button "Policy" [ref=e75] [cursor=pointer]:
                - img [ref=e76]:
                  - img
                - generic [ref=e77]: Policy
              - button "Programs" [ref=e78] [cursor=pointer]:
                - img [ref=e79]:
                  - img
                - generic [ref=e80]: Programs
              - button "projects" [ref=e81] [cursor=pointer]:
                - img [ref=e82]:
                  - img
                - generic [ref=e83]: projects
              - button "Dialogues" [ref=e84] [cursor=pointer]:
                - img [ref=e85]:
                  - img
                - generic [ref=e86]: Dialogues
              - button "Objectives" [ref=e87] [cursor=pointer]:
                - img [ref=e88]:
                  - img
                - generic [ref=e89]: Objectives
              - button "Processes" [ref=e90] [cursor=pointer]:
                - img [ref=e91]:
                  - img
                - generic [ref=e92]: Processes
              - button "Process steps" [ref=e93] [cursor=pointer]:
                - img [ref=e94]:
                  - img
                - generic [ref=e95]: Process steps
              - button "Organisation functions" [ref=e96] [cursor=pointer]:
                - img [ref=e97]:
                  - img
                - generic [ref=e98]: Organisation functions
              - button "KSF's - Opportunities" [ref=e99] [cursor=pointer]:
                - img [ref=e100]:
                  - img
                - generic [ref=e101]: KSF's - Opportunities
              - button "Stakeholders" [ref=e102] [cursor=pointer]:
                - img [ref=e103]:
                  - img
                - generic [ref=e104]: Stakeholders
              - button "Causes" [ref=e105] [cursor=pointer]:
                - img [ref=e106]:
                  - img
                - generic [ref=e107]: Causes
              - button "Risks" [ref=e108] [cursor=pointer]:
                - img [ref=e109]:
                  - img
                - generic [ref=e110]: Risks
              - button "Effects" [ref=e111] [cursor=pointer]:
                - img [ref=e112]:
                  - img
                - generic [ref=e113]: Effects
              - button "Opportunities" [ref=e114] [cursor=pointer]:
                - img [ref=e115]:
                  - img
                - generic [ref=e116]: Opportunities
              - button "Standards Frameworks" [ref=e117] [cursor=pointer]:
                - img [ref=e118]:
                  - img
                - generic [ref=e119]: Standards Frameworks
              - button "Laws and regulations" [ref=e120] [cursor=pointer]:
                - img [ref=e121]:
                  - img
                - generic [ref=e122]: Laws and regulations
              - button "Measures" [ref=e123] [cursor=pointer]:
                - img [ref=e124]:
                  - img
                - generic [ref=e125]: Measures
              - button "Assets" [ref=e126] [cursor=pointer]:
                - img [ref=e127]:
                  - img
                - generic [ref=e128]: Assets
              - button "Information systems" [ref=e129] [cursor=pointer]:
                - img [ref=e130]:
                  - img
                - generic [ref=e131]: Information systems
              - button "Processing" [ref=e132] [cursor=pointer]:
                - img [ref=e133]:
                  - img
                - generic [ref=e134]: Processing
              - button "Audits" [ref=e135] [cursor=pointer]:
                - img [ref=e136]:
                  - img
                - generic [ref=e137]: Audits
              - button "Impact Assessments" [ref=e138] [cursor=pointer]:
                - img [ref=e139]:
                  - img
                - generic [ref=e140]: Impact Assessments
              - button "Audit sets" [ref=e141] [cursor=pointer]:
                - img [ref=e142]:
                  - img
                - generic [ref=e143]: Audit sets
              - button "Tests" [ref=e144] [cursor=pointer]:
                - img [ref=e145]:
                  - img
                - generic [ref=e146]: Tests
              - button "Findings" [ref=e147] [cursor=pointer]:
                - img [ref=e148]:
                  - img
                - generic [ref=e149]: Findings
              - button "Problems" [ref=e150] [cursor=pointer]:
                - img [ref=e151]:
                  - img
                - generic [ref=e152]: Problems
              - button "Changes" [ref=e153] [cursor=pointer]:
                - img [ref=e154]:
                  - img
                - generic [ref=e155]: Changes
              - button "Cases" [ref=e156] [cursor=pointer]:
                - img [ref=e157]:
                  - img
                - generic [ref=e158]: Cases
              - button "Tasks" [ref=e159] [cursor=pointer]:
                - img [ref=e160]:
                  - img
                - generic [ref=e161]: Tasks
              - button "Documents" [ref=e162] [cursor=pointer]:
                - img [ref=e163]:
                  - img
                - generic [ref=e164]: Documents
              - button "News items" [ref=e165] [cursor=pointer]:
                - img [ref=e166]:
                  - img
                - generic [ref=e167]: News items
              - button "Related parties" [ref=e168] [cursor=pointer]:
                - img [ref=e169]:
                  - img
                - generic [ref=e170]: Related parties
              - button "Contracts" [ref=e171] [cursor=pointer]:
                - img [ref=e172]:
                  - img
                - generic [ref=e173]: Contracts
              - button "Vendors" [ref=e174] [cursor=pointer]:
                - img [ref=e175]:
                  - img
                - generic [ref=e176]: Vendors
              - button "Arrangements" [ref=e177] [cursor=pointer]:
                - img [ref=e178]:
                  - img
                - generic [ref=e179]: Arrangements
              - button "Insurances" [ref=e180] [cursor=pointer]:
                - img [ref=e181]:
                  - img
                - generic [ref=e182]: Insurances
              - button "Key Figures" [ref=e183] [cursor=pointer]:
                - img [ref=e184]:
                  - img
                - generic [ref=e185]: Key Figures
              - button "Settings" [ref=e186] [cursor=pointer]:
                - img [ref=e187]:
                  - img
                - generic [ref=e188]: Settings
              - button "BCM Activities" [ref=e189] [cursor=pointer]:
                - img [ref=e190]:
                  - img
                - generic [ref=e191]: BCM Activities
              - button "BCM Plans" [ref=e192] [cursor=pointer]:
                - img [ref=e193]:
                  - img
                - generic [ref=e194]: BCM Plans
              - button "Context analysis" [ref=e195] [cursor=pointer]:
                - img [ref=e196]:
                  - img
                - generic [ref=e197]: Context analysis
              - button "Situations" [ref=e198] [cursor=pointer]:
                - img [ref=e199]:
                  - img
                - generic [ref=e200]: Situations
              - button "Planstappen" [ref=e201] [cursor=pointer]:
                - img [ref=e202]:
                  - img
                - generic [ref=e203]: Planstappen
              - button "BOBOC logs" [ref=e204] [cursor=pointer]:
                - img [ref=e205]:
                  - img
                - generic [ref=e206]: BOBOC logs
            - button "build Maintain keyboard_arrow_down" [ref=e207] [cursor=pointer]:
              - generic [ref=e208]: build
              - generic [ref=e209]: Maintain
              - generic [ref=e210]: keyboard_arrow_down
            - list [ref=e211]:
              - button "assignment_turned_in Questionnaires, forms" [ref=e212] [cursor=pointer]:
                - generic [ref=e213]: assignment_turned_in
                - generic [ref=e214]: Questionnaires, forms
              - button "Workflows & conditions" [ref=e215] [cursor=pointer]:
                - img [ref=e216]:
                  - img
                - generic [ref=e217]: Workflows & conditions
          - generic [ref=e220]:
            - button [ref=e221] [cursor=pointer]:
              - generic [ref=e223]:
                - img [ref=e225]
                - generic [ref=e227]: close
            - menu:
              - generic:
                - generic:
                  - generic:
                    - img
      - generic [ref=e231]:
        - generic [ref=e233]:
          - generic [ref=e234]:
            - generic [ref=e236]:
              - button [ref=e238] [cursor=pointer]:
                - img [ref=e240]: arrow_back
              - generic [ref=e242]:
                - generic [ref=e244] [cursor=pointer]: QualiTlabs
                - generic [ref=e246]: keyboard_arrow_right
                - generic [ref=e248] [cursor=pointer]: Templates
                - generic [ref=e250]: keyboard_arrow_right
                - generic [ref=e252] [cursor=pointer]: QA Automation
                - generic [ref=e254]: keyboard_arrow_right
                - generic [ref=e256] [cursor=pointer]: Questionnaires, forms
            - generic [ref=e258]:
              - button [ref=e259] [cursor=pointer]:
                - img [ref=e261]: content_copy
              - button "Publish" [ref=e262] [cursor=pointer]:
                - generic [ref=e263]:
                  - img [ref=e264]: file_upload
                  - generic [ref=e265]: Publish
              - button [ref=e266] [cursor=pointer]:
                - img [ref=e268]: more_vert
          - generic [ref=e269]: Questionnaire_1780565781537
        - generic [ref=e271]:
          - toolbar [ref=e273]:
            - tablist [ref=e274]:
              - generic [ref=e275]:
                - tab "Settings" [ref=e276] [cursor=pointer]:
                  - generic [ref=e278]: Settings
                - tab "Questionnaire" [selected] [ref=e280] [cursor=pointer]:
                  - generic [ref=e282]: Questionnaire
                - tab "QUESTION CONDITIONS" [ref=e284] [cursor=pointer]:
                  - generic [ref=e286]: QUESTION CONDITIONS
                - tab "QUESTIONNAIRE CONDITIONS" [ref=e288] [cursor=pointer]:
                  - generic [ref=e290]: QUESTIONNAIRE CONDITIONS
                - tab "Indicators" [ref=e292] [cursor=pointer]:
                  - generic [ref=e294]: Indicators
          - tabpanel [ref=e298]:
            - tabpanel [ref=e299]:
              - generic [ref=e300]:
                - generic [ref=e302]:
                  - toolbar [ref=e304]:
                    - generic [ref=e309] [cursor=pointer]:
                      - generic [ref=e310]:
                        - generic [ref=e311]:
                          - generic [ref=e312]: (1-1) User Questions
                          - combobox "(1-1) User Questions Selected questionnaire page" [ref=e313]: (1-1) User Questions
                        - generic:
                          - generic: Selected questionnaire page
                      - generic [ref=e315]: arrow_drop_down
                    - button [ref=e316] [cursor=pointer]:
                      - img [ref=e318]: add
                  - generic [ref=e319]:
                    - generic [ref=e320]:
                      - generic [ref=e326]:
                        - textbox "Page Title" [ref=e327]: User Questions
                        - generic: Page Title
                      - checkbox "Disable" [ref=e329] [cursor=pointer]:
                        - img [ref=e332]
                        - generic [ref=e334]: Disable
                    - generic [ref=e336]:
                      - alert [ref=e340]:
                        - button [ref=e342] [cursor=pointer]:
                          - img [ref=e344]: person
                        - generic [ref=e347]: Select your User
                        - generic [ref=e348]:
                          - button [ref=e350] [cursor=pointer]:
                            - img [ref=e352]: check_box
                          - checkbox [checked] [ref=e353] [cursor=pointer]:
                            - img [ref=e356]
                          - button [ref=e358] [cursor=pointer]:
                            - img [ref=e360]: lock_open
                          - button [ref=e361] [cursor=pointer]:
                            - img [ref=e363]: content_copy
                          - button [ref=e364] [cursor=pointer]:
                            - img [ref=e366]: delete
                      - alert [ref=e370]:
                        - button [ref=e372] [cursor=pointer]:
                          - img [ref=e374]: person
                        - generic [ref=e377]: USER Question
                        - generic [ref=e378]:
                          - button [ref=e380] [cursor=pointer]:
                            - img [ref=e382]: check_box
                          - checkbox [checked] [ref=e383] [cursor=pointer]:
                            - img [ref=e386]
                          - button [ref=e388] [cursor=pointer]:
                            - img [ref=e390]: lock_open
                          - button [ref=e391] [cursor=pointer]:
                            - img [ref=e393]: content_copy
                          - button [ref=e394] [cursor=pointer]:
                            - img [ref=e396]: delete
                      - alert [ref=e400]:
                        - button [ref=e402] [cursor=pointer]:
                          - img [ref=e404]: format_color_text
                        - generic [ref=e407]: What is your name?
                        - generic [ref=e408]:
                          - button [ref=e410] [cursor=pointer]:
                            - img [ref=e412]: check_box
                          - checkbox [checked] [ref=e413] [cursor=pointer]:
                            - img [ref=e416]
                          - button [ref=e418] [cursor=pointer]:
                            - img [ref=e420]: lock_open
                          - button [ref=e421] [cursor=pointer]:
                            - img [ref=e423]: content_copy
                          - button [ref=e424] [cursor=pointer]:
                            - img [ref=e426]: delete
                      - alert [ref=e430]:
                        - button [ref=e432] [cursor=pointer]:
                          - img [ref=e434]: person
                        - generic [ref=e437]: Question with standard answer
                        - generic [ref=e438]:
                          - button [ref=e440] [cursor=pointer]:
                            - img [ref=e442]: check_box
                          - checkbox [checked] [ref=e443] [cursor=pointer]:
                            - img [ref=e446]
                          - button [ref=e448] [cursor=pointer]:
                            - img [ref=e450]: lock_open
                          - button [ref=e451] [cursor=pointer]:
                            - img [ref=e453]: content_copy
                          - button [ref=e454] [cursor=pointer]:
                            - img [ref=e456]: delete
                - generic [ref=e458]:
                  - toolbar [ref=e460]:
                    - tablist [ref=e461]:
                      - generic [ref=e462]:
                        - tab "DATA" [selected] [ref=e463] [cursor=pointer]:
                          - generic [ref=e465]: DATA
                        - tab "SELECT" [ref=e467] [cursor=pointer]:
                          - generic [ref=e469]: SELECT
                        - tab "WIDGETS" [ref=e471] [cursor=pointer]:
                          - generic [ref=e473]: WIDGETS
                  - tabpanel [ref=e477]:
                    - tabpanel [ref=e478]:
                      - generic [ref=e479]:
                        - generic [ref=e481]:
                          - button [ref=e482] [cursor=pointer]:
                            - img [ref=e484]: format_color_text
                          - text: text
                        - generic [ref=e486]:
                          - button [ref=e487] [cursor=pointer]:
                            - img [ref=e489]: event
                          - text: Date and / or time
                        - generic [ref=e491]:
                          - button [ref=e492] [cursor=pointer]:
                            - img [ref=e494]: http
                          - text: URL
                        - generic [ref=e496]:
                          - button [ref=e497] [cursor=pointer]:
                            - img [ref=e499]: subtitles
                          - text: Label
                        - generic [ref=e501]:
                          - button [ref=e502] [cursor=pointer]:
                            - img [ref=e504]: person
                          - text: user
                        - generic [ref=e506]:
                          - button [ref=e507] [cursor=pointer]:
                            - img [ref=e509]: email
                          - text: email
  - generic:
    - iframe
```

# Test source

```ts
  1   | import { Locator, Page, expect } from '@playwright/test';
  2   | import fs from 'fs';
  3   | import dayjs from 'dayjs';
  4   | 
  5   | export class UIActions {
  6   |   constructor(private page: Page) { }
  7   | 
  8   |   async click(element: Locator) {
  9   |     await expect(element).toBeVisible();
  10  |     await expect(element).toBeEnabled();
> 11  |     await element.click();
      |                   ^ TimeoutError: locator.click: Timeout 15000ms exceeded.
  12  |   }
  13  | 
  14  |   async doubleClick(element: Locator) {
  15  |     await expect(element).toBeVisible();
  16  |     await element.dblclick();
  17  |   }
  18  | 
  19  |   async rightClick(element: Locator) {
  20  |     await expect(element).toBeVisible();
  21  |     await element.click({ button: 'right' });
  22  |   }
  23  | 
  24  |   async hover(element: Locator) {
  25  |     await expect(element).toBeVisible();
  26  |     await element.hover();
  27  |   }
  28  | 
  29  |   async type(element: Locator, value: string) {
  30  |     await expect(element).toBeVisible();
  31  |     await expect(element).toBeEnabled();
  32  |     await element.clear();
  33  |     await element.fill(value);
  34  |     await expect(element).toHaveValue(value);
  35  |   }
  36  | 
  37  |   async typeWithoutClearing(element: Locator, value: string) {
  38  |     await expect(element).toBeEnabled();
  39  |     await element.type(value);
  40  | 
  41  |     const currentValue = await element.inputValue();
  42  |     expect(currentValue).toContain(value);
  43  |   }
  44  | 
  45  |   async clear(element: Locator) {
  46  |     await expect(element).toBeEnabled();
  47  |     await element.clear();
  48  |     await expect(element).toHaveValue('');
  49  |   }
  50  | 
  51  |   async check(element: Locator) {
  52  |     // await expect(element).toBeVisible();
  53  |     await element.check();
  54  |     await expect(element).toBeChecked();
  55  |   }
  56  | 
  57  |   async uncheck(element: Locator) {
  58  |     await expect(element).toBeVisible();
  59  |     await element.uncheck();
  60  |     await expect(element).not.toBeChecked();
  61  |   }
  62  | 
  63  |   async selectByValue(element: Locator, value: string) {
  64  |     await element.selectOption(value);
  65  |     await expect(element).toHaveValue(value);
  66  |   }
  67  | 
  68  |   async selectByLabel(element: Locator, label: string) {
  69  |     await element.selectOption({ label });
  70  |   }
  71  | 
  72  |   async getText(element: Locator): Promise<string> {
  73  |     await expect(element).toBeVisible();
  74  |     return (await element.textContent()) ?? '';
  75  |   }
  76  | 
  77  |   async verifyText(element: Locator, expected: string) {
  78  |     await expect(element).toHaveText(expected);
  79  |   }
  80  | 
  81  |   async verifyContainsText(element: Locator, partial: string) {
  82  |     await expect(element).toContainText(partial);
  83  |   }
  84  | 
  85  |   async verifyValue(element: Locator, expected: string) {
  86  |     await expect(element).toHaveValue(expected);
  87  |   }
  88  | 
  89  |   async verifyCount(element: Locator, expected: number) {
  90  |     await expect(element).toHaveCount(expected);
  91  |   }
  92  | 
  93  |   async verifyAttribute(element: Locator, attributeName: string, expected: string) {
  94  |     await expect(element).toHaveAttribute(attributeName, expected);
  95  |   }
  96  | 
  97  |   async verifyChecked(element: Locator) {
  98  |     await expect(element).toBeChecked();
  99  |   }
  100 | 
  101 |   async verifyNotChecked(element: Locator) {
  102 |     await expect(element).not.toBeChecked();
  103 |   }
  104 | 
  105 |   async verifyAttached(element: Locator) {
  106 |     await expect(element).toBeAttached();
  107 |   }
  108 | 
  109 |   async verifyVisible(element: Locator) {
  110 |     await expect(element).toBeVisible();
  111 |   }
```