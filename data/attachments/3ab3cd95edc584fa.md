# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: E2E_Tests/FC021_questionnaire.spec.ts >> FC_021_Questionnaire Flow >> Configure questionnaire with 'Add documents as evidence' and verify 'Show' action is executed when Question condition is triggered on 'Completing the page' and check Questionnaire 'Set Value to Variable' action
- Location: tests/E2E_Tests/FC021_questionnaire.spec.ts:31:9

# Error details

```
Test timeout of 600000ms exceeded.
```

```
Error: expect(locator).toBeEnabled() failed

Locator:  getByRole('img', { name: 'quick-version' }).last()
Expected: enabled
Received: undefined

Call log:
  - Expect "toBeEnabled" with timeout 15000ms
  - waiting for getByRole('img', { name: 'quick-version' }).last()

```

# Page snapshot

```yaml
- generic [ref=e1]:
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
            - status "65" [ref=e44]
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
      - generic [ref=e212]:
        - generic [ref=e214]:
          - generic [ref=e215]:
            - generic [ref=e217]:
              - generic [ref=e218] [cursor=pointer]:
                - generic: apps
                - generic:
                  - img
              - list [ref=e219]:
                - listitem [ref=e220]:
                  - generic [ref=e222]:
                    - generic:
                      - img
                    - generic [ref=e223]: Risk
            - 'button "version:No repeatplan - 1 Version name keyboard_arrow_down Executor: ALL" [ref=e226] [cursor=pointer]':
              - generic [ref=e227]: version:No repeatplan - 1 Version name
              - generic [ref=e228]: keyboard_arrow_down
              - generic [ref=e229]: "Executor: ALL"
            - button "settings" [ref=e231] [cursor=pointer]:
              - img [ref=e232]: settings
            - generic [ref=e233]:
              - button "add mo to projects" [ref=e235] [cursor=pointer]:
                - img [ref=e236]:
                  - img
              - button [ref=e237] [cursor=pointer]:
                - img [ref=e239]:
                  - img [ref=e240]
          - text: ▼ ▼
        - generic [ref=e241]:
          - generic [ref=e243]:
            - img [ref=e245]:
              - img
            - generic [ref=e246]:
              - generic [ref=e248]: "Risk: Risk_1779786115563"
              - button "Copy item" [ref=e250] [cursor=pointer]:
                - img "copy item" [ref=e251]: file_copy
              - button "Close current version and start new version" [ref=e252] [cursor=pointer]:
                - img "quick-version" [ref=e253]:
                  - img
              - generic [ref=e254]:
                - button "previous item" [disabled] [ref=e255]:
                  - img "previous item" [ref=e256]:
                    - img
                - button "previous item" [disabled] [ref=e257]:
                  - img "previous item" [ref=e258]:
                    - img
          - generic [ref=e259]:
            - img:
              - img
            - generic [ref=e260]:
              - generic [ref=e261]:
                - button "Previous Page" [disabled] [ref=e263]:
                  - img [ref=e264]:
                    - img
                - button "Next Page" [ref=e265] [cursor=pointer]:
                  - img [ref=e266]:
                    - img
                - generic [ref=e267]:
                  - tablist "Use the left and right arrow keys to navigate between tabs" [ref=e268]:
                    - tab "Gross risk" [ref=e269] [cursor=pointer]:
                      - generic [ref=e271]: Gross risk
                    - tab "Net risk" [ref=e272] [cursor=pointer]:
                      - generic [ref=e274]: Net risk
                    - tab "Bowtie" [ref=e275] [cursor=pointer]:
                      - generic [ref=e277]: Bowtie
                    - tab "Measures" [ref=e278] [cursor=pointer]:
                      - generic [ref=e280]: Measures
                    - tab "Kritieke Bedrijfsfuncties" [ref=e281] [cursor=pointer]:
                      - generic [ref=e283]: Kritieke Bedrijfsfuncties
                    - tab "Dialogue" [active] [selected] [ref=e284]:
                      - generic [ref=e286]: Dialogue
                    - tab "Chat" [ref=e287] [cursor=pointer]:
                      - generic [ref=e289]: Chat
                    - tab "Information systems" [ref=e290] [cursor=pointer]:
                      - generic [ref=e292]: Information systems
                    - tab "Related" [ref=e293] [cursor=pointer]:
                      - generic [ref=e295]: Related
                    - tab "Tasks" [ref=e296] [cursor=pointer]:
                      - generic [ref=e298]: Tasks
                    - tab "Key Indicators" [ref=e299] [cursor=pointer]:
                      - generic [ref=e301]: Key Indicators
                    - tab "History" [ref=e302] [cursor=pointer]:
                      - generic [ref=e304]: History
                    - tab "mo data" [ref=e305] [cursor=pointer]:
                      - generic [ref=e307]: mo data
                    - tab "Risks" [ref=e308] [cursor=pointer]:
                      - generic [ref=e310]: Risks
                  - generic [ref=e312]:
                    - generic [ref=e315] [cursor=pointer]: Gross risk
                    - generic [ref=e318] [cursor=pointer]: Net risk
                    - generic [ref=e321] [cursor=pointer]: Bowtie
                    - generic [ref=e324] [cursor=pointer]: Measures
                    - generic [ref=e327] [cursor=pointer]: Kritieke Bedrijfsfuncties
                    - generic [ref=e330] [cursor=pointer]: Dialogue
                    - generic [ref=e333] [cursor=pointer]: Chat
                    - generic [ref=e336] [cursor=pointer]: Information systems
                    - generic [ref=e339] [cursor=pointer]: Related
                    - generic [ref=e342] [cursor=pointer]: Tasks
                    - generic [ref=e345] [cursor=pointer]: Key Indicators
                    - generic [ref=e348] [cursor=pointer]: History
                    - generic [ref=e351] [cursor=pointer]: mo data
                    - generic [ref=e354] [cursor=pointer]: Risks
              - generic [ref=e355]:
                - generic [ref=e362]:
                  - generic [ref=e369]:
                    - generic [ref=e372]:
                      - generic [ref=e380]:
                        - textbox "Environment" [ref=e381]: QualiTlabs Hyd
                        - generic: Environment
                      - generic [ref=e389]:
                        - generic [ref=e390]:
                          - combobox "Domain(s)" [ref=e392] [cursor=pointer]
                          - generic:
                            - generic: Domain(s)
                        - generic [ref=e394]: arrow_drop_down
                      - generic [ref=e402]:
                        - generic [ref=e403]:
                          - combobox "Labels" [ref=e405] [cursor=pointer]
                          - generic:
                            - generic: Labels
                        - generic [ref=e407]: arrow_drop_down
                      - generic [ref=e415]:
                        - textbox "Item number" [ref=e416]: QUALITLABS1.RIS.0000476
                        - generic: Item number
                      - generic [ref=e423]:
                        - generic [ref=e424]:
                          - generic [ref=e425]:
                            - generic [ref=e426]: NEW
                            - combobox "NEW Status *" [ref=e427] [cursor=pointer]
                          - generic:
                            - generic: Status *
                        - generic [ref=e429] [cursor=pointer]: close
                        - generic [ref=e431]: arrow_drop_down
                      - generic [ref=e439]:
                        - textbox "Name *" [ref=e440]: Risk_1779786115563
                        - generic: Name *
                      - generic [ref=e448]:
                        - textbox "Description" [ref=e449]: R1
                        - generic: Description
                      - generic [ref=e457]:
                        - textbox "Explanation" [ref=e458]
                        - generic: Explanation
                      - generic [ref=e466]:
                        - generic [ref=e467]:
                          - combobox "Gross valuation type" [ref=e469] [cursor=pointer]
                          - generic:
                            - generic: Gross valuation type
                        - generic [ref=e471]: arrow_drop_down
                      - generic [ref=e477]:
                        - toolbar [ref=e479]:
                          - generic [ref=e480]: Information links
                          - button [ref=e481] [cursor=pointer]:
                            - img [ref=e483]: add
                        - generic [ref=e485]:
                          - list
                      - generic [ref=e493]:
                        - textbox "Cause description" [ref=e494]
                        - generic: Cause description
                      - generic [ref=e502]:
                        - textbox "Effect description" [ref=e503]
                        - generic: Effect description
                      - generic [ref=e511]:
                        - generic [ref=e512]:
                          - combobox "Management Strategy" [ref=e514] [cursor=pointer]
                          - generic:
                            - generic: Management Strategy
                        - generic [ref=e516]: arrow_drop_down
                      - generic [ref=e524]:
                        - generic [ref=e525]:
                          - combobox "Treatment" [ref=e527] [cursor=pointer]
                          - generic:
                            - generic: Treatment
                        - generic [ref=e529]: arrow_drop_down
                      - generic [ref=e536]:
                        - generic [ref=e537]:
                          - combobox "Owner group" [ref=e539] [cursor=pointer]
                          - generic:
                            - generic: Owner group
                        - generic [ref=e541]: arrow_drop_down
                      - generic [ref=e548]:
                        - generic [ref=e549]:
                          - combobox "Owner (A)" [ref=e551] [cursor=pointer]
                          - generic:
                            - generic: Owner (A)
                        - generic [ref=e553]: arrow_drop_down
                      - generic [ref=e561]:
                        - generic [ref=e562]:
                          - combobox "Department" [ref=e564] [cursor=pointer]
                          - generic:
                            - generic: Department
                        - generic [ref=e566]: arrow_drop_down
                      - generic [ref=e574]:
                        - generic [ref=e575]:
                          - combobox "MAPGOOD" [ref=e577] [cursor=pointer]
                          - generic:
                            - generic: MAPGOOD
                        - generic [ref=e579]: arrow_drop_down
                      - generic [ref=e587]:
                        - textbox "Scenario" [ref=e588]
                        - generic: Scenario
                      - generic [ref=e596]:
                        - generic [ref=e597]:
                          - combobox "Categories" [ref=e599] [cursor=pointer]
                          - generic:
                            - generic: Categories
                        - generic [ref=e601]: arrow_drop_down
                      - generic [ref=e609]:
                        - generic [ref=e610]:
                          - combobox "Availabilty" [ref=e612] [cursor=pointer]
                          - generic:
                            - generic: Availabilty
                        - generic [ref=e614]: arrow_drop_down
                      - generic [ref=e622]:
                        - generic [ref=e623]:
                          - combobox "Nearness" [ref=e625] [cursor=pointer]
                          - generic:
                            - generic: Nearness
                        - generic [ref=e627]: arrow_drop_down
                      - generic [ref=e631]:
                        - generic [ref=e632]: Total coverage
                        - progressbar [ref=e634]:
                          - status "0%" [ref=e637]
                      - generic [ref=e641]:
                        - generic [ref=e642]: Effective coverage
                        - progressbar [ref=e644]:
                          - status "0%" [ref=e647]
                      - generic [ref=e651]:
                        - generic [ref=e652]: Potential coverage
                        - progressbar [ref=e654]:
                          - status "0%" [ref=e657]
                      - generic [ref=e668]:
                        - textbox "Itemid" [ref=e669]
                        - generic: Itemid
                      - generic [ref=e677]:
                        - textbox "Added by" [ref=e678]: mahendra j
                        - generic: Added by
                      - generic [ref=e683]:
                        - generic [ref=e684]:
                          - generic: event
                        - generic [ref=e687]:
                          - textbox "Date added" [ref=e688]: 26-05-2026 11:08:47
                          - generic: Date added
                        - generic [ref=e689]:
                          - generic: access_time
                      - generic [ref=e694]:
                        - generic [ref=e695]:
                          - generic: event
                        - generic [ref=e698]:
                          - textbox "Date modified" [ref=e699]
                          - generic: Date modified
                        - generic [ref=e700]:
                          - generic: access_time
                      - generic [ref=e705]:
                        - generic [ref=e706]:
                          - generic [ref=e709]: Documents
                          - button "Choose File" [ref=e710] [cursor=pointer]:
                            - generic [ref=e711]:
                              - img [ref=e712]: upload
                              - button "Choose File" [ref=e713]
                        - generic [ref=e716]:
                          - img [ref=e718]
                          - generic [ref=e719]: Drag and drop files here to upload
                          - button "Choose File" [ref=e720] [cursor=pointer]
                      - generic [ref=e728]:
                        - combobox "Group" [ref=e730] [cursor=pointer]
                        - generic:
                          - generic: Group
                      - generic [ref=e735]:
                        - generic [ref=e736]:
                          - generic: event
                        - generic [ref=e739]:
                          - textbox "State Date" [ref=e740]: 26-05-2026 11:08:47
                          - generic: State Date
                        - generic [ref=e741]:
                          - generic: access_time
                    - generic [ref=e745]:
                      - generic [ref=e752]:
                        - generic [ref=e758]:
                          - textbox "Version number" [ref=e759]: "1"
                          - generic: Version number
                        - generic [ref=e764]:
                          - textbox "Version name *" [ref=e765]: Version name
                          - generic: Version name *
                      - generic [ref=e772] [cursor=pointer]:
                        - generic [ref=e773]:
                          - generic [ref=e774]:
                            - generic [ref=e775]: ACTIVE
                            - combobox "ACTIVE Version status *" [ref=e776]: ACTIVE
                          - generic:
                            - generic: Version status *
                        - generic [ref=e778]: arrow_drop_down
                      - generic [ref=e786]:
                        - textbox "Version description" [ref=e787]
                        - generic: Version description
                      - generic [ref=e794]:
                        - generic [ref=e795]:
                          - combobox "Executor group" [ref=e797] [cursor=pointer]
                          - generic:
                            - generic: Executor group
                        - generic [ref=e799]: arrow_drop_down
                      - generic [ref=e806]:
                        - generic [ref=e807]:
                          - combobox "Executor" [ref=e809] [cursor=pointer]
                          - generic:
                            - generic: Executor
                        - generic [ref=e811]: arrow_drop_down
                      - generic [ref=e815]:
                        - generic [ref=e818]:
                          - generic [ref=e820] [cursor=pointer]: event
                          - generic [ref=e823]:
                            - textbox "Due date" [ref=e824]
                            - generic: Due date
                        - generic [ref=e825]:
                          - button [ref=e827] [cursor=pointer]:
                            - img [ref=e829]:
                              - img [ref=e830]
                          - button [ref=e832] [cursor=pointer]:
                            - img [ref=e834]:
                              - img [ref=e835]
                      - generic [ref=e842]:
                        - generic [ref=e843]:
                          - combobox "Persons to be informed" [ref=e845] [cursor=pointer]
                          - generic:
                            - generic: Persons to be informed
                        - generic [ref=e847]: arrow_drop_down
                      - generic [ref=e854]:
                        - generic [ref=e855]:
                          - combobox "Persons to consult" [ref=e857] [cursor=pointer]
                          - generic:
                            - generic: Persons to consult
                        - generic [ref=e859]: arrow_drop_down
                      - generic [ref=e867]:
                        - textbox "hour estimate" [ref=e868]
                        - generic: hour estimate
                  - generic [ref=e869]:
                    - button "Refresh" [ref=e870] [cursor=pointer]:
                      - img "previous item" [ref=e871]: refresh
                    - generic [ref=e872]:
                      - img [ref=e874]
                      - heading "Select in the gray area in the field Gross valuation type \" a desired data value, after which the corresponding data form appears here!" [level=2] [ref=e1034]
                - tabpanel "Dialogue" [ref=e1035]:
                  - generic [ref=e1043]:
                    - button "inpreparation Test_1779786115563 Card image %" [ref=e1045] [cursor=pointer]:
                      - generic [ref=e1046]:
                        - img "inpreparation" [ref=e1048]
                        - generic "Test_1779786115563" [ref=e1049]:
                          - generic [ref=e1050]: Test_1779786115563
                      - img "Card image" [ref=e1052]
                      - generic [ref=e1054]:
                        - generic [ref=e1055]:
                          - generic: "%"
                        - button [ref=e1057]:
                          - img
                    - button "finished Questionnaire_1779786115563 Card image 100%" [ref=e1059] [cursor=pointer]:
                      - generic [ref=e1060]:
                        - img "finished" [ref=e1062]
                        - generic "Questionnaire_1779786115563" [ref=e1063]:
                          - generic [ref=e1064]: Questionnaire_1779786115563
                      - img "Card image" [ref=e1066]
                      - generic [ref=e1070]: 100%
  - iframe [ref=e1072]:
    - generic [active]:
      - generic:
        - text:  
        - button "Open chat" [ref=f6e1] [cursor=pointer]
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
> 9   |     await expect(element).toBeEnabled();
      |                           ^ Error: expect(locator).toBeEnabled() failed
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
  109 |     await expect(element).toBeVisible();
```