# How to process an internal payroll in Labour Hire

This section contains information relating to Internal Payroll Processing:

- [Entering New Employees](#entering-new-employees)
  - [Employee Card](#employee-card)
  - [Payroll Employee Card](#payroll-employee-card)
- [Processing Pays](#payroll-processing)
  - [Pay Journals](#payroll-processing-pay-journals)
  - [Enter Leave Adjustments](#payroll-processing-enter-any-leave-adjustments)
  - [Calculating Pays](#payroll-processing-calculate-pays)
  - [Entry Validation Reports](#payroll-processing-entry-validation-reports)
  - [Uncalculating Pays](#payroll-processing-uncalculating-pays)
  - [Creating a Bank Transfer File](#payroll-processing-create-bank-transfer-file)
  - [Post and Print Pay Advices](#payroll-processing-post-and-print-pay-advices)
  - [Close Pay Periods](#payroll-processing-close-pay-periods)


# INTERNAL PAYROLL PROCESSING OVERVIEW

All internal staff will be entered into the Human Resources and Payroll modules of Dynamics NAV.

# PROCESS SUMMARY:

## Entering New Employees

1.	Receive employee application and enter relevant details into Dynamics NAV. 
2.	Enter new employee information into the Human Resources module.  Go to the following menu: *Departments/Payroll/Employee Maintenance/Employees*
3.  Enter the new employee into the Payroll module. Go to the following menu: *Departments/Payroll/Employee Maintenance/Payroll Employees*
4.  Enter in Bank Details.  To access the Bank Details task, select the **Pay Dissections** icon. 
5.  Enter in Pay Rates in as an hourly rate.  To access the Bank Details task, select the **Pay Rates** icon. 
6.  Enter in Permanent Pay and Allowances.  To access the Pay and Allowances task, select the **Gross & Allowances** icon. 
7.  Enter in Permanent Deductions.  To access the Deductions task, select the **Deductions** icon. 
8.  Enter in Superannuation Fund.  To access the Superannuation task, select the **Superannuation** icon. 
9.  Enter in Employer On Costs such as Payroll Tax, Superannuation or Workers Compensation.  To access the Employer On Costs task, select the **Accumulation Calculations** and select the **Employer On Costs** icon. 
10. Review or add new leave accrual types such as Annual Leave , Sick Leave and Long Service Leave.  To access the Leave Accrual task,       select the **Accruals** task icon.
11. After you have completed these steps, you are ready to process pays.

[Enter New Employee[(#employee-card)
[Enter New Payroll Employee](#payroll-employee-card)

[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

## Processing Pays

1.  Receive timesheets including Leave and /or pay adjustments for employees.
2.  As an optional task, you can specify a particular payroll to work in.  Go into *Departments/Payroll/Payroll Processing/Payroll Selection* and select the Payroll.  (**Note:** If you perform this task, you can release this filter by coming back into this area and selecting the **Clear Selection** icon and this will release the filter and allow you to access all the Payrolls you have User Access to.
3.  Go into *Departments/Pay Journal/Pay Processing/Pay Journal* and enter in the leave adjustments. 
4.  Once the adjustments are complete, select the **Calculate Pays** function.  Enter the **Pay Date** and select **OK**. 
5.  Run the **Entry Validation Report** , select print preview to check for errors and warnings on the screen, when all clear, **Print the report** or save as a .PDF. 
6.  Select **Create Bank Transfer File** to create an EFT file. This can be saved to a file path. The **Bank Transfer Listing** report will print automatically at this stage. This should be filed with the **Entry Validation Report**.
7.  Select **Post**. This will post the pays into the payroll history areas and print payslips. 
8.  After journal has been successfully posted, you will receive a message about closing the pay period.  You can leave this open if there are any additional adjustments that may need to be processed in this period, otherwise, you can close the period, ready for the next period. 

[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

# PROCESS DETAIL

## Entering New Employees - Human Resources

### Employee Card

1. In the **Search** box, enter in **Employees**, and then choose the related link.  Or go to the following menu:*Departments/Payroll/Employee Maintenance/Employees* 
 
2. Click on the **New** button. The cursor will be in the **Employee No** field on the **General** FastTab. Press **OK** or tab to the next field and a New Employee number will be allocated.  Alternatively you can enter in a user specific number.

3.  On the **General** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Job Title**|Enter the Person’s Job Title.|
|**First Name**|Enter the Employee’s First Name.|
|**Last Name**|Enter the Employee’s Last Name.|
|**Address**|Enter in the Employee’s Address Details.|
|**Post Code / City**|Enter in the Employee’s Post Code e.g. 2000.|
|**Sate / Country Code**|Enter in **AUS**.|
|**Phone Number**|Enter in the employee’s home phone number if known.|
|**Gender**|Select **Male** or **Female**.|
|**Marital Status**|If the Marital Status is known, select the appropriate code.|

4.  On the **Communication** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Extension**|Enter the employee’s work extension number if applicable.|
|**Mobile Phone No**|Enter the employee’s mobile phone number if applicable.|
|**Phone No.**|The employee’s phone number will default if entered on the General FastTab.|
|**E-mail**|Enter the employee’s email address. This will be required if intending on emailing the employee’s pay advice.|

5.  On the **Administration** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Employment date**|Enter the employee’s employment or start date. This field is a mandatory field, if nothing is entered will cause issues when calculating pays.|
|**Status**|This will default to **Active**.|

6.  On the **Personal** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Birth Date**|Enter the employee’s birth date.|

[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

## Entering New Employees – Payroll Module

### Payroll Employee Card

After employees are entered into the Human Resources module they are then entered into the Payroll module. All employee maintenance such as updates to pay details, bank details and tax information is maintained on the Payroll Employee Card.

1. In the **Search** box, enter in **Payroll Employees**, and then choose the related link.  Or go to the following menu:*Departments/Payroll/Employee Maintenance/Payroll Employees* 
 
2. On the Payroll Employee Card, click on the **New** icon to create a new record and go to the **Employee No.** field.  From the Employee List, select the employee you wish to continue entering the details for Payroll.  Once the New Employee has been selected, **Press Enter** and the information that was entered intot he Human Resoures Employee Card will default tot he relevant fields in the Payroll Employee Card.  
 
3.  On the **General** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Payroll No**|Select the appropriate Payroll No. from the **ArrowDown**.  You will receive a message requesting whether you want to change the Employee to the Payroll No. you have selected. Click **Yes**.|
|**Emp Type Code**|Select the Employee Type Code from **ArrowDown**.|
|**Payment Method**|Confirm the Payment Method has been changed to **EFT**. This will default to the Defaults on the Payroll Setup Card.|
|**Email Pay Advice**|If Pay advices will be sent via email, check this field. The employee’s email address must be entered in the Human Resources field, otherwise you will not be able to email the pay advice.|
|**Email Payment Summaries**|If Payment Summaries will be sent via email, check this field. The employee’s email address must be entered in the Human Resources field, otherwise you will not be able to email the pay advice.|
|**Timesheet Reminder**|The Timesheet Reminder field will default to **Yes**. Uncheck this field.|

4.  On the **Posting** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Branch Code**|Select the relevant Branch Code from the **ArrowDown**.|
|**Global Dimension 1 &2**|Select the relevant Dimension Codes from the **ArrowDown**. This will usually be the same as the Branch Code.|

5.  On the **Tax** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Tax Scale No**|The Tax Scale No. will default from the Payroll setup card and can be overridden.|
|**HELP Debt**|Select this field if advised on the declaration form.|
|**Student Loan ( SFSS )**|Select his field if advised on the declaration form.|
|**Fixed Tax Rate Applicable**|This Field needs to be selected and ticked.|
|**Fixed Tax Rate Valid Until Date**|The Valid Until Date will be supplied from the ATO and needs to be entered in this field.|
|**Fixed Tax Rate**|The ATO will supply a letter detailing the fixed Tax rate amount.|

6.  On the **Declaration** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Resident**|Select this field if advised on the Declaration Form.|
|**Tax Free Threshold Claimed**|Select this field if advised on the Declaration Form.|
|**HELP Debt**|Select this field if advised on the Declaration Form.|
|**Student Loan**|Select this field if advised on the Declaration Form.|
|**Claim Pension Rebate**|Select this field if advised on the Declaration Form.|
|**Use TFN for Superannuation**|Select this field if advised on the Declaration Form.|
|**Rebate Amount Claimed**|Select this field if advised on the Declaration Form.|
|**Tax.File No**|Enter the employee’s Tax File No. the format for this field is a maximum of 9 characters.|
|**Birth Date**|This field will populate from the HR Employee card.|
|**Date Declaration Signed**|Enter in the Date Declaration Signed from the Employment Declaration form.|
|**Payee Signature**|If the employee has signed the Employment Declaration form, check this field.|
|**Declaration Lodged**|This field will be populated with a date once the Declaration File Generation has been processed.|

7.  Information on the **Work Cover** FastTab is only completed for Incorporated Company contractors.

[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

### Payroll Employee Card Pay Dissections

Employee Bank accounts are entered in the Pay Dissections area.  

1.  To enter in Employee Bank accounts, select the **Pay Dissections** icon on the **Navigate** ribbon. 

2.  Fill the fields as described in the following table.

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Transaction Type Code**|Transaction Type Code 9999 will default in this field.|
|**Pay Dissection Type**|There are 2 types of dissections: * **Main** – Used to identify the main bank account, * **Part** – Used to identify additional bank accounts.|
|**Bank Account No.**|Enter the employee’s bank account number. This field has a limit of 9 characters which should be entered as follows: 123456789.|
|**Bank Name**|This will default to the employee’s name and can be overridden accordingly.|
|**EFT Bank No.**|Enter in the employee’s BSB no. This field has a limit of 7 characters which should be entered as follows: 032-170.|
|**Standard Amount / Standard %**|If the employee has nominated an additional account, enter in the Amount or the Percentage as nominated by the employee.|

[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

### Payroll Employee Card Pay Rates

1.  To enter in Pay Rates in as an hourly rate, select the **Pay Rates**” icon on the **Navigate** ribbon. 
 
 2. Fill the fields as described in the following table.
 
|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Employee start Date**|This field should default to the Employee’s Start Date.|
|**Classification Code**|Click on the **ArrowDown** and select the award associated with the employee.|
|**Employee Rate**|Enter in the Employee’s rate as an hourly amount.|

After you have updated the rate, go to the **Rate** FastTab where the rate will be updated accordingly. (This will only be updated if the Pay Period is after the Employee’s Start Date).

[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

### Payroll Employee Card Gross / Allowances

It is assumed that Internal Employees are **Auto Paid**. To automatically generate hours, Ordinary / Normal Time should be set up as a permanent occurrence. The same applies if the employee is to receive an allowance on a permanent basis.

1.  To enter in the Pay and Allowances, select the **Gross & Allowances** icon on the **Navigate** ribbon.  

2.  Fill the fields as described in the following table.

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Transaction Type Code**|Select the Transaction Type Code from the **ArrowDown** e.g. Ordinary Time or a Permanent Allowance.|
|**Start Date**|Enter in a Start Date of when the Allowance transaction should commence. If this is for Ordinary of Normal Hours there is no need to enter in a Start Date.|
|**Description**|The Description will default from the Transaction. You can override the description should you require a user defined description to print on the Pay Advice.|
|**Units**|Enter in the number of units required to be generated. For Ordinary / Normal Time type transactions you can enter in the number of hours per the pay period. |
|**Fixed Value**|Enter in the Fixed Value for allowance type transaction if required.|
|**Hourly Rate**|This will default from the Pay Rate table for Ordinary / Normal Time type transactions.|
|**Pay Value**|This will be the sum of the Units field * Hourly Rate field.|
|**Not Used**|The Not Used field is used to suppress the permanent transaction for a single pay only. When the pay period is closed on a payroll, this flag is then removed and ready to be generated for the next period.|

[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

### Payroll Employee Card Deductions

The Deductions Area is used to setup permanent deductions.

1.  To setup Deductions, select the **Deductions** icon on the **Navigate** ribbon.

2.  Fill the fields as described in the following table.

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Transaction Type Code**|Select the Transaction Type Code from the **ArrowDown**.|
|**Priority**|If there are a number of deductions, you can select the order in which they are deducted, by entering 1,2,3, etc. for each transaction type.|
|**Start Date**|Enter in a Start Date of when the Deduction transaction should commence.|
|**Description**|The Description will default from the Transaction. You can override the description should you require a user defined description to print on the Pay Advice.|
|**Standard Amount / Standard %**|Enter in a Standard Amount or Standard % of the deduction.|
|**Details**|Enter in a Reference number for the deduction.|
|**Total Deduction**|If the Deduction is to cease as soon as it reaches a certain amount, enter in this amount here.|
|**LTD Amount**|This field is a sum of all the deductions to date.|
|**Not Used**|The Not Used field is used to suppress the permanent transaction for a single pay only. When the pay period is closed on a payroll, this flag is then removed and ready to be generated for the next period.|

[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

### Payroll Employee Card Superannuation 

1.  To setup Superannuation, select the **Superannuation** icon on the **Navigate** ribbon.

2.  Fill the fields as described in the following table.

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Superannuation Company Code**|Select the Superannuation Company code from the **ArrowDown**.|
|**Membership No.**|Enter in the Membership No. if known.|
|**Date Joined Fund**|The **Date Joined Fund** date will default to the Employee’s start date. If this date differs from the Employee start date, enter in the stat date for the Superannuation Fund.|
|**Employer Standard %**|The employer standard percentage will default to the value setup on the Superannuation Company card.|

[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

#### Superannuation Employee Choice (Changing Superannuation Funds)

The following procedures should be undertaken if an employee elects to change their fund.

1.  Changing Superannuation funds - enter an end date on the old fund and change the 9.5% to zero amount.
2.  Add the new fund on a new line with the current month in the start date, then add the employer standard 9.5%.

If you are updating the employee’s Superannuation fund and your organisation is calculating Employer liabilities using On Costs, you must ensure that you update the Superannuation Code on the [Superannuation On Cost transaction type](#payroll-employee-card-on-cost-transactions).  

[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

### Payroll Employee Card Leave Accruals

Dependent upon what is setup on the Payroll (Pay Cycles) card, will depend upon whether the leave accruals will default to the Payroll Employee card when the employee is assigned to the Payroll.

1.  To review or setup the Leave Accruals, select the **Accruals** icon from the **Navigate** ribbon.  A list of the Leave Accruals for the employee will appear for viewing purposes.

2.  If you wish to create or add a new Leave Accrual, click on the **New** icon and fill the fields as described in the following table.

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Leave Type**|Select the Leave Type code from the **ArrowDown**.|
|**Leave Code**|Select the appropriate Leave Code from the **ArrowDown**.|
|**Start Date**|The **Starting Date** will default to the employees start date. This date is the Employee leave Accrual Start Date.|
 
[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

### Payroll Employee Card On Cost Transactions

If your organisation has chosen to calculate On Cost transactions, you will need to add in the relevant On Cost Transactions so that they are generated during the calculation of pays.  

1.  To setup Employer On Costs, select on the **Employer On Costs** icon, from the **Accumulation Calculations** on the **Navigate** ribbon.  
  
2.  Fill the fields as described in the following table.

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Transaction Type Code**|Select the Transaction Type code from the **ArrowDown**.|
|**Start Date**|The **Start Date** field is used to specify the date at which the On Cost transaction is to commence.|
|**End Date**|The **End Date** field is used to specify the date at which the On Cost transaction is to end.|
|**Pay Rate**|The **Pay Rate** field is used to retain the calculation rate of the On Cost transaction.  This amount entered into this field should be expressed in decimal format.  E.g. If the value is 9%, it should be entered as 0.09.|
|**Superannuation Code**|The **Superannuation Code** field is used to nominate the Contractor’s Superannuation code.  This is only applicable if this On Cost transaction relates to the SGC accrual.|
|**Not Used**|If this field is ticked the Pay Transaction Type is not applied to the “current” pay period only.  The flag will be reset for the next pay period.|

[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

# PAYROLL PROCESSING

## Payroll Processing Pay Journals

To access the Pay Journals task, go to the following menu: *Departments/Pay Journal/Pay Processing/Pay Journal*

## Payroll Processing Enter any leave adjustments

1.  In the **Pay Journal** section enter in any leave taken for auto paid employee. 
 
2.  To enter leave against a specific employee, at a minimum fill the fields as described in the following table.  

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**No.**|Select the Employee’s No. from the **ArrowDown**.|
|**Transaction Type Code**|Enter or select the Transaction Type code for the Leave Type from the **ArrowDown**.|
|**From Date**|Enter in the Start Date of the absence in this field.(**You will need to update your display settings if this field is not displaying**).|
|**To Date**|Enter in the End Date of the absence in this field.(**You will need to update your display settings if this field is not displaying**).|
|**Units**|Enter in the No. of Hours in this field.|
|**Subtract From Permanent Hours**|This field will automatically default from the setup of the Pay Transaction Type card.  If the field is ticked, the value of this leave transaction will be deducted from the Employee’s standard auto-pay. If the field is not ticked, the value of this leave transaction will be paid in addition to the Employee’s standard auto-pay.|

3.  After entering your leave/temporary adjustments, the auto-pays can be calculated.

[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

## Payroll Processing Calculate Pays

1.  In the Pay Journal, select **Calculate Pays** to calculate your pays and enter the **Pay Date** and select **OK**.   

2.  During this process any permanent hours and deductions, leave accruals, tax and superannuation is generated.  Please note : Pays can be calculated by individual or by all employees.

[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

## Payroll Processing Entry Validation Reports

Once pays have been calculated, the Entry Validation report has to be printed. You can preview the report online first for any errors or warnings which need to be fixed before proceeding to the next step. 

1.  Select the **Entry Validation report** icon on the **Home** ribbon.  

2.  Select **Print Preview** to check for errors and warnings on the screen, when all clear, **Print** the report or save as a **.PDF**. 

3.  If errors are found on the Entry Validation Report, the individual’s pay can be fixed by uncalculating the pay. Please see the next step for **uncalculating Pays**.
 
[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

## Payroll Processing Uncalculating Pays

Pays can be uncalculated for individual employees or for all employees within the Pay Journal. 

1.  To **uncalculate** the pays, select the **Actions** ribbon and select **Cancel Calculated Pays**.
 
 [GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)
 
## Payroll Processing Create Bank Transfer File

When the Entry Validation report has been checked and found to be correct, run the create bank transfer file process. 

1.  To create the file, select the **Create Bank Transfer File** icon on the **Home** ribbon. 

2.  Fill the fields as described in the folllowing table.
 
|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Employee No.**|You can create a bank transfer file for one employee by nominating the Employee’s number from the **ArrowDown**.  Otherwise leave it blank to create a bank file for all employees.|
|**Bank Account**|The Bank Account attached to the Payroll will default from the Payroll Card. Otherwise select another bank account from the **ArrowDown**.|
|**Process Date**|This will be the **Processing Date** when the file will be processed by the Bank. The date should be today’s date or greater.|
|**Description**|Enter in a Description for the file.|
|**File Name**|You can specify where you would like to save the file by clicking on the **AssistButton**.  You must ensure that you save the file with an .aba extension.|
|**Print Transfer Listing**|This field will automatically be selected and will provide you with an option to **Print** or **Preview** the Bank Transfer Listing Report. (**If you do not print this report, it can be re-printed at a later stage**).|

3.  Pay advices are automatically flagged as paid. If for any reason you need to re-run the transfer again, select the
**Cancel Bank Transfer** process and redo. 
  
[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

## Payroll Processing Post and Print Pay Advices

When bank files for each batch of pays has been processed, the payroll journals should be posted. This clears them from the Pay Journal area and writes the data to the employee pay history ledgers.
 
1.  Select the **Post** option, and the **Print Pay Advice** message will appear as part of the posting process.
 
2.  To print or reprint payslips, go to the following menu:  *Departments/Payroll/Payroll Processing/ Print Pay Advices*

3.  Fill the fields described in the following table.
 
|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Payroll No.**|From the **ArrowDown**, select the Payroll you wish to re-print pay advices for.|
|**Period No.**|From the **ArrowDown**, select the Period No. you wish to re-print the pay advices for.|

 
1.  To email payslips, go to the following menu: *Departments/Payroll/Payroll Processing/ E-Mail Pay Advices* 

2.  On the **Options** FastTab, fill the fields as described in the following table.
 
|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Pay Advice Message**|Complete this field if you wish to have a pay advice message printed on the emailed pay advices.|

3.  On the **Posted Pay Advice** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|----------------------------------------|---------------------------------------------------------------------|
|**Employee No.**|From the **ArrowDown**, select the Employee No. otherwise leave this blank to generate email pay advices for all.|
|**Payroll No.**|From the **ArrowDown**, select the Payroll No. otherwise leave this blank to generate email pay advices for all.|
|**Tax Year**|From the **ArrowDown**, select the Tax Year otherwise leave this blank to generate email pay advices for all.|
|**Period No.**|From the **ArrowDown**, select the Period No. otherwise leave this blank to generate email pay advices for all.|
|**No.**|From the **ArrowDown**, select the No. (which relates to the Pay Advice No.) otherwise leave this blank to generate email pay advices for all.|

[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)

## Payroll Processing Close Pay Periods

You can close the pay period independently if you choose not to close the pay period at the time of posting the payroll.  

1.  To Close Pay periods, go to the following menu: *Departments/Payroll/Periodic Activities/Periodic Maintenance/ Close Pay Periods*

2.  Select the **Payroll No.** and press **OK**. 

3.  Select the **Pay Period** by the ticking the **Closed and Date Locked** columns to close the pay period.

[GoToTop](#how-to-process-an-internal-payroll-in-labour-hire)
