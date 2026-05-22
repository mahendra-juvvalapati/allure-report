# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: E2E_Tests/FC008_questionnaire.spec.ts >> FC_008_Questionnaire Flow >> Configure questionnaire with 'Add documents as evidence' and verify 'Send mail' action is executed when Question condition is triggered on 'Change a question' and check Questionnaire 'Set item state to' action
- Location: tests/E2E_Tests/FC008_questionnaire.spec.ts:37:9

# Error details

```
Error: expect(locator).not.toBeVisible() failed

Locator:  getByText('Warning')
Expected: not visible
Received: visible
Timeout:  15000ms

Call log:
  - Expect "not toBeVisible" with timeout 15000ms
  - waiting for getByText('Warning')
    18 × locator resolved to <span data-v-395a6c6f="">Warning</span>
       - unexpected value "visible"

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
            - status "7" [ref=e38]
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
              - button "Audit sets" [ref=e138] [cursor=pointer]:
                - img [ref=e139]:
                  - img
                - generic [ref=e140]: Audit sets
              - button "Impact Assessments" [ref=e141] [cursor=pointer]:
                - img [ref=e142]:
                  - img
                - generic [ref=e143]: Impact Assessments
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
              - button "Performance agreements" [ref=e177] [cursor=pointer]:
                - img [ref=e178]:
                  - img
                - generic [ref=e179]: Performance agreements
              - button "Key Figures" [ref=e180] [cursor=pointer]:
                - img [ref=e181]:
                  - img
                - generic [ref=e182]: Key Figures
              - button "Settings" [ref=e183] [cursor=pointer]:
                - img [ref=e184]:
                  - img
                - generic [ref=e185]: Settings
              - button "Critical Business Scenarios" [ref=e186] [cursor=pointer]:
                - img [ref=e187]:
                  - img
                - generic [ref=e188]: Critical Business Scenarios
              - button "BCM Plans" [ref=e189] [cursor=pointer]:
                - img [ref=e190]:
                  - img
                - generic [ref=e191]: BCM Plans
              - button "Context analysis" [ref=e192] [cursor=pointer]:
                - img [ref=e193]:
                  - img
                - generic [ref=e194]: Context analysis
              - button "Situations" [ref=e195] [cursor=pointer]:
                - img [ref=e196]:
                  - img
                - generic [ref=e197]: Situations
              - button "Planstappen" [ref=e198] [cursor=pointer]:
                - img [ref=e199]:
                  - img
                - generic [ref=e200]: Planstappen
              - button "BOBOC logs" [ref=e201] [cursor=pointer]:
                - img [ref=e202]:
                  - img
                - generic [ref=e203]: BOBOC logs
            - button "build Maintain keyboard_arrow_down" [ref=e204] [cursor=pointer]:
              - generic [ref=e205]: build
              - generic [ref=e206]: Maintain
              - generic [ref=e207]: keyboard_arrow_down
            - list [ref=e208]:
              - button "assignment_turned_in Questionnaires, forms" [ref=e209] [cursor=pointer]:
                - generic [ref=e210]: assignment_turned_in
                - generic [ref=e211]: Questionnaires, forms
              - button "Workflows & conditions" [ref=e212] [cursor=pointer]:
                - img [ref=e213]:
                  - img
                - generic [ref=e214]: Workflows & conditions
      - generic [ref=e218]:
        - generic [ref=e220]:
          - generic [ref=e221]:
            - generic [ref=e223]:
              - button [ref=e225] [cursor=pointer]:
                - img [ref=e227]: arrow_back
              - generic [ref=e229]:
                - generic [ref=e231] [cursor=pointer]: QualiTlabs
                - generic [ref=e233]: keyboard_arrow_right
                - generic [ref=e235] [cursor=pointer]: Templates
                - generic [ref=e237]: keyboard_arrow_right
                - generic [ref=e239] [cursor=pointer]: QA Automation
                - generic [ref=e241]: keyboard_arrow_right
                - generic [ref=e243] [cursor=pointer]: Questionnaires, forms
            - generic [ref=e245]:
              - button [ref=e246] [cursor=pointer]:
                - img [ref=e248]: content_copy
              - button "Publish" [ref=e249] [cursor=pointer]:
                - generic [ref=e250]:
                  - img [ref=e251]: file_upload
                  - generic [ref=e252]: Publish
              - button [ref=e253] [cursor=pointer]:
                - img [ref=e255]: more_vert
          - generic [ref=e256]: Questionnaire 1779439453443
        - generic [ref=e258]:
          - toolbar [ref=e260]:
            - tablist [ref=e261]:
              - generic [ref=e262]:
                - tab "Settings" [ref=e263] [cursor=pointer]:
                  - generic [ref=e265]: Settings
                - tab "Questionnaire" [ref=e267] [cursor=pointer]:
                  - generic [ref=e269]: Questionnaire
                - tab "QUESTION CONDITIONS" [selected] [ref=e271] [cursor=pointer]:
                  - generic [ref=e273]: QUESTION CONDITIONS
                - tab "QUESTIONNAIRE CONDITIONS" [ref=e275] [cursor=pointer]:
                  - generic [ref=e277]: QUESTIONNAIRE CONDITIONS
                - tab "Indicators" [ref=e279] [cursor=pointer]:
                  - generic [ref=e281]: Indicators
          - tabpanel [ref=e285]:
            - tabpanel [ref=e286]:
              - generic [ref=e291]:
                - toolbar [ref=e293]:
                  - tablist [ref=e294]:
                    - tab "tab1" [selected] [ref=e296] [cursor=pointer]:
                      - generic [ref=e298]: tab1
                  - button "Add tab" [ref=e302] [cursor=pointer]:
                    - generic [ref=e303]:
                      - generic [ref=e304]: Add tab
                      - img [ref=e305]: add_circle
                - tabpanel [ref=e308]:
                  - tabpanel [ref=e309]:
                    - generic [ref=e310]:
                      - generic [ref=e312]:
                        - generic [ref=e317]:
                          - generic [ref=e319]: search
                          - textbox [ref=e321]:
                            - /placeholder: Type to Search
                        - list [ref=e323]:
                          - listitem [ref=e324]:
                            - generic [ref=e326]: list
                            - generic [ref=e328]: condition1
                            - switch [checked] [ref=e331] [cursor=pointer]
                      - generic [ref=e335]:
                        - generic [ref=e336]:
                          - generic [ref=e337]:
                            - generic [ref=e338]:
                              - generic [ref=e344]:
                                - textbox "Condition Name *" [ref=e345]: condition1
                                - generic: Condition Name *
                              - generic: Enabled
                              - button [ref=e347] [cursor=pointer]:
                                - img [ref=e349]: delete
                              - button [ref=e351] [cursor=pointer]:
                                - img [ref=e353]: content_copy
                            - generic [ref=e358]:
                              - textbox "Condition Description" [ref=e359]
                              - generic: Condition Description
                            - generic [ref=e360]:
                              - generic [ref=e364]:
                                - generic [ref=e365]:
                                  - generic [ref=e366]:
                                    - generic [ref=e367]: Change a question
                                    - combobox "Change a question Trigger On" [ref=e368] [cursor=pointer]
                                  - generic:
                                    - generic: Trigger On
                                - generic [ref=e370]: arrow_drop_down
                              - generic [ref=e371]:
                                - generic [ref=e375]:
                                  - generic [ref=e376]:
                                    - generic [ref=e377]:
                                      - generic [ref=e378]: Number questions
                                      - combobox "Number questions Page" [ref=e379] [cursor=pointer]
                                    - generic:
                                      - generic: Page
                                  - generic [ref=e381]: arrow_drop_down
                                - generic [ref=e386]:
                                  - generic [ref=e387]:
                                    - generic [ref=e388]:
                                      - generic [ref=e389]: Number / Amount question with positive answer
                                      - combobox "Number / Amount question with positive answer Question" [ref=e390] [cursor=pointer]
                                    - generic:
                                      - generic: Question
                                  - generic [ref=e392]: arrow_drop_down
                          - generic [ref=e393]:
                            - generic [ref=e395]:
                              - generic [ref=e397] [cursor=pointer]:
                                - generic [ref=e398]:
                                  - generic [ref=e399]:
                                    - generic [ref=e400]: tab1
                                    - combobox "tab1 Tab *" [ref=e401]: tab1
                                  - generic:
                                    - generic: Tab *
                                - generic [ref=e403]: arrow_drop_down
                              - button [ref=e405] [cursor=pointer]:
                                - img [ref=e407]: edit
                            - generic [ref=e412]:
                              - textbox "Tab Description" [ref=e413]: tab1 description
                              - generic: Tab Description
                        - generic [ref=e415]:
                          - generic [ref=e418]:
                            - generic [ref=e419]:
                              - generic [ref=e420]: Meet
                              - generic [ref=e425] [cursor=pointer]:
                                - generic [ref=e427]:
                                  - generic [ref=e428]: ALL
                                  - combobox "ALL" [ref=e429]
                                - generic [ref=e431]: arrow_drop_down
                              - generic [ref=e432]: OF THE FOLLOWING CONDITIONS
                            - button "Add condition" [ref=e434] [cursor=pointer]:
                              - generic [ref=e435]:
                                - generic [ref=e436]: Add condition
                                - img [ref=e437]: add_circle
                          - generic [ref=e439]:
                            - generic [ref=e444]:
                              - generic [ref=e445]:
                                - generic [ref=e446]:
                                  - generic [ref=e447]: Calculation
                                  - combobox "Calculation Condition On" [ref=e448] [cursor=pointer]
                                - generic:
                                  - generic: Condition On
                              - generic [ref=e450]: arrow_drop_down
                            - generic [ref=e456]:
                              - textbox "Calculation formula" [ref=e457]: 10*10
                              - generic: Calculation formula
                            - generic [ref=e462]:
                              - generic [ref=e463]:
                                - generic [ref=e464]:
                                  - generic [ref=e465]: =
                                  - combobox "= Operator" [ref=e466] [cursor=pointer]
                                - generic:
                                  - generic: Operator
                              - generic [ref=e468]: arrow_drop_down
                            - generic [ref=e475]:
                              - textbox "value" [ref=e476]: "100"
                              - generic: value
                            - button [ref=e478] [cursor=pointer]:
                              - img [ref=e480]: delete
                        - generic [ref=e482]:
                          - generic [ref=e485]:
                            - generic [ref=e486]: ACTIONS WHEN CONDITION IS TRUE
                            - button "Add action" [ref=e488] [cursor=pointer]:
                              - generic [ref=e489]:
                                - generic [ref=e490]: Add action
                                - img [ref=e491]: add_circle
                          - generic [ref=e493]:
                            - generic [ref=e498]:
                              - generic [ref=e499]:
                                - generic [ref=e500]:
                                  - generic [ref=e501]: Send mail
                                  - combobox "Send mail Action type" [ref=e502]
                                - generic:
                                  - generic: Action type
                              - generic [ref=e504]: arrow_drop_down
                            - button [ref=e506] [cursor=pointer]:
                              - img [ref=e508]: settings
                            - button "Configure Email" [ref=e510] [cursor=pointer]:
                              - generic [ref=e512]: Configure Email
                            - button [ref=e514] [cursor=pointer]:
                              - img [ref=e516]: delete
                      - button [ref=e517] [cursor=pointer]:
                        - img [ref=e519]: add
  - iframe [ref=e521]:
    - generic [active]:
      - generic:
        - text:  
        - button "Open chat" [ref=f6e1] [cursor=pointer]
  - generic:
    - dialog:
      - generic [ref=e523]:
        - toolbar [ref=e525]:
          - generic [ref=e526]: User Settings
          - button [ref=e528] [cursor=pointer]:
            - img [ref=e530]: close
        - generic [ref=e534]:
          - generic [ref=e539]:
            - generic [ref=e540]:
              - generic [ref=e541]:
                - generic [ref=e542]:
                  - generic [ref=e544]: Added by
                  - button "Remove" [ref=e545] [cursor=pointer]: cancel
                - combobox "Added by Remove Select user fields" [ref=e546] [cursor=pointer]
              - generic:
                - generic: Select user fields
            - generic [ref=e548]: arrow_drop_down
          - generic [ref=e553] [cursor=pointer]:
            - generic [ref=e554]:
              - combobox "Role" [ref=e556]
              - generic:
                - generic: Role
            - generic [ref=e558]: arrow_drop_down
          - generic [ref=e563]:
            - generic [ref=e564]:
              - generic [ref=e565]:
                - generic [ref=e566]: What is your user?
                - combobox "What is your user? Select user type questions" [ref=e567] [cursor=pointer]
              - generic:
                - generic: Select user type questions
            - generic [ref=e569] [cursor=pointer]: close
            - generic [ref=e571]: arrow_drop_down
          - generic [ref=e576]:
            - generic [ref=e577]:
              - generic [ref=e578]:
                - generic [ref=e579]: What is your email?
                - combobox "What is your email? Select email type questions" [ref=e580] [cursor=pointer]
              - generic:
                - generic: Select email type questions
            - generic [ref=e582] [cursor=pointer]: close
            - generic [ref=e584]: arrow_drop_down
          - radiogroup [ref=e589]:
            - radio "Send link to item" [ref=e591] [cursor=pointer]:
              - img [ref=e593]
              - generic [ref=e595]: Send link to item
            - radio "Send link to questionnaire" [checked] [ref=e597] [cursor=pointer]:
              - img [ref=e599]
              - generic [ref=e602]: Send link to questionnaire
        - generic [ref=e604]:
          - button "Cancel" [ref=e605] [cursor=pointer]:
            - generic [ref=e607]: Cancel
          - button "Ok" [ref=e608] [cursor=pointer]:
            - generic [ref=e610]: Ok
  - generic:
    - dialog:
      - generic [ref=e612]:
        - generic [ref=e613]:
          - generic [ref=e614]:
            - generic [ref=e615]: Warning
            - img [ref=e617]
            - button [ref=e618] [cursor=pointer]:
              - img [ref=e620]: close
          - separator [ref=e621]
          - generic [ref=e622]: Changing mail type will clear previous mail configuration. Do you want to change the mail type?
        - generic [ref=e625]:
          - button "Yes" [ref=e626] [cursor=pointer]:
            - generic [ref=e628]: "Yes"
          - button "No" [ref=e629] [cursor=pointer]:
            - generic [ref=e631]: "No"
```

