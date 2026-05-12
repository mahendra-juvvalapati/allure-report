# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: questionnaireCondition.spec.ts >> Questionnaire Condition Tests >> TC_QNC_030-Verify 'Update Current Item' action can be created successfully in questionnaire conditions
- Location: tests/questionnaireCondition.spec.ts:302:9

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByLabel('Owner grouparrow_drop_down').last()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for getByLabel('Owner grouparrow_drop_down').last()

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
          - status "43" [ref=e36]
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
    - generic [ref=e216]:
      - generic [ref=e218]:
        - generic [ref=e219]:
          - generic [ref=e221]:
            - button [ref=e223] [cursor=pointer]:
              - img [ref=e225]: arrow_back
            - generic [ref=e227]:
              - generic [ref=e229] [cursor=pointer]: QualiTlabs
              - generic [ref=e231]: keyboard_arrow_right
              - generic [ref=e233] [cursor=pointer]: Templates
              - generic [ref=e235]: keyboard_arrow_right
              - generic [ref=e237] [cursor=pointer]: QA Automation
              - generic [ref=e239]: keyboard_arrow_right
              - generic [ref=e241] [cursor=pointer]: Questionnaires, forms
          - generic [ref=e243]:
            - button [ref=e244] [cursor=pointer]:
              - img [ref=e246]: content_copy
            - button "Publish" [ref=e247] [cursor=pointer]:
              - generic [ref=e248]:
                - img [ref=e249]: file_upload
                - generic [ref=e250]: Publish
            - button [ref=e251] [cursor=pointer]:
              - img [ref=e253]: more_vert
        - generic [ref=e254]: Questionnaire_1778569762428
      - generic [ref=e256]:
        - toolbar [ref=e258]:
          - tablist [ref=e259]:
            - generic [ref=e260]:
              - tab "Settings" [ref=e261] [cursor=pointer]:
                - generic [ref=e263]: Settings
              - tab "Questionnaire" [ref=e265] [cursor=pointer]:
                - generic [ref=e267]: Questionnaire
              - tab "QUESTION CONDITIONS" [ref=e269] [cursor=pointer]:
                - generic [ref=e271]: QUESTION CONDITIONS
              - tab "QUESTIONNAIRE CONDITIONS" [selected] [ref=e273] [cursor=pointer]:
                - generic [ref=e275]: QUESTIONNAIRE CONDITIONS
              - tab "Indicators" [ref=e277] [cursor=pointer]:
                - generic [ref=e279]: Indicators
        - tabpanel [ref=e283]:
          - tabpanel [ref=e284]:
            - generic [ref=e289]:
              - toolbar [ref=e291]:
                - tablist [ref=e292]:
                  - tab "RenamedTab" [selected] [ref=e294] [cursor=pointer]:
                    - generic [ref=e296]: RenamedTab
                - button "Add tab" [ref=e300] [cursor=pointer]:
                  - generic [ref=e301]:
                    - generic [ref=e302]: Add tab
                    - img [ref=e303]: add_circle
              - tabpanel [ref=e306]:
                - tabpanel [ref=e307]:
                  - generic [ref=e308]:
                    - generic [ref=e310]:
                      - generic [ref=e315]:
                        - generic [ref=e317]: search
                        - textbox [ref=e319]:
                          - /placeholder: Type to Search
                      - list [ref=e321]:
                        - listitem [ref=e322]:
                          - generic [ref=e324]: list
                          - generic [ref=e326]: default
                          - switch [checked] [ref=e329] [cursor=pointer]
                        - listitem [ref=e333]:
                          - generic [ref=e335]: list
                          - generic [ref=e337]: condition1
                          - switch [checked] [ref=e340] [cursor=pointer]
                        - listitem [ref=e344]:
                          - generic [ref=e346]: list
                          - generic [ref=e348]: RenamedCondition
                          - switch [checked] [ref=e351] [cursor=pointer]
                        - listitem [ref=e355]:
                          - generic [ref=e357]: list
                          - generic [ref=e359]: Always
                          - switch [checked] [ref=e362] [cursor=pointer]
                        - listitem [ref=e366]:
                          - generic [ref=e368]: list
                          - generic [ref=e370]: nonConfirmity
                          - switch [checked] [ref=e373] [cursor=pointer]
                        - listitem [ref=e377]:
                          - generic [ref=e379]: list
                          - generic [ref=e381]: allQuestionnaireFinished
                          - switch [checked] [ref=e384] [cursor=pointer]
                        - listitem [ref=e388]:
                          - generic [ref=e390]: list
                          - generic [ref=e392]: notAllQuestionnaireFinished
                          - switch [checked] [ref=e395] [cursor=pointer]
                    - generic [ref=e400]:
                      - generic [ref=e401]:
                        - generic [ref=e402]:
                          - generic [ref=e408]:
                            - textbox "Condition Name *" [ref=e409]: notAllQuestionnaireFinished
                            - generic: Condition Name *
                          - generic: Enabled
                          - button [ref=e411] [cursor=pointer]:
                            - img [ref=e413]: delete
                          - button [ref=e415] [cursor=pointer]:
                            - img [ref=e417]: content_copy
                        - generic [ref=e422]:
                          - textbox "Condition Description" [ref=e423]
                          - generic: Condition Description
                        - generic [ref=e425]:
                          - text: Pre
                          - switch [disabled]
                          - text: Post
                      - generic [ref=e426]:
                        - generic [ref=e428]:
                          - generic [ref=e430]:
                            - generic [ref=e431]:
                              - generic [ref=e432]:
                                - generic [ref=e433]: RenamedTab
                                - combobox "RenamedTab Tab *" [ref=e434] [cursor=pointer]
                              - generic:
                                - generic: Tab *
                            - generic [ref=e436]: arrow_drop_down
                          - button [ref=e438] [cursor=pointer]:
                            - img [ref=e440]: edit
                        - generic [ref=e445]:
                          - textbox "Tab Description" [ref=e446]: This is a default tab
                          - generic: Tab Description
                      - generic [ref=e451]:
                        - generic [ref=e452]:
                          - generic [ref=e453]: Meet
                          - generic [ref=e458] [cursor=pointer]:
                            - generic [ref=e460]:
                              - generic [ref=e461]: ALL
                              - combobox "ALL" [ref=e462]
                            - generic [ref=e464]: arrow_drop_down
                          - generic [ref=e465]: OF THE FOLLOWING CONDITIONS
                        - button "Add condition" [ref=e468] [cursor=pointer]:
                          - generic [ref=e469]:
                            - generic [ref=e470]: Add condition
                            - img [ref=e471]: add_circle
                      - generic [ref=e474]:
                        - generic [ref=e477]:
                          - generic [ref=e478]: ACTIONS WHEN CONDITION IS TRUE
                          - button "Add action" [ref=e480] [cursor=pointer]:
                            - generic [ref=e481]:
                              - generic [ref=e482]: Add action
                              - img [ref=e483]: add_circle
                        - generic [ref=e484]:
                          - generic [ref=e485]:
                            - generic [ref=e490]:
                              - generic [ref=e491]:
                                - generic [ref=e492]:
                                  - generic [ref=e493]: Enable
                                  - combobox "Enable Action type" [ref=e494] [cursor=pointer]
                                - generic:
                                  - generic: Action type
                              - generic [ref=e496]: arrow_drop_down
                            - generic [ref=e501]:
                              - generic [ref=e502]:
                                - generic [ref=e503]:
                                  - generic [ref=e504]: Questionnaire
                                  - combobox "Questionnaire Action on" [ref=e505] [cursor=pointer]
                                - generic:
                                  - generic: Action on
                              - generic [ref=e507]: arrow_drop_down
                            - generic [ref=e512]:
                              - generic [ref=e513]:
                                - combobox "Action field" [ref=e515] [cursor=pointer]
                                - generic:
                                  - generic: Action field
                              - generic [ref=e517]: arrow_drop_down
                            - button [ref=e519] [cursor=pointer]:
                              - img [ref=e521]: delete
                          - generic [ref=e522]:
                            - generic [ref=e527]:
                              - generic [ref=e528]:
                                - generic [ref=e529]:
                                  - generic [ref=e530]: Enable
                                  - combobox "Enable Action type" [ref=e531] [cursor=pointer]
                                - generic:
                                  - generic: Action type
                              - generic [ref=e533]: arrow_drop_down
                            - generic [ref=e538]:
                              - generic [ref=e539]:
                                - generic [ref=e540]:
                                  - generic [ref=e541]: Questionnaire
                                  - combobox "Questionnaire Action on" [ref=e542] [cursor=pointer]
                                - generic:
                                  - generic: Action on
                              - generic [ref=e544]: arrow_drop_down
                            - generic [ref=e549]:
                              - generic [ref=e550]:
                                - combobox "Action field" [ref=e552] [cursor=pointer]
                                - generic:
                                  - generic: Action field
                              - generic [ref=e554]: arrow_drop_down
                            - button [ref=e556] [cursor=pointer]:
                              - img [ref=e558]: delete
                          - generic [ref=e559]:
                            - generic [ref=e564]:
                              - generic [ref=e565]:
                                - generic [ref=e566]:
                                  - generic [ref=e567]: Enable
                                  - combobox "Enable Action type" [ref=e568] [cursor=pointer]
                                - generic:
                                  - generic: Action type
                              - generic [ref=e570]: arrow_drop_down
                            - generic [ref=e575]:
                              - generic [ref=e576]:
                                - generic [ref=e577]:
                                  - generic [ref=e578]: Condition
                                  - combobox "Condition Action on" [ref=e579] [cursor=pointer]
                                - generic:
                                  - generic: Action on
                              - generic [ref=e581]: arrow_drop_down
                            - generic [ref=e586]:
                              - generic [ref=e587]:
                                - generic [ref=e588]:
                                  - generic [ref=e589]: default
                                  - combobox "default Action field" [ref=e590] [cursor=pointer]
                                - generic:
                                  - generic: Action field
                              - generic [ref=e592]: arrow_drop_down
                            - button [ref=e594] [cursor=pointer]:
                              - img [ref=e596]: delete
                          - generic [ref=e597]:
                            - generic [ref=e602]:
                              - generic [ref=e603]:
                                - generic [ref=e604]:
                                  - generic [ref=e605]: Disable
                                  - combobox "Disable Action type" [ref=e606] [cursor=pointer]
                                - generic:
                                  - generic: Action type
                              - generic [ref=e608]: arrow_drop_down
                            - generic [ref=e613]:
                              - generic [ref=e614]:
                                - generic [ref=e615]:
                                  - generic [ref=e616]: Condition
                                  - combobox "Condition Action on" [ref=e617] [cursor=pointer]
                                - generic:
                                  - generic: Action on
                              - generic [ref=e619]: arrow_drop_down
                            - generic [ref=e624]:
                              - generic [ref=e625]:
                                - generic [ref=e626]:
                                  - generic [ref=e627]: default
                                  - combobox "default Action field" [ref=e628] [cursor=pointer]
                                - generic:
                                  - generic: Action field
                              - generic [ref=e630]: arrow_drop_down
                            - button [ref=e632] [cursor=pointer]:
                              - img [ref=e634]: delete
                          - generic [ref=e635]:
                            - generic [ref=e640]:
                              - generic [ref=e641]:
                                - generic [ref=e642]:
                                  - generic [ref=e643]: Disable Finishing of a questionnaire
                                  - combobox "Disable Finishing of a questionnaire Action type" [ref=e644] [cursor=pointer]
                                - generic:
                                  - generic: Action type
                              - generic [ref=e646]: arrow_drop_down
                            - generic [ref=e652]:
                              - textbox "Message" [ref=e653]: You are not eligible to finish this questionnaire.
                              - generic: Message
                            - button [ref=e655] [cursor=pointer]:
                              - img [ref=e657]: delete
                          - generic [ref=e658]:
                            - generic [ref=e663]:
                              - generic [ref=e664]:
                                - generic [ref=e665]:
                                  - generic [ref=e666]: Set version result state to
                                  - combobox "Set version result state to Action type" [ref=e667] [cursor=pointer]
                                - generic:
                                  - generic: Action type
                              - generic [ref=e669]: arrow_drop_down
                            - generic [ref=e674]:
                              - generic [ref=e675]:
                                - generic [ref=e676]:
                                  - generic [ref=e677]: PRE PASSED 1
                                  - combobox "PRE PASSED 1 Action value" [ref=e678] [cursor=pointer]
                                - generic:
                                  - generic: Action value
                              - generic [ref=e680] [cursor=pointer]: close
                              - generic [ref=e682]: arrow_drop_down
                            - button [ref=e684] [cursor=pointer]:
                              - img [ref=e686]: delete
                          - generic [ref=e687]:
                            - generic [ref=e692]:
                              - generic [ref=e693]:
                                - generic [ref=e694]:
                                  - generic [ref=e695]: Set quality state to
                                  - combobox "Set quality state to Action type" [ref=e696] [cursor=pointer]
                                - generic:
                                  - generic: Action type
                              - generic [ref=e698]: arrow_drop_down
                            - generic [ref=e703]:
                              - generic [ref=e704]:
                                - generic [ref=e705]:
                                  - generic [ref=e706]: Effective
                                  - combobox "Effective Action value" [ref=e707] [cursor=pointer]
                                - generic:
                                  - generic: Action value
                              - generic [ref=e709]: arrow_drop_down
                            - button [ref=e711] [cursor=pointer]:
                              - img [ref=e713]: delete
                          - generic [ref=e714]:
                            - generic [ref=e719]:
                              - generic [ref=e720]:
                                - generic [ref=e721]:
                                  - generic [ref=e722]: Set version state to closed
                                  - combobox "Set version state to closed Action type" [ref=e723] [cursor=pointer]
                                - generic:
                                  - generic: Action type
                              - generic [ref=e725]: arrow_drop_down
                            - button [ref=e727] [cursor=pointer]:
                              - img [ref=e729]: delete
                          - generic [ref=e730]:
                            - generic [ref=e735]:
                              - generic [ref=e736]:
                                - generic [ref=e737]:
                                  - generic [ref=e738]: Set item state to
                                  - combobox "Set item state to Action type" [ref=e739] [cursor=pointer]
                                - generic:
                                  - generic: Action type
                              - generic [ref=e741]: arrow_drop_down
                            - generic [ref=e746]:
                              - generic [ref=e747]:
                                - generic [ref=e748]:
                                  - generic [ref=e749]: Risks
                                  - combobox "Risks Module" [ref=e750] [cursor=pointer]
                                - generic:
                                  - generic: Module
                              - generic [ref=e752]: arrow_drop_down
                            - generic [ref=e757]:
                              - generic [ref=e758]:
                                - generic [ref=e759]:
                                  - generic [ref=e760]: IN PROGRESS
                                  - combobox "IN PROGRESS Module state" [ref=e761] [cursor=pointer]
                                - generic:
                                  - generic: Module state
                              - generic [ref=e763]: arrow_drop_down
                            - button [ref=e765] [cursor=pointer]:
                              - img [ref=e767]: delete
                          - generic [ref=e768]:
                            - generic [ref=e773]:
                              - generic [ref=e774]:
                                - generic [ref=e775]:
                                  - generic [ref=e776]: Set item list field to
                                  - combobox "Set item list field to Action type" [ref=e777] [cursor=pointer]
                                - generic:
                                  - generic: Action type
                              - generic [ref=e779]: arrow_drop_down
                            - generic [ref=e784]:
                              - generic [ref=e785]:
                                - generic [ref=e786]:
                                  - generic [ref=e787]: Categories
                                  - combobox "Categories List field" [ref=e788] [cursor=pointer]
                                - generic:
                                  - generic: List field
                              - generic [ref=e790]: arrow_drop_down
                            - generic [ref=e795]:
                              - generic [ref=e796]:
                                - generic [ref=e797]:
                                  - generic [ref=e798]: Planning
                                  - combobox "Planning List field value" [ref=e799] [cursor=pointer]
                                - generic:
                                  - generic: List field value
                              - generic [ref=e801]: arrow_drop_down
                            - button [ref=e803] [cursor=pointer]:
                              - img [ref=e805]: delete
                          - generic [ref=e806]:
                            - generic [ref=e811]:
                              - generic [ref=e812]:
                                - generic [ref=e813]:
                                  - generic [ref=e814]: Set Value to Variable
                                  - combobox "Set Value to Variable Action type" [ref=e815] [cursor=pointer]
                                - generic:
                                  - generic: Action type
                              - generic [ref=e817]: arrow_drop_down
                            - generic [ref=e822]:
                              - generic [ref=e824] [cursor=pointer]: close
                              - generic [ref=e825]:
                                - combobox "Variable name" [ref=e826]: What is your age?
                                - generic: Variable name
                            - checkbox "Calculate Formula" [checked] [ref=e828] [cursor=pointer]:
                              - img [ref=e831]
                              - generic [ref=e833]: Calculate Formula
                            - generic [ref=e839]:
                              - textbox "Variable value" [ref=e840]: ">=18"
                              - generic: Variable value
                            - button [ref=e842] [cursor=pointer]:
                              - img [ref=e844]: delete
                          - generic [ref=e845]:
                            - generic [ref=e850]:
                              - generic [ref=e851]:
                                - generic [ref=e852]:
                                  - generic [ref=e853]: Calculate all linktab kpis
                                  - combobox "Calculate all linktab kpis Action type" [ref=e854] [cursor=pointer]
                                - generic:
                                  - generic: Action type
                              - generic [ref=e856]: arrow_drop_down
                            - generic [ref=e861]:
                              - generic [ref=e862]:
                                - generic [ref=e863]:
                                  - generic [ref=e864]: Risks
                                  - combobox "Risks For MoType" [ref=e865] [cursor=pointer]
                                - generic:
                                  - generic: For MoType
                              - generic [ref=e867]: arrow_drop_down
                            - button [ref=e869] [cursor=pointer]:
                              - img [ref=e871]: delete
                          - generic [ref=e872]:
                            - generic [ref=e877]:
                              - generic [ref=e878]:
                                - generic [ref=e879]:
                                  - generic [ref=e880]: Update linked items of type
                                  - combobox "Update linked items of type Action type" [ref=e881] [cursor=pointer]
                                - generic:
                                  - generic: Action type
                              - generic [ref=e883]: arrow_drop_down
                            - generic [ref=e888]:
                              - generic [ref=e889]:
                                - generic [ref=e890]:
                                  - generic [ref=e891]: Risks
                                  - combobox "Risks Module" [ref=e892] [cursor=pointer]
                                - generic:
                                  - generic: Module
                              - generic [ref=e894]: arrow_drop_down
                            - button "Settings" [ref=e896] [cursor=pointer]:
                              - generic [ref=e898]: Settings
                            - button [ref=e900] [cursor=pointer]:
                              - img [ref=e902]: delete
                          - generic [ref=e903]:
                            - generic [ref=e908]:
                              - generic [ref=e909]:
                                - generic [ref=e910]:
                                  - generic [ref=e911]: Update Current Item
                                  - combobox "Update Current Item Action type" [ref=e912] [cursor=pointer]
                                - generic:
                                  - generic: Action type
                              - generic [ref=e914]: arrow_drop_down
                            - generic [ref=e919]:
                              - generic [ref=e920]:
                                - generic [ref=e921]:
                                  - generic [ref=e922]: Risks
                                  - combobox "Risks Module" [ref=e923] [cursor=pointer]
                                - generic:
                                  - generic: Module
                              - generic [ref=e925]: arrow_drop_down
                            - button "Settings" [ref=e927] [cursor=pointer]:
                              - generic [ref=e929]: Settings
                            - button [ref=e931] [cursor=pointer]:
                              - img [ref=e933]: delete
                    - button [ref=e934] [cursor=pointer]:
                      - img [ref=e936]: add
  - iframe [ref=e938]:
    - generic [active]:
      - generic:
        - text:  
        - button "Open chat" [ref=f10e1] [cursor=pointer]
  - generic:
    - dialog:
      - generic [ref=e940]:
        - toolbar [ref=e942]:
          - generic [ref=e943]: Settings
          - button [ref=e945] [cursor=pointer]:
            - img [ref=e947]: close
        - generic [ref=e950]:
          - generic [ref=e958]:
            - generic [ref=e959]:
              - generic [ref=e960]:
                - generic [ref=e961]: NEW
                - combobox "NEW Status" [ref=e962] [cursor=pointer]
              - generic:
                - generic: Status
            - generic [ref=e964] [cursor=pointer]: close
            - generic [ref=e966]: arrow_drop_down
          - generic [ref=e974]:
            - generic [ref=e975]:
              - generic [ref=e976]:
                - generic [ref=e977]: Effective
                - combobox "Effective Quality State" [active] [ref=e978] [cursor=pointer]
              - generic:
                - generic: Quality State
            - generic [ref=e980]: arrow_drop_down
          - generic [ref=e988]:
            - generic [ref=e989]:
              - combobox "Owner group" [ref=e991] [cursor=pointer]
              - generic:
                - generic: Owner group
            - img [ref=e993]
          - generic [ref=e1002]:
            - generic [ref=e1003]:
              - combobox "Executor group" [ref=e1005] [cursor=pointer]
              - generic:
                - generic: Executor group
            - img [ref=e1007]
          - generic [ref=e1011]:
            - checkbox "Set obligatory" [ref=e1012] [cursor=pointer]:
              - img [ref=e1015]
              - generic [ref=e1017]: Set obligatory
            - generic [ref=e1018]:
              - text: Not obligatory
              - switch [disabled]
              - text: Obligatory
          - generic [ref=e1021]:
            - checkbox "Set relevant" [ref=e1022] [cursor=pointer]:
              - img [ref=e1025]
              - generic [ref=e1027]: Set relevant
            - generic [ref=e1028]:
              - text: Relevant
              - switch [disabled]
              - text: Not relevant
          - generic [ref=e1031]:
            - generic [ref=e1032]: "Set Reminderdate1 to :"
            - generic [ref=e1038]:
              - spinbutton "Period Number" [ref=e1039]
              - generic: Period Number
            - generic [ref=e1044]:
              - generic [ref=e1045]:
                - combobox "period Type" [ref=e1047] [cursor=pointer]
                - generic:
                  - generic: period Type
              - generic [ref=e1049]: arrow_drop_down
            - generic [ref=e1054]:
              - generic [ref=e1055]:
                - combobox "Condition Order" [ref=e1057] [cursor=pointer]
                - generic:
                  - generic: Condition Order
              - generic [ref=e1059]: arrow_drop_down
          - generic [ref=e1062]:
            - generic [ref=e1063]: "Set Reminderdate2 to :"
            - generic [ref=e1069]:
              - spinbutton "Period Number" [ref=e1070]
              - generic: Period Number
            - generic [ref=e1075]:
              - generic [ref=e1076]:
                - combobox "period Type" [ref=e1078] [cursor=pointer]
                - generic:
                  - generic: period Type
              - generic [ref=e1080]: arrow_drop_down
            - generic [ref=e1085]:
              - generic [ref=e1086]:
                - combobox "Condition Order" [ref=e1088] [cursor=pointer]
                - generic:
                  - generic: Condition Order
              - generic [ref=e1090]: arrow_drop_down
          - generic [ref=e1093]:
            - generic [ref=e1094]: "Set Reminderdate3 to :"
            - generic [ref=e1100]:
              - spinbutton "Period Number" [ref=e1101]
              - generic: Period Number
            - generic [ref=e1106]:
              - generic [ref=e1107]:
                - combobox "period Type" [ref=e1109] [cursor=pointer]
                - generic:
                  - generic: period Type
              - generic [ref=e1111]: arrow_drop_down
            - generic [ref=e1116]:
              - generic [ref=e1117]:
                - combobox "Condition Order" [ref=e1119] [cursor=pointer]
                - generic:
                  - generic: Condition Order
              - generic [ref=e1121]: arrow_drop_down
          - generic [ref=e1124]:
            - generic [ref=e1125]: "Set Reminderdate4 to :"
            - generic [ref=e1131]:
              - spinbutton "Period Number" [ref=e1132]
              - generic: Period Number
            - generic [ref=e1137]:
              - generic [ref=e1138]:
                - combobox "period Type" [ref=e1140] [cursor=pointer]
                - generic:
                  - generic: period Type
              - generic [ref=e1142]: arrow_drop_down
            - generic [ref=e1147]:
              - generic [ref=e1148]:
                - combobox "Condition Order" [ref=e1150] [cursor=pointer]
                - generic:
                  - generic: Condition Order
              - generic [ref=e1152]: arrow_drop_down
          - generic [ref=e1155]:
            - generic [ref=e1156]: "Set Start date to :"
            - generic [ref=e1162]:
              - spinbutton "Period Number" [ref=e1163]
              - generic: Period Number
            - generic [ref=e1168]:
              - generic [ref=e1169]:
                - combobox "period Type" [ref=e1171] [cursor=pointer]
                - generic:
                  - generic: period Type
              - generic [ref=e1173]: arrow_drop_down
            - generic [ref=e1178]:
              - generic [ref=e1179]:
                - combobox "Condition Order" [ref=e1181] [cursor=pointer]
                - generic:
                  - generic: Condition Order
              - generic [ref=e1183]: arrow_drop_down
          - generic [ref=e1186]:
            - generic [ref=e1187]: "Set End date to :"
            - generic [ref=e1193]:
              - spinbutton "Period Number" [ref=e1194]
              - generic: Period Number
            - generic [ref=e1199]:
              - generic [ref=e1200]:
                - combobox "period Type" [ref=e1202] [cursor=pointer]
                - generic:
                  - generic: period Type
              - generic [ref=e1204]: arrow_drop_down
            - generic [ref=e1209]:
              - generic [ref=e1210]:
                - combobox "Condition Order" [ref=e1212] [cursor=pointer]
                - generic:
                  - generic: Condition Order
              - generic [ref=e1214]: arrow_drop_down
          - generic [ref=e1217]:
            - generic [ref=e1218]: "Set Due date to :"
            - generic [ref=e1224]:
              - spinbutton "Period Number" [ref=e1225]
              - generic: Period Number
            - generic [ref=e1230]:
              - generic [ref=e1231]:
                - combobox "period Type" [ref=e1233] [cursor=pointer]
                - generic:
                  - generic: period Type
              - generic [ref=e1235]: arrow_drop_down
            - generic [ref=e1240]:
              - generic [ref=e1241]:
                - combobox "Condition Order" [ref=e1243] [cursor=pointer]
                - generic:
                  - generic: Condition Order
              - generic [ref=e1245]: arrow_drop_down
          - generic [ref=e1248]:
            - generic [ref=e1249]: "Set Versionreminderdate1 to :"
            - generic [ref=e1255]:
              - spinbutton "Period Number" [ref=e1256]
              - generic: Period Number
            - generic [ref=e1261]:
              - generic [ref=e1262]:
                - combobox "period Type" [ref=e1264] [cursor=pointer]
                - generic:
                  - generic: period Type
              - generic [ref=e1266]: arrow_drop_down
            - generic [ref=e1271]:
              - generic [ref=e1272]:
                - combobox "Condition Order" [ref=e1274] [cursor=pointer]
                - generic:
                  - generic: Condition Order
              - generic [ref=e1276]: arrow_drop_down
          - generic [ref=e1279]:
            - generic [ref=e1280]: "Set Versionreminderdate2 to :"
            - generic [ref=e1286]:
              - spinbutton "Period Number" [ref=e1287]
              - generic: Period Number
            - generic [ref=e1292]:
              - generic [ref=e1293]:
                - combobox "period Type" [ref=e1295] [cursor=pointer]
                - generic:
                  - generic: period Type
              - generic [ref=e1297]: arrow_drop_down
            - generic [ref=e1302]:
              - generic [ref=e1303]:
                - combobox "Condition Order" [ref=e1305] [cursor=pointer]
                - generic:
                  - generic: Condition Order
              - generic [ref=e1307]: arrow_drop_down
          - generic [ref=e1310]:
            - generic [ref=e1311]: "Set Versionreminderdate3 to :"
            - generic [ref=e1317]:
              - spinbutton "Period Number" [ref=e1318]
              - generic: Period Number
            - generic [ref=e1323]:
              - generic [ref=e1324]:
                - combobox "period Type" [ref=e1326] [cursor=pointer]
                - generic:
                  - generic: period Type
              - generic [ref=e1328]: arrow_drop_down
            - generic [ref=e1333]:
              - generic [ref=e1334]:
                - combobox "Condition Order" [ref=e1336] [cursor=pointer]
                - generic:
                  - generic: Condition Order
              - generic [ref=e1338]: arrow_drop_down
          - generic [ref=e1341]:
            - generic [ref=e1342]: "Set Versionreminderdate4 to :"
            - generic [ref=e1348]:
              - spinbutton "Period Number" [ref=e1349]
              - generic: Period Number
            - generic [ref=e1354]:
              - generic [ref=e1355]:
                - combobox "period Type" [ref=e1357] [cursor=pointer]
                - generic:
                  - generic: period Type
              - generic [ref=e1359]: arrow_drop_down
            - generic [ref=e1364]:
              - generic [ref=e1365]:
                - combobox "Condition Order" [ref=e1367] [cursor=pointer]
                - generic:
                  - generic: Condition Order
              - generic [ref=e1369]: arrow_drop_down
          - generic [ref=e1375]:
            - generic [ref=e1377]:
              - generic [ref=e1378]: Set
              - generic [ref=e1383]:
                - generic [ref=e1384]:
                  - combobox "User Field" [ref=e1386] [cursor=pointer]
                  - generic:
                    - generic: User Field
                - generic [ref=e1388]: arrow_drop_down
              - generic [ref=e1389]: "to :"
            - generic [ref=e1395] [cursor=pointer]:
              - generic [ref=e1396]:
                - combobox "User Role" [ref=e1398]
                - generic:
                  - generic: User Role
              - img [ref=e1400]
            - generic [ref=e1407]:
              - generic [ref=e1408]:
                - combobox "Contact" [ref=e1410] [cursor=pointer]
                - generic:
                  - generic: Contact
              - generic [ref=e1412]: arrow_drop_down
            - button [ref=e1414] [cursor=pointer]:
              - img [ref=e1416]: add
        - generic [ref=e1418]:
          - button "Cancel" [ref=e1419] [cursor=pointer]:
            - generic [ref=e1421]: Cancel
          - button "Save" [ref=e1422] [cursor=pointer]:
            - generic [ref=e1424]: Save
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