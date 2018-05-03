# How to process an internal payroll in Labour Hire

This document will contain information relating to Internal Payroll Processing encompassing the following sections:


- Entering New Employees
  - Employee Card
  - Payroll Employee Card
- Processing Pays
  - Pay Journals  
  - Enter Leave Adjustmentso Calculating Pays  
  - Entry Validation Reports  
  - Un-calculating Payso Creating a Bank Transfer File  
  - Post and Print Pay Advices  
  - Close Pay Period

## INTERNAL PAYROLL PROCESSING OVERVIEW
All internal staff will be entered into the Human Resources and Payroll modules of Dynamics NAV.
 
## PROCESS SUMMARY

### Entering New Employees

1. Receive employee application and relevant details to enter into Dynamics NAV. 
2. Enter new employee information into the Human Resources module. 

To access the Employee Maintenance task, go to the following menu:

*Departments/Payroll/Employee Maintenance/Employees* 

- Enter the new employee into the Payroll module. To access the Employee Maintenance task Click the “Payroll Employee Card” button or go to the following menu: *Departments/Payroll/Employee Maintenance/Payroll Employees* 
- Enter in Bank Details. To access the Bank Details task, Click the “Pay Dissections” task icon. 
- Enter in Pay Rates in as an hourly rate. To access the Bank Details task, Click the “Pay Rates” task icon. 
- Enter in Permanent Pay and Allowances. To access the Pay and Allowances task, Click the “Gross & Allowances” task icon. 
- Enter in Permanent Deductions. To access the Deductions task, Click the “Deductions” task icon. 
- Enter in Superannuation Fund. To access the Superannuation task, Click the “Superannuation” task icon. 
- Enter in Employer On Costs such as Payroll Tax. To access the Employer On Costs task, Click the “Accumulation Calculations” and select the “Employer On Costs” task icon. 
- Review and Add new leave accrual types such as Annual Leave , Sick Leave and Long Service Leave. To access the Leave Accrual task, Click the “Accruals” task icon.  
- After you have completed these steps, you are then ready to process pays.

### Processing Pays

- Receive timesheets including Leave and /or pay adjustments for employees.
- Go into Departments/Payroll/Payroll Processing/Payroll Selection and select the payroll you wish to work in (note this is optional). 
- Go into Departments/Pay Journal/Pay Processing/Pay Journal and enter in the leave adjustments. After completing entering adjustments, select the “Calculate Pays” function. 
- In the Pay Journal - Select “Calculate Pays” toer File” to create an EFT file. This can be saved to a file path. A “Bank Transfer Listing” report will print automatically at this stage. This should be filed with the “Entry Validation Report”.
- Then select “Post”. This will post the pays into the payroll history areas and print payslips. 

After posting of the journal has occurred, you will be asked if you want to close the pay period. You can leave this open if there are and additional adjustments that may need to be processed in this period, otherwise, you can close the period, ready for the next period.

## PAY PROCESS DETAIL

### Entering New Employees – Human Resources Module

To access the Employee Maintenance task, go to the following menu:

*Departments/Payroll/Employee Maintenance/Employees*  

Click on the “New” button. The cursor will be on the ‘Employee No’ on the General Tab. Press ‘OK’, NAV will allocate the New Employee number. Proceed to complete the following details.

### Edit: Employee Card
|Field Name|Description|
|-----------------------------------------|-------------------------------------------------------------------------------|
|**GENERAL FASTTAB**||
|**Job Title**|Enter the Person’s Job Title| 
|**First Name**|Enter the Employee’s First Name| 
|**Last Name**|Enter the Employee’s Last Name|
|**Address**|Enter in the Employee’s Address Details.| 
|**Post Code / City**|Enter in the Employee’s Post Code e.g. 2000.|
|**Sate / Country Code**|Enter in ‘AUS’|
|**Phone Number**|Enter in the employee’s home phone number if known.|
|**Gender**|Select ‘Male’ or ‘Female’|
|**Marital Status**|If the Marital Status is known, select the appropriate code from the drop down arrow.|
|**COMMUNICATION FASTTAB**||
|**Extension**|Enter the employee’s work extension number if applicable.|
|**Mobile Phone No**|Enter the employee’s mobile phone number if applicable|
|**Phone No.**|The employee’s phone number will default if entered on the General Tab|
|**E-mail**|Enter the employee’s email address. This will be required if intending on emailing the employee’s pay advice| 
|**ADMINISTRATION FASTTAB**|| 
|**Employment date**|Enter the employee’s employment or start date. This field is a mandatory field, if nothing is entered will cause issues when calculating pays.|
|**Status**|This will default to ‘Active’| 
|**PERSONAL FASTTAB**||
|**Birth Date**|Enter the employee’s birth date|
|**Click “OK” once you have completed all fields required.**||




