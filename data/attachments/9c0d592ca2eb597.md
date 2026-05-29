# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: E2E_Tests/FC030_questionnaire.spec.ts >> FC_030_Questionnaire Flow >> Configure questionnaire with 'External user can finish the questionnaire' and verify 'Calculate all linked kpis' action is executed when Question condition is triggered on 'Completing the page' and check Questionnaire 'Generate report and send to service' action
- Location: tests/E2E_Tests/FC030_questionnaire.spec.ts:47:9

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
  148 |             await editPage.verifyQuestionnaireIsPublished();
  149 |         });
  150 | 
  151 |         await test.step('Navigate to risk management and link questionnaire', async () => {
  152 |             await leftNav.clickOnDashboard();
  153 |             await leftNav.hoverOnNotifications();
  154 |             await navigationHelper.navigateToCompanyDashboard('Qualitlabs');
  155 |             await environmentsPage.clickOnEnvironment("QualiTlabs Hyd");
  156 |             await leftNav.clickOnModules();
  157 |             await leftNav.clickOnRisksModule();
  158 |         });
  159 | 
  160 |         await test.step('Create risk2 and link questionnaire', async () => {
  161 |             risk.name = risk2;
  162 |             await risksPage.clickOnAddNewRiskBtn();
  163 |             await risksPage.createNewRiskWithData(risk);
  164 |             await risksPage.clickDialogueTab();
  165 |             await risksPage.linkQuestionnaireToRisk(questionnaireName2, 'QA Automation');
  166 |             await risksPage.verifyAddedQuestionnaireLinked(questionnaireName2);
  167 |         });
  168 | 
  169 |         await test.step('Create risk1  and link questionnaire', async () => {
  170 |             risk.name = uniqueRiskName
  171 |             await leftNav.clickOnDashboard();
  172 |             await leftNav.hoverOnNotifications();
  173 |             await navigationHelper.navigateToCompanyDashboard('Qualitlabs');
  174 |             await environmentsPage.clickOnEnvironment("QualiTlabs Hyd");
  175 |             await leftNav.clickOnRisksModule();
  176 |             await page.waitForTimeout(3000);
  177 |             await risksPage.clickOnAddNewRiskBtn();
  178 |             await risksPage.createNewRiskWithData(risk);
  179 |             await risksPage.clickDialogueTab();
  180 |             await risksPage.linkQuestionnaireToRisk(existingQuestionnaire, 'QA Automation')
  181 |             await risksPage.linkQuestionnaireToRisk(questionnaireConfig.QuestionnaireName, 'QA Automation');
  182 |             await risksPage.verifyAddedQuestionnaireLinked(questionnaireConfig.QuestionnaireName);
  183 |             await actions.setPageZoom(80);
  184 |         });
  185 | 
  186 |         await test.step('Link Risk 2 to Risk 1 ', async () => {
  187 |             await risksPage.clickOnRisksTab();
  188 |             await risksPage.linkItemToRisk(risk2);
  189 |             await risksPage.configureKPI(LinkTabKPIs[0]);
  190 | 
  191 |         })
  192 | 
  193 |         const question1Locator = page.locator(`[data-test-mo-question-name="${questions.question1.Question.questionName}"]`);
  194 |         const question2Locator = page.locator(`[data-test-mo-question-name="${questions.question2.Question.questionName}"]`);
  195 |         const question3Locator = page.locator(`[data-test-mo-question-name="${questions.question3.Question.questionName}"]`);
  196 |         const question4Locator = page.locator(`[data-test-mo-question-name="${questions.question4.Question.questionName}"]`);
  197 |         const question5Locator = page.locator(`[data-test-mo-question-name="${questions.question5.Question.questionName}"]`);
  198 | 
  199 |         await test.step('Open questonnaire and verifyall questions are visible', async () => {
  200 |             await risksPage.clickDialogueTab();
  201 |             await risksPage.clickOnQuestionnaire(questionnaireConfig.QuestionnaireName);
  202 |             await expect(question1Locator).toBeVisible();
  203 |             await expect(question2Locator).toBeVisible();
  204 |             await expect(question3Locator).toBeVisible();
  205 | 
  206 |         })
  207 | 
  208 |         await test.step('Verify next button is enabled', async () => {
  209 |             await risksPage.verifyNextButtonIsEnabled();
  210 |         });
  211 | 
  212 |         await test.step('Verify mandatory field state', async () => {
  213 |             await risksPage.clickCompleteAndNextButton();
  214 |             await risksPage.verifyMandatoryFieldsErrorMessageDisplayed();
  215 |             await risksPage.clickCloseDialogButton();
  216 |             await expect(question2Locator.getByText('This field is required!')).toBeVisible();
  217 |         });
  218 | 
  219 | 
  220 |         await test.step('Fill all the questions and complete the page', async () => {
  221 |             let date = await actions.getTodayDateFormatted('DD-MM-YYYY');
  222 |             let time = await actions.getTodayDateFormatted('HH:mm:ss');
  223 | 
  224 |             await question1Locator.getByRole('textbox').click();
  225 |             await actions.type(question1Locator.getByRole('textbox'), date + " " + time);
  226 |             question1Locator.getByRole('textbox').blur();
  227 |             await actions.type(question2Locator.getByRole('textbox'), date);
  228 |             question2Locator.getByRole('textbox').blur();
  229 |             await actions.type(question3Locator.getByRole('textbox'), time);
  230 |             question3Locator.getByRole('textbox').blur();
  231 |             await page.waitForTimeout(2000);
  232 |             await risksPage.clickCompleteAndNextButton();
  233 | 
  234 |         })
  235 | 
  236 |         await test.step('Verify Readonly field state', async () => {
  237 |             await expect(question4Locator).toBeVisible();
  238 |             await expect(question5Locator.getByRole('textbox')).toBeDisabled();
  239 |         });
  240 | 
  241 |         await test.step('Verify All link tab KPIs are calculated on completing the page', async () => {
  242 |             await risksPage.clickCloseQuestionnaireButton();
  243 |             await risksPage.clickKeyIndicatorTab();
  244 |             await risksPage.verifyIndicatorIsDisplayedInIndicatorTab(LinkTabKPIs[0].kpiNameForCalculation);
  245 |             await risksPage.verifyKPICalculatedInIndicatorTab(LinkTabKPIs[0].kpiNameForCalculation);
  246 |             await risksPage.clickGrossRiskTab();
  247 |             await page.reload();
> 248 |             await expect(page.locator('span').filter({ hasText: 'Risk:' }).last()).toBeVisible({ timeout: 15000 });
      |                                                                                    ^ Error: expect(locator).toBeVisible() failed
  249 |             await page.waitForTimeout(5000);
  250 |             await risksPage.verifyIndicatorIsDisplayedInGrossRiskTab(LinkTabKPIs[0].kpiNameForCalculation);
  251 |             await risksPage.verifyKPICalculated(LinkTabKPIs[0].kpiValue, LinkTabKPIs[0].kpiNameForCalculation);
  252 |         });
  253 | 
  254 |         await test.step('Finish Questionnaire', async () => {
  255 |             await risksPage.clickDialogueTab();
  256 |             await risksPage.clickOnQuestionnaire(questionnaireConfig.QuestionnaireName);
  257 |             await risksPage.clickCompleteButton();
  258 |             await risksPage.verifyFinishMessageDisplayed()
  259 |             await risksPage.clickYesButton();
  260 |             await risksPage.verifyQuestionnaireIsFinished(questionnaireConfig.QuestionnaireName);
  261 |         });
  262 | 
  263 |         await test.step('Verify Indicators are added Succesfully', async () => {
  264 |             await risksPage.clickKeyIndicatorTab();
  265 |             await risksPage.verifyIndicatorIsDisplayedInIndicatorTab(indicators[0].name);
  266 |             await risksPage.clickGrossRiskTab();
  267 |             await risksPage.verifyIndicatorIsDisplayedInGrossRiskTab(indicators[0].name);
  268 |         })
  269 | 
  270 |         await test.step.skip('Verify report is generated and send to service action is executed when question condition is met', async () => {
  271 |             await page.locator('[data-test-id="notifications"]').click();
  272 |             const notification = page.locator('[role="listitem"][index="1"]');
  273 |             await expect(notification.getByText('Generate report and send to service', { exact: true }).first()).toBeVisible();
  274 |             await expect(notification.getByText('The report \'Test Report\' will be generated and sent to a service.', { exact: true }).first()).toBeVisible();
  275 |             await notification.getByRole('button', { name: 'Dismiss' }).first().click();
  276 |             await page.locator('.sidebar-backdrop').first().click();
  277 |         });
  278 | 
  279 | 
  280 | 
  281 | 
  282 |     });
  283 | });
```