# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: E2E_Tests/FC018_questionnaire.spec.ts >> FC_018_Questionnaire Flow >> Configure questionnaire with 'Complete questionnaire without warning' and verify 'Update linked items of type' action is executed when Question condition is triggered on 'Completing the page' and check Questionnaire 'Disable' action
- Location: tests/E2E_Tests/FC018_questionnaire.spec.ts:31:9

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: locator('span').filter({ hasText: 'Risk:' }).last()
Expected: visible
Timeout: 15000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 15000ms
  - waiting for locator('span').filter({ hasText: 'Risk:' }).last()

```

```yaml
- main:
  - img
  - img
  - textbox "Valid email address"
  - textbox "User password"
  - text: Have you forgotten your password?
  - button "LOGIN" [disabled]
  - text: For the best user experience, we recommend the use of the Google Chrome browser or Safari
```

# Test source

```ts
  81  | 
  82  |         await test.step('Configure questionnaire conditions', async () => {
  83  |             await editPage.clickOnQuestionnaireConditionsTab();
  84  |             await questionnaireConditionsPage.createNewConditionTabWithData(questionnaireConditions.tabs.tab1);
  85  |             await questionnaireConditionsPage.addConditionToTabWithData(questionnaireConditions.conditions.condition1);
  86  |             await questionnaireConditionsPage.addConditionToTabWithData(questionnaireConditions.conditions.condition2);
  87  |             await questionnaireConditionsPage.clickOnFirstCondition();
  88  |             await questionnaireConditionsPage.createConditionRules(questionnaireConditions.conditionOn);
  89  |             await questionnaireConditionsPage.createActionRules(questionnaireConditions.actionType);
  90  |         });
  91  | 
  92  |         await test.step('Configure indicators', async () => {
  93  |             await editPage.clickOnIndicatorsTab();
  94  |             await indicatorsPage.configureIndicators(indicators);
  95  |         });
  96  | 
  97  |         await test.step('Publish questionnaire', async () => {
  98  |             await editPage.clickOnPublishOrEdit();
  99  |             await editPage.verifyQuestionnaireIsPublished();
  100 |         });
  101 | 
  102 |         await test.step('Navigate to risk management and link questionnaire', async () => {
  103 |             await leftNav.clickOnDashboard();
  104 |             await leftNav.hoverOnNotifications();
  105 |             await navigationHelper.navigateToCompanyDashboard('Qualitlabs');
  106 |             await environmentsPage.clickOnEnvironment("QualiTlabs Hyd");
  107 |             await leftNav.clickOnModules();
  108 |             await leftNav.clickOnRisksModule();
  109 |         });
  110 | 
  111 |         await test.step('Create risk and link questionnaire', async () => {
  112 |             await risksPage.clickOnAddNewRiskBtn();
  113 |             fc018Data.risk.name = uniqueRiskName;
  114 |             await risksPage.createNewRiskWithData(fc018Data.risk);
  115 |             await risksPage.clickDialogueTab();
  116 |             await risksPage.linkQuestionnaireToRisk(uniqueName, 'QA Automation');
  117 |             await risksPage.verifyAddedQuestionnaireLinked(uniqueName);
  118 |         });
  119 | 
  120 |         await test.step('Navigate to risk tab and link a new item', async () => {
  121 |             await risksPage.clickOnRisksTab();
  122 |             await risksPage.clickOnGridView();
  123 |             await risksPage.clickOnAddNewRiskBtn();
  124 |             fc018Data.risk.name = uniqueRiskName + 'New';
  125 |             await risksPage.createNewRiskWithData(fc018Data.risk);
  126 |         });
  127 |         const question1Locator = page.locator(`[data-test-mo-question-name="${questions.Label.Question.labelTitle}"]`);
  128 |         const question2Locator = page.locator(`[data-test-mo-question-name="${questions.Text1.Question.questionName}"]`);
  129 | 
  130 |         await test.step('Open questionnaire and verify all questions visible', async () => {
  131 |             await risksPage.clickDialogueTab();
  132 |             await risksPage.clickOnQuestionnaire(uniqueName);
  133 | 
  134 |             await expect(question1Locator).toBeVisible();
  135 |             await expect(question2Locator).toBeVisible();
  136 |         });
  137 | 
  138 |         await test.step('Verify next button is enabled', async () => {
  139 |             await risksPage.verifyNextButtonIsEnabled();
  140 |         });
  141 | 
  142 |         await test.step('Verify Standard answer is set', async () => {
  143 |             await expect(question2Locator.getByRole('textbox').first()).toHaveValue(questions.Text1.Question.standardAnswer);
  144 |         });
  145 | 
  146 |         await test.step('Verify Complete without warning setting applied', async () => {
  147 |             await risksPage.clickCompleteAndNextButton();
  148 |             await risksPage.clickCompleteButton();
  149 |             await risksPage.verifyWarningMessageNotDisplayed();
  150 |             await risksPage.verifyQuestionnaireIsFinished(uniqueName);
  151 |         });
  152 | 
  153 |         await test.step('verify disable action executed when questionnaire condition is met', async () => {
  154 |             await risksPage.clickOnSettingsIcon();
  155 |             await risksPage.clickOnMoreOptionsInCard(uniqueName);
  156 |             await risksPage.clickConditionSettingMenuItem();
  157 |             await risksPage.clickQuestionnaireConditionsTab();
  158 | 
  159 |             await expect(page.locator('md-switch').filter({ hasText: questionnaireConditions.conditions.condition2.name }))
  160 |                 .toHaveAttribute('aria-checked', 'false');
  161 |             await risksPage.clickOkButton();
  162 |         });
  163 | 
  164 |         await test.step('verify Update linked item of type action executed when question condition is met', async () => {
  165 |             await risksPage.clickOnRelatedTab();
  166 |             const linkedItem = {
  167 |                 select: fc018Data.risk.name,
  168 |                 settings: {
  169 |                     status: questionConditions.actionType[0].settings.status
  170 |                 }
  171 |             }
  172 |             await risksPage.verifyRelatedTabHasRisk(linkedItem);
  173 |         });
  174 | 
  175 |         await test.step('Verify Indicators added Succesfully', async () => {
  176 |             await risksPage.clickKeyIndicatorTab();
  177 |             await risksPage.verifyIndicatorIsDisplayedInIndicatorTab(indicators[0].name);
  178 | 
  179 |             await risksPage.clickGrossRiskTab();
  180 |             await page.reload();
> 181 |             await expect(page.locator('span').filter({ hasText: 'Risk:' }).last()).toBeVisible({ timeout: 15000 });
      |                                                                                    ^ Error: expect(locator).toBeVisible() failed
  182 |             await page.waitForTimeout(5000);
  183 |             await risksPage.verifyIndicatorIsDisplayedInGrossRiskTab(indicators[0].name);
  184 |         });
  185 | 
  186 |     });
  187 | });
  188 | 
```