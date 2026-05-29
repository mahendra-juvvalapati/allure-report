# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: E2E_Tests/FC029_questionnaire.spec.ts >> FC_029_Questionnaire Flow >> Configure questionnaire with 'Complete questionnaire without warning' and verify 'Set quality state to' action is executed when Question condition is triggered on 'Change a question' and check Questionnaire 'Send mail' action
- Location: tests/E2E_Tests/FC029_questionnaire.spec.ts:31:9

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
  89  |             await questionnaireConditionsPage.addConditionToTabWithData(questionnaireConditions.conditions.condition1);
  90  |             await questionnaireConditionsPage.disablePostSubmission();
  91  |             await questionnaireConditionsPage.createConditionRules(questionnaireConditions.conditionOn);
  92  |             await questionnaireConditionsPage.createActionRules(questionnaireConditions.actionType);
  93  |         });
  94  | 
  95  |         await test.step('Configure indicators', async () => {
  96  |             await editPage.clickOnIndicatorsTab();
  97  |             await indicatorsPage.configureIndicators(indicators);
  98  |         });
  99  | 
  100 |         await test.step('Publish questionnaire', async () => {
  101 |             await editPage.clickOnPublishOrEdit();
  102 |             await editPage.verifyQuestionnaireIsPublished();
  103 |         });
  104 | 
  105 |         await test.step('Navigate to risk management', async () => {
  106 |             await leftNav.clickOnDashboard();
  107 |             await leftNav.hoverOnNotifications();
  108 |             await navigationHelper.navigateToCompanyDashboard('Qualitlabs');
  109 |             await environmentsPage.clickOnEnvironment("QualiTlabs Hyd");
  110 |             await leftNav.clickOnModules();
  111 |             await leftNav.clickOnRisksModule();
  112 |         });
  113 | 
  114 |         await test.step('Create risk and link questionnaire', async () => {
  115 |             await risksPage.clickOnAddNewRiskBtn();
  116 |             fc029Data.risk.name = uniqueRiskName;
  117 |             await risksPage.createNewRiskWithData(fc029Data.risk);
  118 |             await risksPage.clickDialogueTab();
  119 |             await risksPage.linkQuestionnaireToRisk(uniqueName, 'QA Automation');
  120 |             await risksPage.verifyAddedQuestionnaireLinked(uniqueName);
  121 |         });
  122 | 
  123 |         const question1Locator = page.locator(`[data-test-mo-question-name="${questions.text1.Question.questionName}"]`);
  124 |         const question2Locator = page.locator(`[data-test-mo-question-name="${questions.text2.Question.questionName}"]`);
  125 |         const question3Locator = page.locator(`[data-test-mo-question-name="${questions.text3.Question.questionName}"]`);
  126 |         const question4Locator = page.locator(`[data-test-mo-question-name="${questions.text4.Question.questionName}"]`);
  127 | 
  128 | 
  129 |         await test.step('Open questionnaire and verify all questions visible', async () => {
  130 |             await risksPage.clickOnQuestionnaire(uniqueName);
  131 | 
  132 |             await expect(question1Locator).toBeVisible();
  133 |             await expect(question2Locator).toBeVisible();
  134 |         });
  135 | 
  136 |         await test.step('Verify next button is enabled', async () => {
  137 |             await risksPage.verifyNextButtonIsEnabled();
  138 |         });
  139 | 
  140 |         await test.step('Verify mandatory field state', async () => {
  141 |             await risksPage.clickCompleteAndNextButton();
  142 |             await risksPage.verifyMandatoryFieldsErrorMessageDisplayed();
  143 |             await risksPage.clickCloseDialogButton();
  144 |         });
  145 | 
  146 |         await test.step('verify set quality state to action executed when question condition is met', async () => {
  147 |             await question1Locator.getByRole('textbox').fill('mahendra');
  148 |             await question2Locator.click();
  149 |             await risksPage.clickCloseQuestionnaireButton();
  150 |             await risksPage.clickMoDataTab();
  151 |             await risksPage.verifyModataQualityState(questionConditions.actionType[0].actionValue);
  152 |         })
  153 | 
  154 |         await test.step('Verify explanation  is visible', async () => {
  155 |             await risksPage.clickDialogueTab();
  156 |             await risksPage.clickOnQuestionnaire(uniqueName);
  157 |             await risksPage.verifyExplanationOfQuestion(question1Locator, questions.text1.explanationText);
  158 |         })
  159 | 
  160 |         await test.step('Verify readonly field state', async () => {
  161 |             await expect(question2Locator.getByRole('textbox')).toHaveAttribute('readonly');
  162 |         });
  163 | 
  164 |         await test.step('Verify standard answer is set', async () => {
  165 |             await risksPage.clickCompleteAndNextButton();
  166 |             await expect(question3Locator.locator('input[type="number"]')).toHaveValue(questions.text3.Question.standardAnswer);
  167 |         });
  168 | 
  169 |         await test.step('Verify complete questionnaire without warning setting applied', async () => {
  170 |             await question4Locator.getByRole('textbox').fill('mahendra');
  171 |             await risksPage.clickCompleteAndNextButton();
  172 |             await risksPage.clickCompleteButton();
  173 |             await risksPage.verifyWarningMessageNotDisplayed();
  174 |             await risksPage.clickYesButton();
  175 |             await risksPage.verifyQuestionnaireIsFinished(uniqueName);
  176 |         });
  177 | 
  178 |         await test.step.skip('verify send email action executed when questionnaire condition is met', async () => {
  179 |             //need to check Api response
  180 |         })
  181 | 
  182 |         await test.step('Verify Indicators are added Succesfully and verify indicator level', async () => {
  183 |             await risksPage.clickKeyIndicatorTab();
  184 |             await risksPage.verifyIndicatorIsDisplayedInIndicatorTab(indicators[0].name);
  185 |             await risksPage.verifyIndicatorLevelNumberIsDisplayedInIndicatorTab('3');
  186 | 
  187 |             await risksPage.clickGrossRiskTab();
  188 |             await page.reload();
> 189 |             await expect(page.locator('span').filter({ hasText: 'Risk:' }).last()).toBeVisible({ timeout: 15000 });
      |                                                                                    ^ Error: expect(locator).toBeVisible() failed
  190 |             await page.waitForTimeout(5000);
  191 |             await risksPage.verifyIndicatorIsDisplayedInGrossRiskTab(indicators[0].name);
  192 |         })
  193 | 
  194 |         await test.step('Verify Inherit answer from previous Version', async () => {
  195 |             await risksPage.clickDialogueTab();
  196 |             await risksPage.createNewVersion();
  197 |             await risksPage.clickOnQuestionnaire(uniqueName);
  198 |             await question1Locator.getByRole('textbox').fill('mahendra');
  199 |             await question2Locator.click();
  200 |             await risksPage.clickCompleteAndNextButton();
  201 |             await expect(question4Locator.getByRole('textbox')).toHaveValue('mahendra');
  202 |         })
  203 |     });
  204 | });
```