1.1   
Entering New Employees – Payroll Module

After
employees are entered into the Human Resources module they are then entered into
the Payroll module. All employee maintenance such as applications, updates to
pay details, bank details and tax information is maintained on the Payroll
Employee Card.

To access the
Employee Maintenance task Click the “Payroll Employee
Card” button or go to the following menu: 

Departments/Payroll/Employee
Maintenance/Payroll Employees

Click on the “New” button.  

 

On the Payroll Employee Card go to the Employee No and from the
Employee List select the employee you wish to continue entering on Payroll and
proceed to complete the following details:

Once the New Employee has been selected ‘Press Enter’ and the information that was entered
into the Human Resources Employee Card will default to the relevant fields in
the Payroll Employee Card.



1.1.1    
Edit: Payroll
Employee Card


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  GENERAL FASTTAB
  
 
 
  
  Payroll No
  
  
  Select the appropriate Payroll No. from the “ArrowDown”.  You will receive a message requesting
  whether you want to change the Employee to the Payroll No. you have selected.
  Click ‘Yes’
  
 
 
  
  Emp Type Code
  
  
  Select the Employee Type Code from “ArrowDown”.
  
 
 
  
  Payment Method
  
  
  Confirm the Payment Method has been changed to
  ‘EFT’. This will default to the Defaults on the Payroll Setup Card.
  
 
 
  
  Email Pay Advice
  
  
  If Pay advices will be sent via email, check
  this field. The employee’s email address must be entered in the Human
  Resources field, otherwise you will not be able to email the pay advice.
  
 
 
  
  Email Payment Summaries
  
  
  If Payment Summaries will be sent via email,
  check this field. The employee’s email address must be entered in the Human
  Resources field, otherwise you will not be able to email the pay advice.
  
 
 
  
  Timesheet Reminder
  
  
  The Timesheet Reminder field will default to
  ‘Yes’. Uncheck this field. 
  
 
 
  
   
   POSTING FASTTAB - The
   Posting Tab determines where and what information will be posted to the GL
   Accounts.
   
  
 
 
  
  Branch Code
  
  
  Select the relevant Branch Code from the “ArrowDown”.
  
 
 
  
  Global Dimension 1 &2
  
  
  Select the relevant Dimension Codes from the “ArrowDown”. This will
  usually be the same as the Branch Code. 
  
 
 
  
   
   RATE FASTTAB - There is nothing that needs to
   be completed on this tab, as the pay rates are later entered in the Pay
   Rates area.
   
  
  
   
   TAX FASTTAB 
   
  
 
 
  
  Tax Scale No
  
  
  The Tax Scale No. will default from the Payroll
  setup card and can be overridden.
  
 
 
  
  HELP Debt
  
  
  Select this field if advised on the declaration
  form.
  
 
 
  
  Student Loan ( SFSS )
  
  
  Select his field if advised on the declaration
  form.
  
 
 
  
  Fixed Tax Rate Applicable
  
  
  This Field needs to be selected and ticked.
  
 
 
  
  Fixed Tax Rate Valid Until Date
  
  
  The Valid Until Date will be supplied from the
  ATO and needs to be entered in this field.
  
 
 
  
  Fixed Tax Rate
  
  
  The ATO will supply a letter detailing the
  fixed Tax rate amount.
  
 
 
  
  G.S.T. Exempt
  
  
  This relates to the setup of an Incorporated Company
  and if this is required, it needs to be ticked.
  
 
 
  
  Fringe Benefits Amount
  
  
  This field needs to be entered for reporting on
  the PAYG Payment Summary.
  
 
 
  
  Inc. Company Tax Inv.Not Req
  
  
  This relates to the setup of an Incorporated Company
  and if this is required, it needs to be ticked.
  
 
 
  
   
   DECLARATION FASTTAB - If you have an
   Employment Declaration form for your employee, check the fields as per this
   form if you intend on remitting your employment declarations electronically
   to the ATO.
   
  
 
 
  
  Resident
  
  
  Select this field if advised on the Declaration
  Form.
  
 
 
  
  Tax Free Threshold Claimed
  
  
  Select this field if advised on the Declaration
  Form.
  
 
 
  
  HELP Debt
  
  
  Select this field if advised on the Declaration
  Form.
  
 
 
  
  Student Loan
  
  
  Select this field if advised on the Declaration
  Form.
  
 
 
  
  Claim Pension Rebate
  
  
  Select this field if advised on the Declaration
  Form.
  
 
 
  
  Use TFN for Superannuation
  
  
  Select this field if advised on the Declaration
  Form.
  
 
 
  
  Rebate Amount Claimed
  
  
  Select this field if advised on the Declaration
  Form.
  
 
 
  
  A.B.N.
  
  
  This relates to the setup of an Incorporated
  Company and needs to be entered – the format of this field is 11 characters.
  
 
 
  
  Incorporated Company Name
  
  
  This relates to the setup of an Incorporated
  Company and will need to be entered.
  
 
 
  
  Tax.File No
  
  
  Enter the employee’s Tax File No. the format
  for this field is a maximum of 9 characters.
  
 
 
  
  Birth Date
  
  
  This field will populate from the HR Employee
  card.
  
 
 
  
  Date Declaration Signed
  
  
  Enter in the Date Declaration Signed from the
  Employment Declaration form.
  
 
 
  
  Payee Signature
  
  
  If the employee has signed the Employment
  Declaration form, check this field.
  
 
 
  
  Declaration Lodged
  
  
  This field will be populated with a date once
  the Declaration File Generation has been processed. 
  
 
 
  
   
   PAY DETAILS FASTTAB - There is nothing that needs to
   be completed on this tab, as the pay details are populated from the history
   ledgers.
   
  
  
   
   WORK COVER FASTTAB - This
   tab is only required if the employee has been setup as an Incorporated
   Company.
   
  
 
 
  
  Workers Comp Policy No.
  
  
  The “Workers Comp Policy No” is used to record
  a Contractors policy number.
  
 
 
  
  Workers Comp Insurer
  
  
  The “Workers Comp Insurer” is used to record
  the name of the Contractors Workers Comp Insurer.
  
 
 
  
  Policy Expiration Policy
  
  
  The “Policy Expiration Date” is used to record
  the expiry date of the policy.
  
 


