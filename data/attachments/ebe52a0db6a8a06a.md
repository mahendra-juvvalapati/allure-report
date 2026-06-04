# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: E2E_Tests/FC028_questionnaire.spec.ts >> FC_028_Questionnaire Flow >> Configure questionnaire with 'Disable next button' and verify 'Set version result state to' action is executed when Question condition is triggered on 'Entering the questionnaire the first time' and check Questionnaire 'Calculate all linktab kpis' action
- Location: tests/E2E_Tests/FC028_questionnaire.spec.ts:48:9

# Error details

```
TimeoutError: locator.click: Timeout 15000ms exceeded.
Call log:
  - waiting for getByTestId('Qualitlabs')

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
            - status "60" [ref=e42]
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
            - button "home Dashboard" [active] [ref=e80] [cursor=pointer]:
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
              - button "Impact Assessments" [ref=e145] [cursor=pointer]:
                - img [ref=e146]:
                  - img
                - generic [ref=e147]: Impact Assessments
              - button "Audit sets" [ref=e148] [cursor=pointer]:
                - img [ref=e149]:
                  - img
                - generic [ref=e150]: Audit sets
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
              - button "Arrangements" [ref=e184] [cursor=pointer]:
                - img [ref=e185]:
                  - img
                - generic [ref=e186]: Arrangements
              - button "Insurances" [ref=e187] [cursor=pointer]:
                - img [ref=e188]:
                  - img
                - generic [ref=e189]: Insurances
              - button "Key Figures" [ref=e190] [cursor=pointer]:
                - img [ref=e191]:
                  - img
                - generic [ref=e192]: Key Figures
              - button "Settings" [ref=e193] [cursor=pointer]:
                - img [ref=e194]:
                  - img
                - generic [ref=e195]: Settings
              - button "BCM Activities" [ref=e196] [cursor=pointer]:
                - img [ref=e197]:
                  - img
                - generic [ref=e198]: BCM Activities
              - button "BCM Plans" [ref=e199] [cursor=pointer]:
                - img [ref=e200]:
                  - img
                - generic [ref=e201]: BCM Plans
              - button "Context analysis" [ref=e202] [cursor=pointer]:
                - img [ref=e203]:
                  - img
                - generic [ref=e204]: Context analysis
              - button "Situations" [ref=e205] [cursor=pointer]:
                - img [ref=e206]:
                  - img
                - generic [ref=e207]: Situations
          - generic [ref=e210]:
            - button [ref=e211] [cursor=pointer]:
              - generic [ref=e213]:
                - img [ref=e215]
                - generic [ref=e217]: close
            - menu:
              - generic:
                - generic:
                  - generic:
                    - img
      - generic [ref=e221]:
        - generic [ref=e223]:
          - generic [ref=e224]:
            - generic [ref=e230]:
              - button [ref=e232] [cursor=pointer]:
                - img [ref=e234]: arrow_back
              - generic [ref=e238] [cursor=pointer]: Qualitlabs
            - button [ref=e241] [cursor=pointer]:
              - img [ref=e243]: settings
          - generic [ref=e244]: QualiTlabs Hyd
        - generic [ref=e246]:
          - img [ref=e248]
          - generic [ref=e249]: There are no Dashboards yet!
  - generic:
    - iframe
  - generic:
    - tooltip "Notifications"
```

# Test source

```ts
  1  | import { Page } from '@playwright/test';
  2  | 
  3  | export class NavigationHelper {
  4  |   readonly page: Page;
  5  | 
  6  |   constructor(page: Page) {
  7  |     this.page = page;
  8  |   }
  9  | 
  10 |   async navigateToCompanyDashboard(companyName: string) {
  11 |     const companyDashboard = this.page.getByTestId(companyName);
  12 |     try {
  13 |       await companyDashboard.click();
  14 |     } catch (error) {
  15 |       console.log(error);
> 16 |       await companyDashboard.click();
     |                              ^ TimeoutError: locator.click: Timeout 15000ms exceeded.
  17 |     }
  18 |   }
  19 | }
  20 | 
```