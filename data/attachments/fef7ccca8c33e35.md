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
    31 × locator resolved to <span data-v-395a6c6f="">Warning</span>
       - unexpected value "visible"

```

```yaml
- text: Warning
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