1.1.2    
Payroll Employee Card  – Pay Dissections

 

Employee Bank accounts are entered
in the Pay Dissections area.

Access this task by clicking the “Pay Dissections”
task icon. 



 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  Transaction Type Code
  
  
  Transaction Type Code 9999 will default in this
  field.
  
 
 
  
  Pay Dissection Type
  
  
  There are 2 types of dissections:
  ·        
  Main – Used to
  identify the main bank account
  ·        
  Part – Used to
  identify additional bank accounts 
  
 
 
  
  Bank Account No.
  
  
  Enter the employee’s bank account number. This
  field has a limit of 9 characters which should be entered as follows:
  123456789
  
 
 
  
  Bank Name
  
  
  This will default to the employee’s name and
  can be overridden accordingly 
  
 
 
  
  EFT Bank No.
  
  
  Enter in the employee’s BSB no. This field has
  a limit of 7 characters which should be entered as follows: 032-170
  
 
 
  
  Standard Amount / Standard %
  
  
  If the employee has nominated an additional
  account, enter in the Amount or the Percentage as nominated by the employee.
  
 
 
  
  Click “OK” once you
  have completed all fields required.
  
 


 

1.1.3    
Payroll Employee Card  – Pay Rates

 

Enter in Pay Rates in as an hourly rate. To access the Employee
Pay Rates task, click the “Pay
Rates” task
icon. 

 



 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  Employee start Date
  
  
  This field should default to the Employee’s
  Start Date
  
 
 
  
  Classification Code
  
  
  Click on the Arrow Up Button and select from
  the list – system created. 
  
 
 
  
  Employee Rate
  
  
  Enter in the Employee’s rate as an hourly
  amount.
  
 
 
  
  Click “OK” once you
  have completed all fields required.
  
 


 

After
you have updated the rate and you click on the Rate Tab, the rate should be
updated accordingly. ( This will only be updated if the Pay Period is after the
Employee’s Start Date ).

1.1.4    
Payroll Employee Card  – Gross / Allowances

It is assumed that Internal Employees are ‘Auto Paid’. To
automatically generate hours, Ordinary / Normal Time should be set up as a
permanent occurrence. The same applies if the employee is to receive an
allowance on a permanent basis.