# Test source

```ts
  480 |       await this.actions.click(this.okBtn);
  481 |     }
  482 |     else {
  483 |       const okText = this.page.getByText('OK', { exact: true });
  484 |       await this.actions.click(okText);
  485 |     }
  486 |   }
  487 | 
  488 |   async clickOkayButton() {
  489 |     await this.actions.click(this.okayBtn);
  490 |   }
  491 | 
  492 |   async clickAddHeadersButton() {
  493 |     await this.actions.click(this.addHeadersBtn);
  494 |   }
  495 | 
  496 |   async enterKeyAndValue(key: string, value: string) {
  497 |     const keyInput = this.page.getByRole('gridcell').locator('col-id="type"');
  498 |     await this.actions.type(keyInput, key);
  499 | 
  500 |     const valueInput = this.page.getByRole('gridcell').locator('col-id="value"');
  501 |     await this.actions.type(valueInput, value);
  502 |   }
  503 | 
  504 |   async selectReport(reportName: string) {
  505 |     await this.actions.click(this.reportsDropdown);
  506 |     const option = this.page.getByRole('option', { name: reportName });
  507 |     await this.actions.click(option);
  508 |   }
  509 | 
  510 |   async clickOnConfigureIcon() {
  511 |     await this.actions.click(this.configureIcon);
  512 |   }
  513 | 
  514 |   async selectUserFieldInSendEmail(user: string) {
  515 |     await this.actions.click(this.userFieldDorpdownInEmailAction);
  516 |     // await this.actions.click(this.page.getByRole('option', { name: 'Owner (A)', exact: true }));
  517 |     const option = this.page.getByRole('option', { name: user, exact: true });
  518 |     await this.actions.click(option);
  519 |     await this.actions.click(this.userFieldDorpdownInEmailAction);
  520 |   }
  521 | 
  522 |   async selectRoleInSendEmail(role: string) {
  523 |     await this.actions.click(this.userRoleDropdownInEmailAction);
  524 | 
  525 |     const option = this.page.getByRole('option', { name: role, exact: true });
  526 |     await this.actions.click(option);
  527 |     await this.actions.click(this.userRoleDropdownInEmailAction);
  528 |   }
  529 | 
  530 |   async selectUserTypeQuestionInSendEmail(userType: string) {
  531 |     const userTypeQuestionDefault = this.page.getByLabel(userType + 'Select user type questionsclosearrow_drop_down', { exact: true });
  532 |     await this.actions.click(this.userTypeQuestionDropdownInEmailAction);
  533 | 
  534 |     const option = this.page.getByRole('option', { name: userType, exact: true });
  535 |     if (!await userTypeQuestionDefault.isVisible()) {
  536 |       await this.actions.click(option);
  537 |     }
  538 |     await this.actions.click(this.userTypeQuestionDropdownInEmailAction);
  539 |   }
  540 | 
  541 |   async selectEmailTypeQuestionInSendEmail(emailType: string) {
  542 |     const emailTypeQuestionDefault = this.page.getByLabel(emailType + 'Select email type questionsclosearrow_drop_down', { exact: true });
  543 |     await this.actions.click(this.emailTypeQuestionDropdownInEmailAction);
  544 | 
  545 |     const option = this.page.getByRole('option', { name: emailType, exact: true });
  546 |     if (!await emailTypeQuestionDefault.isVisible()) {
  547 |       await this.actions.click(option);
  548 |     }
  549 |     await this.actions.click(this.emailTypeQuestionDropdownInEmailAction);
  550 |   }
  551 | 
  552 |   async enableSendLinkToItemInSendEmail() {
  553 |     await this.actions.click(this.sendLinkToItemRadioBtnInEmailAction);
  554 |     if (await this.yesBtn.isVisible()) {
  555 |       await this.clickOnyesBtn();
  556 |     }
  557 |   }
  558 | 
  559 |   async enableSendLinkToQuestionnaireInSendEmail() {
  560 |     await this.actions.click(this.sendLinkToQuestionnaireRadioBtnInEmailAction);
  561 |     if (await this.yesBtn.isVisible()) {
  562 |       await this.clickOnyesBtn();
  563 |     }
  564 |   }
  565 | 
  566 |   async configureUserSettingsforSendMail(userSettings: any) {
  567 |     await this.clickOnConfigureIcon();
  568 |     await this.userFieldDorpdownInEmailAction.locator('xpath=/preceding::i[@aria-label="Remove"]').click();
  569 |     await this.selectUserFieldInSendEmail(userSettings.userField);
  570 |     // await this.selectRoleInSendEmail(userSettings.userRole);
  571 |     await this.selectUserTypeQuestionInSendEmail(userSettings.userTypeQuestion);
  572 |     await this.selectEmailTypeQuestionInSendEmail(userSettings.emailTypeQuestion);
  573 | 
  574 |     if (userSettings.sendLinkToItem) {
  575 |       await this.enableSendLinkToItemInSendEmail();
  576 |     }
  577 |     else if (userSettings.sendLinkToQuestionnaire) {
  578 |       await this.enableSendLinkToQuestionnaireInSendEmail();
  579 |     }
> 580 |     await expect(this.page.getByText('Warning')).not.toBeVisible({ timeout: 15000 });
      |                                                      ^ Error: expect(locator).not.toBeVisible() failed
  581 |     
  582 |     await this.actions.click(this.okBtn);
  583 |   }
  584 | 
  585 |   async selectTrigger(triggerOption: string) {
  586 |     await this.clickTriggerOnDropdown();
  587 |     const option = this.page.getByRole('option', { name: triggerOption });
  588 |     await this.actions.click(option);
  589 |   }
  590 | 
  591 |   async selectPageName(pageName: string) {
  592 |     await this.actions.click(this.selectPageNameDropdown);
  593 | 
  594 |     const option = this.page.getByRole('option', { name: pageName });
  595 |     await this.actions.click(option);
  596 |   }
  597 | 
  598 |   async selectQuestion(questionName: string) {
  599 |     await this.clickQuestionAnswerChange();
  600 | 
  601 |     const option = this.page.getByRole('option', { name: questionName });
  602 |     await this.actions.click(option);
  603 |   }
  604 | 
  605 |   async clickQuestionAnswerChange() {
  606 |     await this.actions.click(this.questionAnswerChangeBtn);
  607 |   }
  608 | 
  609 |   async addCondition(conditionType: string) {
  610 |     await this.actions.click(this.addConditionBtn);
  611 |     await this.actions.click(this.conditionTypeDropdown);
  612 | 
  613 |     const option = this.page.getByRole('option', { name: conditionType });
  614 |     await this.actions.click(option);
  615 |   }
  616 | 
  617 |   async selectPageNameInCondition(pageName: string) {
  618 |     await this.actions.click(this.pageNameDropdownInCondition);
  619 | 
  620 |     const option = this.page.getByRole('option', { name: pageName, exact: true });
  621 |     await this.actions.click(option);
  622 |   }
  623 | 
  624 |   async selectWhereInCondition(whereOption: string) {
  625 |     await this.actions.click(this.whereDropdownInCondition);
  626 | 
  627 |     const option = this.page.getByRole('option', { name: whereOption });
  628 |     await this.actions.click(option);
  629 |   }
  630 | 
  631 |   async selectOperatorInCondition(operator: string) {
  632 |     await this.actions.click(this.operatorDropdownInCondition);
  633 | 
  634 |     const option = this.page.getByRole('option', { name: operator, exact: true });
  635 |     await this.actions.click(option);
  636 |   }
  637 | 
  638 |   async enterValueInCondition(value: string) {
  639 |     await this.actions.type(this.valueInputInCondition, value);
  640 |   }
  641 | 
  642 |   async clickAddActionButton() {
  643 |     await this.actions.click(this.addActionBtn);
  644 |   }
  645 | 
  646 |   async selectServiceInAction(serviceName: string) {
  647 |     await this.actions.click(this.servicesDropdown);
  648 | 
  649 |     const option = this.page.getByRole('option', { name: serviceName, exact: true });
  650 |     await this.actions.click(option);
  651 |   }
  652 | 
  653 |   async addAction(actionType: string) {
  654 |     await this.actions.click(this.addActionBtn);
  655 |     await this.actions.click(this.actionTypeDropdown);
  656 | 
  657 |     const option = this.page.getByRole('option', { name: actionType, exact: true });
  658 |     await this.actions.click(option);
  659 |   }
  660 | 
  661 |   async selectActionOn(actionOnOption: string) {
  662 |     await this.actions.click(this.actionOnDropdown);
  663 | 
  664 |     const option = this.page.getByRole('option', { name: actionOnOption });
  665 |     await this.actions.click(option);
  666 |   }
  667 | 
  668 |   async selectPageNameInAction(pageName: string) {
  669 |     await this.actions.click(this.pageNameDropdownInAction);
  670 | 
  671 |     const option = this.page.getByRole('option', { name: pageName, exact: true });
  672 |     await this.actions.click(option);
  673 |   }
  674 | 
  675 |   async selectFieldInAction(fieldName: string) {
  676 |     await this.actions.click(this.actionFieldDropdownInAction);
  677 | 
  678 |     const option = this.page.getByRole('option', { name: fieldName }).first();
  679 |     await this.actions.click(option);
  680 |   }
```