To access the Pay and Allowances
task, Click the “Gross & Allowances” task
icon. 

 

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  Transaction Type Code
  
  
  Select the Transaction Type Code from the “ArrowDown” e.g. Normal
  Time or a Permanent Allowance.
  
 
 
  
  Start Date
  
  
  Enter in a Start Date of when the Allowance
  transaction should commence. If this is for Ordinary of Normal Hours there is
  no need to enter in a Start Date.
  
 
 
  
  Description
  
  
  The Description will default from the
  Transaction. You can override the description should you require a user
  defined description to print on the Pay Advice. This will save using
  duplicate codes.
  
 
 
  
  Units
  
  
  Enter in the number of units required to be
  generated. For Ordinary / Normal Time type transactions you can enter in the
  number of hours per the pay period. 
  
 
 
  
  Fixed Value
  
  
  Enter in the Fixed Value for allowance type
  transaction if required.
  
 
 
  
  Hourly Rate
  
  
  This will default from the Pay Rate table for
  Ordinary / Normal Time type transactions
  
 
 
  
  Pay Value
  
  
  This will be the sum of the Units field *
  Hourly Rate field
  
 
 
  
  Not Used
  
  
  The Not Used field is used to suppress the
  permanent transaction for a single pay only. When the pay period is closed on
  a payroll, this flag is then removed and ready to be generated for the next
  period.
  
 
 
  
  Click “OK” once you
  have completed all fields required.
  
 


 

1.1.5    
Payroll Employee Card  – Deductions

 

The Deductions Area is used to
setup permanent deductions.

To access the Deductions task, Click the “Deductions” task icon. 

 



 

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  Transaction Type Code
  
  
  Select the Transaction Type Code from the “ArrowDown”.
  
 
 
  
  Priority
  
  
  If there are a number of deductions, you can
  select the order in which they are deducted, by entering 1,2,3, etc. for each
  transaction type.
  
 
 
  
  Start Date
  
  
  Enter in a Start Date of when the Allowance
  transaction should commence. If this is for Ordinary or Normal Hours there is
  no need to enter in a Start Date. 
  
 
 
  
  Description
  
  
  The Description will default from the
  Transaction. You can override the description should you require a user
  defined description to print on the Pay Advice. This will save using
  duplicated codes.
  
 
 
  
  Standard Amount / Standard %
  
  
  Enter in a Standard Amount or Standard % of the
  deduction.
  
 
 
  
  Details
  
  
  Enter in a Reference number for the deduction
  
 
 
  
  Total Deduction
  
  
  If the Deduction is to cease as soon as it
  reaches a certain amount, enter in this amount here.
  
 
 
  
  LTD Amount
  
  
  This field is a sum of all the deductions to
  date.
  
 
 
  
  Not Used
  
  
  The Not Used field is used to suppress the
  permanent transaction for a single pay only. When the pay period is closed on
  a payroll, this flag is then removed and ready to be generated for the next
  period.
  
 
 
  
  Click “OK” once you
  have completed all fields required.
  
 


1.1.6    
Payroll Employee Card  – Superannuation 

To access the Superannuation task, Click the “Superannuation”
task icon. 

 



 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  Superannuation Company Code
  
  
  Select the Superannuation Company code from the
  “ArrowDown”.
  
 
 
  
  Membership No.
  
  
  Enter in the Membership No. if known
  
 
 
  
  Date Joined Fund
  
  
  The ‘Date Joined Fund’ date will default to the
  Employee’s start date. If this date differs from the Employee start date,
  enter in the stat date for the Superannuation Fund. 
  
 
 
  
  Employer Standard %
  
  
  The employer standard percentage will default
  to the value setup on the Superannuation Company card.
  
 
 
  
  Click “OK” once you
  have completed all fields required.
  
 


 

1.1.6.1    
Superannuation
- Employee Choice ( Changing Superannuation Funds )

Changing Superannuation funds - enter an end date
on the old fund and change the 9.5% to zero amount.

Then on the next line Add the new fund with the
current month in the start date, then add the employer standard 9.5%.

If you are updating the employee’s Superannuation
fund and your organisation is calculating Employer liabilities using On Costs,
you must ensure that you update the Superannuation Code on the Superannuation
On Cost transaction type.  (Reference 4.2.8 - Payroll Employee Card  – On Cost Transactions.

1.1.7    
Payroll Employee Card  – Leave Accruals

Dependent upon what is setup on the
Payroll (Pay Cycles) card, will depend upon whether the leave accruals will
default to the Payroll Employee card when the employee is assigned to the
Payroll.

To access the Leave Accrual task, Click the “Accruals” task icon. 
A list of the
Leave Accruals for the employee will appear for viewing purposes.

 



If you wish to create or add a new Leave Accrual,
click on the “New” icon.  

 



 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  Leave Type
  
  
  Select the Leave Type code from the “ArrowDown”.
  
 
 
  
  Leave Code
  
  
  Select the appropriate Leave Code from the “ArrowDown”.
  
 
 
  
  Start Date
   
  
  
  The ‘Starting Date’ will default to the
  employees start date. This date is the Employee leave Accrual Start Date.
  
 
 
  
  Click “OK” once you
  have completed all fields required.
  
 


 

1.1.8    
Payroll Employee Card  – On Cost Transactions

If your organisation has chosen to calculate
On Cost transactions, you will need to add in the relevant On Cost Transactions
so that they are generated during the calculation of pays.  

You access Employer On Costs from the Payroll
Employee Card by clicking on the “Accumulation
Calculations/” on the “Navigate”
ribbon.  

 

 



 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  Transaction Type Code
  
  
  Select the Transaction Type code from the “ArrowDown”.
  
 
 
  
  Start Date 
  
  
  The “Start Date” field is used to
  specify the date at which the On Cost transaction is to commence.
  
 
 
  
  End Date
  
  
  The “End Date” field is used to
  specify the date at which the On Cost transaction is to end.
  
 
 
  
  Pay Rate
  
  
  The “Pay Rate” field is used to
  retain the calculation rate of the On Cost transaction.  This amount entered into this field should
  be expressed in decimal format.  E.g.
  If the value is 9%, it should be entered as 0.09.
  
 
 
  
  Superannuation Code
  
  
  The “Superannuation Code” field is
  used to nominate the Contractor’s Superannuation code.  This is only applicable if this On Cost
  transaction relates to the SGC accrual.
  
 
 
  
  Not Used
  
  
  If this field is ticked the Pay
  Transaction Type is not applied to the “current” pay period only.  The
  flag will be reset for the next pay period.
  
 
 
  
  Click
  “OK”
  after you have completed your selection.
  
 


 

 

2      Payroll
Processing

2.1   
Payroll Processing   – Pay Journals

To access the Pay Journals task, go to the following menu:

Departments/Pay Journal/Pay
Processing/Pay Journal



 

2.2    Payroll
Processing   – Enter any leave
adjustments

In the “Pay Journal” section enter in any leave taken for
auto paid employee. 



To enter leave against a specific employee, at a minimum the
following fields should be populated:


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  No.
  
  
  Select the Employee’s No. from the “ArrowDown”.
  
 
 
  
  Transaction Type Code
  
  
  Enter or select the Transaction Type code for
  the Leave Type from the “ArrowDown”.
  
 
 
  
  From Date
  
  
  Enter in the Start Date of the absence in this
  field.   (**You will need to update
  your display settings if this field is not displaying)
  
 
 
  
  To Date
  
  
  Enter in the End Date of the absence in this
  field.  (**You will need to update your
  display settings if this field is not displaying)
  
 
 
  
  Units
  
  
  Enter in the No. of Hours in this field.
  
 
 
  
  Subtract From Permanent Hours
  
  
  This field will automatically default from the
  setup of the Pay Transaction Type card.
  If the field is ticked, the value of this leave
  transaction will be deducted from the Employee’s standard auto-pay.
  If the field is not ticked, the value of this
  leave transaction will be paid in addition to the Employee’s standard
  auto-pay.
  
 
 
  
  After entering your leave/temporary
  adjustments, the auto-pays can be calculated.
  
 


 

2.3    Payroll
Processing   – Calculate Pays

In the Pay Journal - Select “Calculate Pays” to calculate your pays and “Enter the Pay Date“ and select “OK”. 



 

During this process any permanent hours and deductions,
leave accruals, tax and superannuation is generated.

 

Please note : Pays can be calculated by
individual or by all employees.

2.4    Payroll
Processing   – Entry Validation Reports

Once pays have been calculated, the
Entry Validation report has to be printed. You can  preview the report online first for any errors
or warnings which need to be fixed before proceeding to the next step. To run click
on the  “Entry
Validation report” task. 

 

Select Print Preview to check
for errors and warnings on the screen, when all clear, Print. 

 



 

If errors are found on the Entry Validation Report, the
individual’s pay can be fixed by uncalculating the pay. Please see the next
step for “uncalculating Pays”.



2.5    Payroll
Processing   – Uncalculating Pays

Pays can be uncalculated for individual employees or for all
employees within the Pay Journal. To “uncalculate” the pays, open the Actions
Tab and click on “Cancel
Calculated Pays”

 

2.6   
Payroll Processing  - Create Bank Transfer File

When the Entry Validation report has been checked and found to be
correct, run the create bank transfer file process. To run the process click on
the “Create Bank Transfer File” icon. The file can be saved to a network.




 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  Employee No.
  
  
  You can create a bank transfer file for one
  employee by nominating the Employee’s number from the AssistButton.
  Otherwise leave it blank to create a bank file
  for all employees.
  
 
 
  
  Bank Account
  
  
  The Bank Account attached to the Payroll will
  default from the Payroll Card.
  Otherwise you can click on the AssistButton if
  you wish to nominate another Bank Account.
  
 
 
  
  Process Date
  
  
  This will be the “Processing Date” when the
  file will be processed by the Bank.
  The date should be today’s date or greater.
  
 
 
  
  Description
  
  
  Enter in a Description for the file.
  
 
 
  
  File Name
  
  
  You can specify where you would like to save
  the file by clicking on the AssistButton. 
  
  You must ensure that you save the file with an
  .aba extension.
  
 
 
  
  Print Transfer Listing
  
  
  This field will automatically be selected and
  will provide you with an option to Print or Preview the Bank Transfer Listing
  Report.
  (*If you do not print this report, it can be
  re-printed at a later stage).
  
 
 
  
  Click “OK” once you
  have completed all fields required.
  
 


Pay advices are automatically flagged as paid. If for any reason
you need to re-run the transfer again, run the “Cancel Bank Transfer” process
and redo. 

 

 

2.7   
Payroll Processing  - Post and Print Pay Advices

When each batch of pays has been processed, they should be posted.
This clears them from the Pay Journal area and writes the data to the employee
pay history ledgers.



 

After you nominate the “Post” option, a “Print Pay Advice”
message will appear as part of the posting process.



To print or reprint payslips, go to the following menu:

Departments/Payroll/Payroll
Processing/ Print Pay Advices



 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  Payroll No.
  
  
  From the AssistButton, nominate the Payroll you
  wish to re-print pay advices for.
  
 
 
  
  Period No.
  
  
  From the AssistButton, nominate the Period No.
  you wish to re-print the pay advices for.
  
 
 
  
  Click “OK” once you
  have completed all fields required.
  
 


 



To email payslips, go to the following menu:

Departments/Payroll/Payroll
Processing/ E-Mail Pay Advices 



 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  OPTIONS FASTTAB
  
 
 
  
  Pay Advice Message
  
  
  Complete this field if you wish to have a pay
  advice message printed on the emailed pay advices.
  
 
 
  
  POSTED PAY ADVICE FASTTAB
  
 
 
  
  Employee No.
  
  
  From the AssistButton, select the Employee No.
  otherwise leave this blank to generate email pay advices for all.
  
 
 
  
  Payroll No.
  
  
  From the AssistButton, select the Payroll No.
  otherwise leave this blank to generate email pay advices for all.
  
 
 
  
  Tax Year
  
  
  From the AssistButton, select the Tax Year otherwise
  leave this blank to generate email pay advices for all.
  
 
 
  
  Period No.
  
  
  From the AssistButton, select the Period No.
  otherwise leave this blank to generate email pay advices for all.
  
 
 
  
  No.
  
  
  From the AssistButton, select the No. (which
  relates to the Pay Advice No.) otherwise leave this blank to generate email
  pay advices for all.
  
 
 
  
  Click “OK” once you
  have completed all fields required.
  
 


 

 

2.8   
Payroll Processing  - Close Pay Periods

You can close the pay period independently if you choose not to
close the pay period at the time of posting the payroll.  To Close Pay periods, go to the following
menu:

Departments/Payroll/Periodic
Activities/Periodic Maintenance/ Close Pay Periods



 

Select
the Payroll No and press “OK’. Then select the Pay Period by the ticking the
‘Closed and Date Locked’ columns to close the pay period.


