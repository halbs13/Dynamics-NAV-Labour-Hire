

# Introduction

Superannuation processing within the Dynamics NAV Payroll and Labour Hire modules encompasses the following functions: 

 - Setup. 
   - Superannuation SGC,NON SGC, Salary Sacrifice and Post Tax Deductions Pay Transaction Types 
   - Superannuation Funds
   - SGC rules as per the ATO Legislation defined on the Payroll Setup Card
   - Allocating SGC and NON SGC transactions to the Rate Set or Payroll Employee Card
   - Allocating a Superannuation Fund to an employee
- Superannuation Calculation and Reporting

This document will specifically discuss how to use the Superannuation Processing function within Dynamics NAV.
For further information relating to the setup of each of these areas, please refer to the Dialog – Training – LH –
Payroll Setup Configuration document. 

The activities discussed are: 
   - Bulk Adjustments
   - Calculate Monthly Superannuation
   - Calculate and Post Superannuation
   - Superannuation Report
   - Superannuation Adjustments 
      
## Superannuation Overview

There are two (2) options available in relation to setting up Superannuation within Dynamics
NAV Payroll and Labour Hire module and this will depend upon whether the rate that you pay your 
candidates is inclusive or exclusive of the SGC component. This section will summarise where 
superannuation is treated as an On cost (SGC is exclusive of the pay rate).

Within the Dynamics NAV Payroll and Labour Hire module, Superannuation is accrued as an On
Cost transaction to facilitate itinerant staff hired within the Recruitment industry.  

The Superannuation On Cost transaction will either be stored on the Rate Set of a Job whereby
the cost of the superannuation will be allocated back to a Job No. or otherwise stored on the Payroll Employee. 

Salary Sacrifice and Post Tax deductions are entered via the Employee Deductions area of the Payroll Employee card and will be generated on a pay-by-pay basis when the candidate’s pay is processed.

When the pays are calculated, the superannuation on cost transaction is generated within the pay journal based upon the transactions
contained in the journal and if the candidate has any superannuation deductions, these are also generated at this during
this process.    

After the journal has been validated, posting the pay journal will update the General Ledger and 
Employee Ledger Entry tables and if a Job No. is specified against the on cost transaction, the Job Ledger Entry 
is also updated. The General Ledger is updated with an expense and provisional transaction when the pays are posted 
and this is automatically re-adjusted when the superannuation is posted at the end of the month.

The Calculate Monthly Superannuation report is designed to be processed at the end of each calendar
month whereby a recalculation will occur to see if the candidate hasmet the SGC rules setup on the 
Payroll Setup card.  The transactions are sourced from the Employee Ledger Entry table where the pays 
were previously posted to and if the candidate meets the requirements, a superannuation ledger entry will be
generated with the employee’s nominated fund, otherwise a threshold transaction is generated and will be 
posted to the Employee Ledger Entry and General Ledgers as a “Threshold Adjustment”.  

When you have completed generating your superannuation ledger entries, the next step is to perform the
“Calculate & Post Superannuation” function which will post any threshold adjustments to the General 
Ledger and if you’ve opted for Vendor integration, an Invoice transaction will post to the Vendor Ledger Entry.

      
## Superannuation Processing

### Bulk Adjustments

This option is used to create bulk Superannuation changes to the Payroll Employee – superannuation cards when the
SGC % changes.

To access the Bulk Adjustments task, go to the following menu:

Departments/Payroll/EOM Processing/Superannuation Processing/Bulk Adjustment
   
### Edit: Bulk Update Superannuation 

|**Field Name**|**Description**|
|-------------------------------------------|------------------------------------------------------------------------------------|
||**OPTIONS FASTTAB**| 
|**New Employer SGC %**|Enter the new percentage for the selected Superannuation records.|
|**New Employer SGC amount**|Enter the new amount for the selected Superannuation records.|
|**New Employer Factor**|Enter the new amount for the selected Superannuation records.|
|**New Employee Post Tax Standard %**|Enter the new standard percentage for the selected Superannuation records.||**New Employee Post Tax Amount**|Enter the new standard amount for the selected Superannuation records.|
|**Update Employees**|Tick this field to update the records. Leave this field un-ticked not to update the employee records.|
||**SUPERANNUATION FUND PRODUCT FASTTAB - Only the standard fields are covered. A full list of fields available as filters can be used by selecting the add filter.**|
|**Transaction Type Code**|Select the Transaction Type Code for the Superannuation records you wish to adjust. If left blank all Superannuation Pay Transaction Type codes are selected.|
|**Employer SGC %**|To filter the records you wish to change enter the Employee Standard Percentage to select for adjustment.|
||**SUPERANNUATION EMPLOYEE FASTTAB - Only the standard fields are covered. A full list of fields available as filters can be used by selecting the add filter.**| 
|**Employee No**|Enter or Select the Employee’s you wish to adjust the superannuation records. If left blank all employees are selected.|
||**Click “OK” once you have completed your selection.**|

**Calculate Monthly Superannuation**

This option isused to create monthly superannuation transactions to post to the General Ledger. 
This option is used where the “Calc. Superannuation Monthly” flag isticked on the “Payroll” card 
in the “Options Tab”. It is also used when you arecalculating employee on-cost superannuation.

**Note:** You only need to run this report when the On Costing Method is used for calculating superannuation.

This process updates the Employee’s superannuation Ledger Entry with on-cost superannuation transaction 
details ready for Posting to the General Ledger using the “Calculate & Post Superannuation” process. You must 
print the report for the process to move the on-cost transactions to the Superannuation LedgerEntries table.

To access the Calculate Monthly Superannuation, go to the following menu:

Departments/Payroll/EOM Processing/Superannuation Processing/Calculate Monthly Superannuation

### Edit: Calc. Monthly Superannuation 
   
|**Field Name**|**Description**|
|------------------------------------------------|----------------------------------------------------------------------------------|
|**Calculation Date**|Enter the date you want the Monthly Superannuation transactions calculated. The last date of the month must be entered to ensure all pays for the month are picked up for the calculations.|
|**Month to Calculate**|This field displays the month automatically after you enter the Calculation Date.|
|**Month Start Date**|This field displays the 1st date of the above month after the date has been entered.|
|**Month End Date**|This field displays the last date of the above month after the date has been entered.|
|**Report Only**|Tick this flag to produce a report without updating the Employee Superannuation Ledger records. Leave this field blank to update the Employee Superannuation Ledger records.|
||**If you wish to preview the report to screen, you should ensure that you click “Report Only” and then click “Preview”. If you wish to create Superannuation Ledger Entries, you should ensure that “Report Only” is NOT TICKED and print the report. You can send the report to a printer or save as a pdf, click “Print” and select the relevant option.**|

## Calculate & Post Superannuation

This option is used to calculate and post superannuation transactions to the General Ledger. This 
option can be run after each pay period to pick up Superannuation Transactions that were calculated 
during the pay process.

This process must be run after the “Calculate Monthly Superannuation” process has run when you
use the On Costing method to calculate Superannuation.

To access the Calculate Monthly Superannuation, go to the following menu:

Departments/Payroll/EOM Processing/Superannuation Processing/Calculate & Post Superannuation  

### Edit: Calculate & Post Super.Exp

|**Field Name**|**Description**|
|------------------------------------------|---------------------------------------------------------------------------------------| 
|**Payroll No.**|This field displays the payroll number for the selected payroll.|
|**Posting date**|This field is used to enter the date you want the Superannuation transactions posted.|
|**Month Start Date**|This field displays the 1st date of the above month after the date has been entered.| 
|**Month End Date**|This field displays the last date of the above month after the date has been entered.|
|**Document No.**|Enter a meaningful document number to identify the transactions in the General Ledger.|
|**Report Only**|Tick this flag to produce a report without updating the General Ledger. Leave this field blank to update the General Ledger. When the “Report Only” is ticked no posting will occur even if Post to G/L is ticked.|
|**Post to General Ledger**|Tick this flag to post to the General ledger. If left un-ticked the report is produced without updating the General Ledger.|
|**Create Vendor Invoices**|Tick this option to create Vendor Invoices for the Superannuation Pay Transaction Type with Vendor Number setups.|
|**Consolidate Vendor Invoices**|Tick this option to create one invoice per Vendor. If left un-ticked a separate vendor invoice is created for each employee Superannuation record.| 
|**Skip SGC Employees**|If you run this process more than once per month (i.e. after each payroll for non-monthly pay frequencies then) you must tick this option. The flag must be left blank for the last Calculate & Post Superannuation process for the month. SGC Employee transactions are Employer contributions.|
||**If you wish to preview the report to screen, you should ensure that you click “Report Only” and then click “Preview”.**|
||**If you wish to create Superannuation Ledger Entries, you should ensure that “Report Only” is NOT TICKED and print the report. You can send the report to a printer or save as a pdf, click “Print” and select the relevant option.**|

## Superannuation Report

After you have finalised the EOM Superannuation use this report to remit your payments to the funds.

This report lists the detailed superannuation transaction types (Employee, Membership No and Amount) for the selected
criteria.

The report is sorted by Superannuation Company and then transaction type with a transaction total for both Employee and
Employer contributions.

You can select to run this report using a total per Employee with a Fund total instead.

To access the Superannuation Report, go to the following menu:

Departments/Payroll/EOM Processing/Superannuation Processing/Superannuation Report  

### Edit: Superannuation Report 
   
|**Field Name**|**Description**|
|---------------------------------------|---------------------------------------------------------------------------------------|   
||**OPTIONS FASTTAB**|
|**Payroll No.**|Type in or select from the ArrowDown button, the Payroll which you wish to report on.| 
||**SUPERANNUATION FUND PRODUCT FASTTAB - Only the standard fields are covered. A full list of fields available as filters can be used by selecting the add filter.**|
|**Code**|Select the Transaction Type Code for the Superannuation records you wish to adjust. If left blank all Superannuation Pay Transaction Type codes are selected.| 
||**SUPERANNUATION LEDGER ENTRY FASTTAB - Only the standard fields are covered. A full list of fields available as filters can be used by selecting the add filter.**|
|**Posting Date**|Enter the date of which you wish to generate transactions for.|
||You can enter in date filters as follows:| 
||01/09/2012..30/09/2012 and this will retrieve information with a posting date within this range.|
||If you wish to preview the report to screen, click “Preview”. If you wish to print the report to a printer or save as a pdf, click “Print” and select the relevant option.|
  
The fields on the Superannuation Report are:

|**Report Field**|**Field No.**|**Obtained from**|
|---------------------------------|---------|----------------------------------------------------------------------------------| 
|**Transaction Type Code**|(1)|This identifies the Transaction Type code for the contribution. This information will be available on each of the Superannuation Products.|
|**Tran. Type Description**|(2)|This field identifies the description of the Transaction Type code for the contribution.|
|**Employee No.**|(3)|This is the Employee No.|
  
 
 
  
  Employee Name
  
  
  (4)
  
  
  This is the Employee Name.
  
 
 
  
  Membership No.
  
  
  (5)
  
  
  This is the Employee’s Superannuation Membership No.
  
 
 
  
  Amount
  
  
  (6)
  
  
  This is the contribution amount of the employee. 
  
 
 
  
  Fund Total
  
  
  (7)
  
  
  This will be the Fund Total Amount.
  
 




 

2.5      
SuperStream Payment Requirements



 

Under the Superannuation
Guarantee you must pay superannuation contributions to the correct
superannuation fund, by the cut off dates, for all your eligible
employees.  

 

You may also be required to offer
a choice of superannuation fund to your eligible employees.

 

The superannuation guarantee is
administered on a self-assessing basis and there are laws requiring you to meet
your superannuation obligations.  It is your responsibility as an employer
to ensure arrangements you have in place for your employees satisfy the
government’s superannuation guarantee requirements.  

 

More information can be found on
at the Australian Taxation Office website: http://www.ATO.gov.au.

 

Dialog Pty Ltd has developed the
“Superannuation Payments” Module.  The module will allow you to produce a
mail merge (.CSV) file or print the Superannuation payments on the employees
next Pay Advice after you pay the fund.  

 

When an employee is not paid in
the next pay run the module will allow you to produce a mail merge (.CSV) file
to create a letter for the employee.

 

An export has been created to allow for New Member information to be
remitted to the fund electronically which can be produced for an employee or a
Payroll, Superannuation Fund Product. 
The export can be revised in preview mode which will highlight any
missing information such as Membership and Address information.

 

There are 5 Superannuation Payment File options:

 


 Generic
 ClickSuper
 SuperChoice
 SunSuper
 SuperStream Alternative
 Quick Super


 

It is recommended
that you review the requirements of the file layouts as contained in section 2.5.6- 
Superannuation File Layouts to ensure that you have the necessary mandatory
information completed.

 

To open the Superannuation Payments module, 

 

Department/Payroll/Periodic Activities/Superannuation/Superannuation
Payments



The Superannuation Payment Module
contains the following Menu Options: 

 

Super. Payment Export &
Notification – this report flags the Employee Superannuation Ledger Entry
records for reporting to the employee by either Letter or Pay Advice. 
When the report is run you select the parameters for processing, to control how
the update is processed.  As a default the report runs as “Preview no
Post” to be used to reconcile the reportable amounts.  After you have
reconciled the amounts; re-run the report selecting the reporting method you
wish to report the amounts to your employees.

 

Super. Payment Export Reversal
– This option is used to reverse the reporting flags when an error was made
before the amounts have been physically reported to your employees.  If
the Payment Advice has been reported to your employees you cannot use this
option.

 

New Member Registration Export
– This report is used to provide the Employee information to the
Superannuation Fund.  The report can be
previewed so that any errors or information missing on the Employee file is
rectified prior to producing a file.  

 

2.5.1    
Superannuation Payment
Reporting

 

Employers have an obligation to
report superannuation contributions to their employees: 

 

The amount of each superannuation
contribution made for the employee during the period to which the pay slip
relates and the name of any fund to which the contribution was made.

 

The Super. Payment Export &
Notification Report flags the Employee Superannuation Ledger Entry records to
report to the employee by either Letter or Pay Advice.  When the report is
run you must enter parameters for processing.  

 




2.5.2     New
Member Registration Export

 

The New Member Registration
Export produces a file which may be used to send to the Superannuation
Fund.  

 

It is recommended that you
preview the report first as it will highlight potential issues with the file
such as invalid tax file numbers and missing information.

 

To access the New Member
Registration Export,

 

Departments/Payroll/EOM
Processing/Superannuation Processing

 



 




 
  
   
   Field
   
   
   Comments
   
  
 
 
  
  OPTIONS FASTTAB
   
  
 
 
  
  Run Type
  
  
  Select the process from the list.  
  
  
  Preview no export
  – This option previews the report and allows you to verify the data before
  reporting.  This option can be run multiple times.  
  
  
  Export new member
  file – Used to create a “.CSV” file.  
  
 
 
  
  Member File Export Location
  
  
  Click on the “ArrowDown”
  to specify where to save the file.
  
 
 
  
  PAYROLL EMPLOYEE FASTTAB – Payroll Employee information can be
  filtered by entering information in this tab. 
  Otherwise it can be left blank. 
  
 
 
  
  EMPLOYEE SUPERANNUATION FASTTAB – Employee Superannuation information can be
  filtered by entering information in this tab. Otherwise it can be left blank.
  
 
 
  
  SUPERANNUATION FUND PRODUCT FASTTAB– Superannuation Fund Product information
  can be filtered by entering information in this tab.  Otherwise it can be left blank.
  
 
 
  
  When you have finished entering your
  information, click on “Preview” or “Print” to
  produce the file and report.
  
 




 

2.5.2.1    
New Member Registration Export Report Sample

 



 

The
report fields contained on the New Member Registration Report are:

 


 Employee No.
 Employee First Name
 Employee Last Name
 Membership No.
 Employee Product Code
 Product Name


 

Missing
information will appear in the report and you should update the information
accordingly.  Please refer to the Error! Reference source not found. in Section 2.5.6.1 as to the location of
where the data is stored with Dynamics NAV Payroll.

 

2.5.2.2    
Possible Error Messages

 

Each of the Payment File Options will have their own
mandatory requirements.  If the files are
rejected, please refer to the Error! Reference source not found. in Section 2.5.6
of this document.

 

2.5.3    
Super Payment Export & Notification

 

Employers have an obligation to
report superannuation contributions to their employees:

 


 The amount of each superannuation contribution made
     for the employee during the period to which the pay slip relates, the name
     of any fund to which the contribution was made and the date the
     contribution was paid.


 

The Super Payment Export &
Notification Report flags the Employee Superannuation Ledger Entry records to
report to the employee by either Letter or Pay Advice.  When the report is
run you must enter parameters for processing.  

 

To access the Super Payment
Export & Notification, 

 

Departments/Payroll/EOM
Processing/Superannuation Processing/Super.Payment Export & Notification
Report



 




 
  
   
   Field
   
   
   Comments
   
  
 
 
  
  Payroll No.
  
  
  The Payroll No. can be selected from the “ArrowDown”. 
   
  If left blank all Payrolls are processed. 
  
 
 
  
  Start Posting Date
  
  
  Enter the Start Posting Date of the period you want to
  include.  This will filter transactions
  in the Superannuation Ledger Entry table based on the date that you enter in
  this field.
  
 
 
  
  End Posting Date
  
  
  Enter the End Posting Date of the period you want to
  include.  This will filter transactions
  in the Superannuation Ledger Entry table based on the date that you enter in
  this field.
  
 
 
  
  Contribution Period Start Date
  
  
  This date will default to the date that you have entered
  in the “Start Posting Date” field.
  
 
 
  
  Contribution End Date
  
  
  This date will default to the end date that you have
  entered in the “End Posting Date” field.
  
 
 
  
  Run Type
  
  
  Select the process from the list. 
   
  Preview no post – This option
  previews the report without flagging the amounts as reported to the
  Employee.  Use this option to verify the amounts remitted to the fund
  before reporting.  This option can be run multiple times.  
   
  Post and create
  letter file – Used to create a “.CSV” file to produce letters to the
  employee and flag the employee records as advised of Superannuation
  contributions.  
  
  Post and Create Pay Advice record–
  This option is similar to the previous option but instead of creating a
  “.CSV” file the Employee Superannuation Ledger Entries are flagged to print
  on the next Employee Pay Advice.
  
  Employees with no pay next period
  – This option must be used after your Next Pay is posted to general
  Ledger.  The option selects all employees who did not receive a Pay
  Advice in the “next pay” after “Post and create Pay Advice record” are
  run.  A “.CSV” file is then created that you can use to produce a letter
  for these employees.
   
  Note: If your
  Company has multiple Payrolls and you select all Payrolls you must ensure
  that you have completed processing all payrolls before you run this
  process.  If you don’t the employees
  contributions not yet paid and posted to the GL will go to the “.CSV” file
  and the message will not print on their Pay Advice.  Or run this process
  separately for each payroll.
  
 
 
  
  Payment Export Format
  
  
  There are currently 5 options for you to select from:
   
  Generic:  The Generic payment file layout is
  described in Section 2.5.6.2
  Generic Payment Format.
    
  ClickSuper:  The ClickSuper payment file layout is
  described in Section 2.5.6.3
  ClickSuper Payment Format.
   
  SuperChoice:
  The SuperChoice payment file layout is described in Section 2.5.6.4
  SuperChoice Payment Format.
   
  SunSuper: The
  SunSuper payment file layout is described in Section 2.5.6.4
  SunSuper Payment Format.
   
  SuperStream
  Alternative: The SuperStream Alternative payment file layout is described
  in Section 2.5.6.6
  SuperStream Alternative Payment Format.
   
  QuickSuper: The
  QuickSuper payment file layout is described in Section 2.5.6.7
  QuickSuper Payment Format.
   
   
  
 
 
  
  Date Paid to Fund
  
  
  Enter the date you paid the SGC amounts to the fund.
  
 
 
  
  Notification Letter File Export Location
  
  
  This field is only used for “Post and create letter file”
  and “Employees with no pay next period”.  
  Enter the path and file name location where you want to create the “.CSV”
  file.  This field remains greyed out for the other “Run Type” options 
  
 
 
  
  Payment File Export Location
  
  
  This field is used to identify the Payment File Export
  Location.  
  Enter the path and file name location where you want to create the “.CSV”
  file.  
  
 
 
  
  Sunsuper USI
  
  
  Enter in the Sun Super USI no. so this may be added to the
  Sun Super file on generation.
  
 
 
  
  SUPERANNUATION FUND PRODUCT FASTTAB – Superannuation Fund Product information
  can be filtered by entering information in this tab.  Otherwise it can be left blank. 
  
 
 
  
  SUPERANNUATION LEDGER ENTRY FASTTAB – Superannuation Ledger Entry information
  can be filtered by entering information in this tab.  Otherwise it can be left blank. 
  
 
 
  
  When you have finished entering your
  information, click on “Preview” or “Print” to
  produce the file and report.
  
 




 

 

2.5.3.1    
Superannuation Payment Export and Notification
Report



 

 

The fields on the Superannuation Payment Export &
Notification report are:

 




 
  
   
   Report Field
   
   
   Field No.
   
   
   Obtained from
   
  
 
 
  
  Run ID
  
  
  (1)
  
  
  This identifies the Run ID of the Superannuation Export
  & Notification.  
   
  If you need to reverse the report, you will use this record
  no.
  
 
 
  
  Run Type
  
  
  (2)
  
  
  This identifies the run type of the report.  The run type values are:
  
   “Export
       Payment and create notification letter”
   “Export
       Payment and create pay advice notification”
  
  
 
 
  
  Contribution Date
  
  
  (3)
  
  
  This is the Contribution End date of the records.
  
 
 
  
  Date Paid To Fund
  
  
  (4)
  
  
  This is the Date Paid To Fund.
  
 
 
  
  Letter File Export Location
  
  
  (5)
  
  
  This is the location of where the Letter export will be
  saved.
  
 
 
  
  Payment File Export Location
  
  
  (6)
  
  
  This is the location of where the Payment File export will
  be saved.
  
 
 
  
  Code
  
  
  (7)
  
  
  This is the Superannuation Product Code
  
 
 
  
  Product Name
  
  
  (8)
  
  
  This is the Product Name
  
 
 
  
  Employee No.
  
  
  (9)
  
  
  This is the Employee No.
  
 
 
  
  Employee Name
  
  
  (10)
  
  
  This is the Employee name
  
 
 
  
  Membership No.
  
  
  (11)
  
  
  This is the Employee’s Superannuation Membership No.
  
 
 
  
  Employee Amount
  
  
  (12)
  
  
  An amount will appear in this column if the employee has
  made contributions.
  
 
 
  
  Employer Amount
  
  
  (13)
  
  
  An amount will appear in this column if the employer has
  made contributions for the employee.
  
 




 

 

 

2.5.3.2    
Pay Advice Notification 

 

The Pay Advice Notification
Report flags the Employee Superannuation Ledger entry records as reported to
your employees.  The following steps outline the process:

 


 Select
     the Pay Advice Notification Report.
 Select
     the Employees or Groups of Employees on the “Superannuation Ledger Entry”
     tab.
 Select
     the “Payroll No.” you wish to process.
 Enter
     either the “Pay Period End” or “Contribution” date.  If a Payroll is
     not selected the “Pay Period End” date field is greyed out.
 Select
     the “Run Type”.  It is recommended that the “Run Type” option
     “Preview no post” is run initially to reconcile the fund amounts before
     running the report and committing the amounts reported to employees.
      When selecting this option a report is produced.  
 Enter
     the “Date Paid to Fund”.  This is the date that the payments were
     made to the Superannuation Fund.
 Enter
     the “File Export Location”.  Enter the path you wish the “.CSV” file
     to be placed.  This field is greyed out except for Run Type
      “Post and create letter file” or “Employees with no pay next period”
 Select
     either the “Print” or “Preview” button to run the process.
 If
     you have selected the Run Type “Post and create Pay Advice record” then
     you must run the “Employees with no pay next period” after you have
     processed your payrolls for the next pay period.  This option will
     create a .CSV file so that you can use Word and Mail Merge to produce a
     letter to your employees who were not paid.


 

2.5.3.3    
Example of the Pay Advice message:

 

“The Superannuation payment of $9999.99 for the period of dd/mm/yyyy to
dd/mm/yyyy was paid into xxxxxxxxxxxxxx for credit to your account 99999999 on
dd/mm/yyyy.”

 

This message will be printed on
the Pay Advice for each Superannuation fund the employee has used within the
Superannuation reporting period.

 

Note: Each company has
subtle setup differences to meet their business requirements.  It is recommended that the values on the
report are verified prior to distribution. 

 

2.5.3.4    
Possible Error Messages

 

The employee’s Superannuation
record for the Superannuation Product Code has been changed or deleted after
payments have been made to the fund during the Superannuation Reporting period.

 

In the Payroll Employee
card/Navigate ribbon/Superannuation add the deleted Superannuation Product
Code.  Change the amounts and percentage value to zero to prevent the
deduction from processing in future pay journals.

 

2.5.4    
Super. Payment
Export Reversal 

 

You may use this process to
reverse the Superannuation Notification Report by entering the “SGC Extract
Report Run Id” for the current processing month.  The “SGC Extract Report
Run Id” is located on the Superannuation Payment Export and
Notification Report
towards the top left hand corner of the report.  You can only reverse the
Payment process in the following conditions:

 


 When
     you have used the Letter (.CSV) file.  You can reverse the process up
     to one month after the file has been produced.  If you have already
     issued the letters a letter explaining the changes you have made must be
     issued to the employees.
 When
     you have used the Pay Advice option.  You can only reverse the
     process up until you print the Pay Advices in the next pay run.


 

To access the Super. Payment Export Reversal report, 

 

Departments/Payroll/EOM
Processing/Superannuation Processing/Super. Payment Export Reversal 



 




 
  
   
   Field
   
   
   Comments
   
  
 
 
  
  SGC Extract Report Run ID 
  
  
  Enter the SGC Extract Report Run Id for the Run Id you
  wish to reverse.
  
  The Run Id is found at the top left corner of the Superannuation Payment
  & Notification Report.
  
 
 
  
  When you have finished entering your
  information, click on “OK”.
  
   
 
 
 
  
  
  
 
 




 

2.5.4.1    
Running Super. Export & Notification
Reversal

 

The Reversing process is used to
reset the reporting flags where after you have processed the transactions for
reporting and wish to make changes.  You can only reverse the transactions
if you have not reported the payments to your employees by producing Pay
Advices for the next payroll run or created the letter file (.CSV).  The
following steps outline the Reversal process.

 

Select the Super.Payment Export Reversal Report.Enter the “SGC Extract Report Run Id”.Select OK.A message will display the number of records
reversed when the process is completed.Make any required corrections and repeat your
“Super.Payment Export & Notification” process again. 














2.5.5    
Super. Payment History

 

The Super. Payment History report will provide you with
information by fund on each of the payments made to an employee.

 

You enter in the Payroll No., Contribution Date, Date Paid
to Fund and whether you want to display the information in detail.

 

To access the Super. Payment History report, 

 

Departments/Payroll/EOM
Processing/Superannuation Processing/Super. Payment History



 

 




 
  
   
   Field
   
   
   Comments
   
  
 
 
  
  Payroll No.
  
  
  Select the Payroll No. from the “ArrowDown”.  
   
  If left blank all Payrolls are processed. 
  
 
 
  
  Contribution Date
  
  
  Enter in the Contribution Date or the Ending Posting Date
  that you entered when producing the Super. Payment Export & Notification
  report.  
  
 
 
  
  Date Paid to Fund
  
  
  Enter the date you paid the SGC amounts to the fund.
  
 
 
  
  Show Detail
  
  
  If you wish to preview the information in Detail, select
  this field.
  
 
 
  
  SUPERANNUATION LEDGER ENTRY FASTTAB – Superannuation Ledger Entry information
  can be filtered by entering information in this tab.  Otherwise it can be left blank. 
  
 
 
  
  When you have finished entering your
  information, select “Preview” or “Print” to
  produce the file and report.
  
 




 

 

 

2.5.5.1    
Employee SGC Reporting History (Super.Payment
History Report) – Detail

 



 

 

The fields on the Employee SGC Reporting History (Super.
Payment History) report are:

 




 
  
   
   Report Field
   
   
   Field No.
   
   
   Obtained from
   
  
 
 
  
  Fund Name
  
  
  (1)
  
  
  This field identifies the Superannuation Fund Code for the
  employee.
  
 
 
  
  Superannuation Code
  
  
  (2)
  
  
  This field identifies the Superannuation Product Code for
  the employee.
  
 
 
  
  Membership No.
  
  
  (3)
  
  
  This field is the Employee’s Superannuation Membership No.
  
 
 
  
  Date Paid To Super Fund
  
  
  (4)
  
  
  This field is the Date the Superannuation was paid to the
  Superannuation Fund.
  
 
 
  
  Amount paid on Date
  
  
  (5)
  
  
  This is the amount that as paid to the Superannuation
  Fund.
  
 
 
  
  Fund Total
  
  
  (6)
  
  
  This is the Fund Total for the Employee.
  
 
 
  
  Employee Total
  
  
  (7)
  
  
  This is the Employee Total for the Employee.
  
 
 
  
  Employee No.
  
  
  (8)
  
  
  This is the Employee No.
  
 
 
  
  Employee Name
  
  
  (9)
  
  
  This is the Employee Name.
  
 




 

2.5.5.2    
Employee SGC Reporting History (Super.Payment
History Report) – Summary

 



 

The fields on the Employee SGC Reporting History (Super.
Payment History) report are:

 




 
  
   
   Report Field
   
   
   Field No.
   
   
   Obtained from
   
  
 
 
  
  Fund Name
  
  
  (1)
  
  
  This field identifies the Superannuation Fund Code for the
  employee.
  
 
 
  
  Superannuation Code
  
  
  (2)
  
  
  This field identifies the Superannuation Product Code for
  the employee.
  
 
 
  
  Membership No.
  
  
  (3)
  
  
  This field is the Employee’s Superannuation Membership No.
  
 
 
  
  Date Paid To Super Fund
  
  
  (4)
  
  
  This field is the Date the Superannuation was paid to the
  Superannuation Fund.
  
 
 
  
  Amount paid on Date
  
  
  (5)
  
  
  This is the amount that as paid to the Superannuation
  Fund.
  
 
 
  
  Fund Total
  
  
  (6)
  
  
  This is the Fund Total for the Employee.
  
 
 
  
  Employee Total
  
  
  (7)
  
  
  This is the Employee Total for the Employee.
  
 
 
  
  Employee No.
  
  
  (8)
  
  
  This is the Employee No.
  
 
 
  
  Employee Name
  
  
  (9)
  
  
  This is the Employee Name.
  
 




 




2.5.6    
Superannuation File Layouts

 

2.5.6.1    
New Member Registration Export

The fields contained in the New
Member Registration Export file are:

 




 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  Company Name
  
  
  The “Company Name” is sourced from the Company Name field
  on the Payroll card the employee is assigned to.
  
 
 
  
  Company ABN
  
  
  The “Company ABN” is sourced from the Company ABN field on
  the Payroll card the employee is assigned to
  
 
 
  
  Fund Assigned Employer No.
  
  
  The “Fund Assigned Employer No.” is sourced from the
  Superannuation Fund the employee is assigned to.
  
 
 
  
  Fund ABN
  
  
  The “Fund ABN” is sourced from the Superannuation Fund the
  employee is assigned to.
  
 
 
  
  Superannuation Fund No. (SFN)
  
  
  The “Superannuation Fund No. (SFN)” is sourced from the
  Superannuation Fund the employee is assigned to.
  
 
 
  
  Product ID No. (SPIN)
  
  
  The “Product ID No. (SPIN)” is sourced from the
  Superannuation Product assigned on the Employee Superannuation card. 
  
 
 
  
  Unique Identifier (USI)
  
  
  The “Unique Identifier (USI)” is sourced from the
  Superannuation Product the employee is assigned to.
  
 
 
  
  Title
  
  
  The “Title” field is sourced from the Employee card.
  
 
 
  
  Surname
  
  
  The “Surname” field is sourced from the Employee card.
  
 
 
  
  First Name
  
  
  The “First Name” field is sourced from the Employee card.
  
 
 
  
  Middle Name
  
  
  The “Middle Name” field is sourced from the Employee card.
  
 
 
  
  Gender
  
  
  The “Gender” field is sourced from the Employee card.
  
 
 
  
  Birth Date
  
  
  The “Birth Date” field is sourced from the Employee card.
  
 
 
  
  Job Title
  
  
  The “Job Title” field is sourced from the Payroll Employee
  card.
  
 
 
  
  Address Line 1
  
  
  The “Address Line 1” field is sourced from the Employee
  card.
  
 
 
  
  Address Line 2
  
  
  The “Address Line 2” field is sourced from the Employee
  card.
  
 
 
  
  Suburb
  
  
  The “Suburb” is sourced from the Employee card.
  
 
 
  
  Post Code
  
  
  The “Post Code” field is sourced from the Employee card.
  
 
 
  
  State 
  
  
  The “State” field is sourced from the Employee card.
  
 
 
  
  Country
  
  
  The “Country” field is sourced from the Employee card.
  
 
 
  
  E-Mail 
  
  
  The “E-Mail” field is sourced from the Employee card.
  
 
 
  
  Phone No.
  
  
  The “Phone No.” field is sourced from the Employee card.
  
 
 
  
  Membership No.
  
  
  The “Membership No.” field is sourced from the Employee
  Superannuation card.
  
 
 
  
  Tax File No.
  
  
  The “Tax File No.” field is sourced from the Payroll
  Employee card.
  
 
 
  
  Payroll ID
  
  
  The “Payroll ID” field is the Employee No. and is sourced
  from the Employee card.
  
 
 
  
  Employment Date
  
  
  The “Employment Date” field is sourced from the Payroll
  Employee card.
  
 
 
  
  Termination Date
  
  
  The “Termination Date” field is sourced from the Payroll
  Employee card.
  
 
 
  
  Termination Reason
  
  
  The “Termination Reason” field is sourced from the
  Employee card.
  
 
 
  
  Annual Salary
  
  
  The Annual Salary information is sourced from the Employee
  Pay Rates card.
   
  
 
 
  
  Hours worked per Week
  
  
  The “Hours worked per Week” information is sourced from
  the Payroll Employee card.
  
 
 
  
  Date Joined Fund
  
  
  The “Date Joined Fund” field is populated from the
  Employee Superannuation card.
  
 




 

 

2.5.6.2    
Generic Payment Format

The fields contained in the
Generic Payment file are:

 




 
  
   
   Field Name
   
   
   Mandatory
   
   
   Description
   
  
 
 
  
  Reference
  
  
  Mandatory
  
  
  This is the Reference ID for the file and is system
  generated.
  
 
 
  
  Contribution Start Date
  
  
  Mandatory
  
  
  The “Contribution Start Date” field is populated from the
  data that you enter into the Super Payment Export & Notification Form. 
  
 
 
  
  Contribution End Date
  
  
  Mandatory
  
  
  The “Contribution End Date” field is populated from the
  data that you enter into the Super Payment Export & Notification Form. 
  
 
 
  
  Organisation Name
  
  
  Mandatory
  
  
  The “Organisation Name” is sourced from the Payroll
  Company Name field.
  
 
 
  
  Organisation ABN
  
  
  Mandatory
  
  
  The “Organisation ABN” is sourced from the Payroll Company
  ABN field.
  
 
 
  
  Superannuation Fund Employer ID
  
  
  Mandatory
  
  
  The “Superannuation Fund Employer ID” is sourced from the
  Fund Employer ID on the Superannuation Fund.
  
 
 
  
  Superannuation Fund ABN
  
  
  Mandatory
  
  
  The “Superannuation Fund ABN” is sourced from the Fund ABN
  on the Superannuation Fund.
  
 
 
  
  Superannuation Fund Banking Institution Name
  
  
  Mandatory
  
  
  The “Superannuation Fund Banking Institution Name” is
  sourced from the Banking Institution Name on the Superannuation Fund.
  
 
 
  
  Superannuation Fund Bank Account Name
  
  
  Mandatory
  
  
  The “Superannuation Fund Bank Account Name” is sourced
  from the Bank Account Name on the Superannuation Fund.
  
 
 
  
  Superannuation Fund Bank Account Number
  
  
  Mandatory
  
  
  The “Superannuation Fund Bank Account Number” is sourced
  from the Bank Account Number on the Superannuation Fund.
  
 
 
  
  Superannuation Fund Bank Branch No.
  
  
  Mandatory
  
  
  The “Superannuation Fund Bank Branch No.” is sourced from
  the Bank Branch No. on the Superannuation Fund.
  
 
 
  
  Remittance E-Mail
  
  
  Mandatory
  
  
  The “Remittance E-Mail” is sourced from the Remittance
  E-Mail Address on the Superannuation Fund. 
  (This will be replaced by IP address from 1 July 2014)
  
 
 
  
  Electronic Service Address
  
  
  Mandatory
  
  
  The “Electronic Service Address” is sourced from the
  Electronic Service Address on the Superannuation Fund.
  
 
 
  
  Product ID No. (SPIN)
  
  
  Mandatory
  
  
  The “Product ID No.” is sourced from the Product ID No. on
  the Superannuation Product.
  
 
 
  
  Unique Identifier (USI)
  
  
  Mandatory
  
  
  The “Unique Identifier (USI)” is sourced from the Unique
  Identifier on the Superannuation Product.
  
 
 
  
  Employee Membership No.
  
  
  Mandatory
  
  
  The “Employee Membership No.” is sourced from the
  Membership No. on the Employee Superannuation table.
  
 
 
  
  Employee No.
  
  
  Optional
  
  
  The “Employee No.” is sourced from the Employee No. on the
  Payroll Employee table.
  
 
 
  
  Tax File Number
  
  
  Mandatory
  
  
  The “Tax File Number” is sourced from the Tax File Number
  on the Payroll Employee table.
  
 
 
  
  Tax File Number Not Provided Indicator
  
  
  Mandatory
  
  
  The “Tax File Number” field is updated is an employee does
  not provide a Tax File Number.
  
 
 
  
  Title
  
  
  Optional
  
  
  The “Title” is sourced from the Title field on the
  Employee table.
  
 
 
  
  Employee Last Name
  
  
  Mandatory
  
  
  The “Employee Last Name” is sourced from the Last Name on
  the Employee table.
  
 
 
  
  Employee First Name
  
  
  Mandatory
  
  
  The “Employee First Name” is sourced from the First Name
  on the Employee table.
  
 
 
  
  Employee Middle Name
  
  
  Optional
  
  
  The “Employee Middle Name” is sourced from the Middle Name
  on the Employee table.
  
 
 
  
  Employee Gender
  
  
  Optional
  
  
  The “Employee Gender” is sourced from the Gender on the
  Employee table.
  
 
 
  
  Employee Birth Date
  
  
  Optional
  
  
  The “Employee Birth Date” is sourced from the Birth Date
  on the Employee table.
  
 
 
  
  Employment Start Date
  
  
  Mandatory
  
  
  The “Employment Start Date” is sourced from the Start Date
  on the Employee table.
  
 
 
  
  Employee Termination Date
  
  
  Optional
  
  
  The “Employee Termination Date” is sourced from the
  Termination Date on the Payroll Employee table.
  
 
 
  
  Employee Address
  
  
  Optional
  
  
  The “Employee Address” is sourced from the Address on the
  Employee table.
  
 
 
  
  Employee Address 2 
  
  
  Optional
  
  
  The “Employee Address 2” is sourced from the Address 2 on
  the Employee table.
  
 
 
  
  Employee Suburb
  
  
  Optional
  
  
  The “Employee Suburb” is sourced from the City on the
  Employee table.
  
 
 
  
  Employee Post Code
  
  
  Optional
  
  
  The “Employee Post Code” is sourced from the Post Code on
  the Employee table.
  
 
 
  
  Employee State
  
  
  Optional
  
  
  The “Employee State” is sourced from the State on the
  Employee table.
  
 
 
  
  Employee Country Name
  
  
  Optional
  
  
  The “Employee Country” is sourced from the Country on the
  Employee table.
  
 
 
  
  Employee E-Mail
  
  
  Optional
  
  
  The “Employee E-Mail” is sourced from the E-Mail on the
  Employee table.
  
 
 
  
  Employee Phone No
  
  
  Optional
  
  
  The “Employee Phone No.” is sourced from the Phone No. on
  the Employee table.
  
 
 
  
  Employee Mobile No.
  
  
  Optional
  
  
  The “Employee Mobile No.” is sourced from the Mobile No.
  on the Employee table.
  
 
 
  
  Employer SGC Amount
  
  
  Mandatory
  
  
  The “Employer SGC Amount” is sourced from the Employer SGC
  contributions on the Superannuation Ledger Entry table.
  
 
 
  
  Employee Post Tax Contribution – Personal Contributions
  
  
  Optional
  
  
  The “Employee Post Tax Contribution” is sourced from the
  Employee Post Tax on the Superannuation Ledger Entry table.
  
 
 
  
  Employee Salary Sacrifice Amount
  
  
  Optional
  
  
  The “Employee Salary Sacrifice Amount” is sourced from the
  Employee Salary Sacrifice contributions on the Superannuation Ledger Entry
  table.
  
 
 
  
  Employee Non SGC Amount – Employer Contributions Voluntary
  
  
  Optional
  
  
  The “Employer Non SGC Amount” is sourced from the Employer
  Non SGC contributions on the Superannuation Ledger Entry table.
  
 




 

 

2.5.6.3    
ClickSuper Payment Format

The fields contained in the
ClickSuper Payment file are:

 




 
  
   
   Field Name
   
   
   Mandatory
   
   
   Description
   
  
 
 
  
  Reference
  
  
  Mandatory
  
  
  This is the Reference ID for the file and is system
  generated.
  
 
 
  
  Total Payment
  
  
  Optional
  
  
  This is the Total Payment for the Employee sourced from
  the Superannuation Ledger Entry table.
  
 
 
  
  Sender ID
  
  
  Optional
  
  
  The “Sender ID” field is not exported.
  
 
 
  
  Sender Email
  
  
  Mandatory
  
  
  The “Sender Email” is sourced from the Company Email
  address on the Payroll table.
  
 
 
  
  Contact Given Name
  
  
  Optional
  
  
  The “Contact Given Name” is not exported.
  
 
 
  
  Contact Family Name
  
  
  Optional
  
  
  The “Contact Family Name” is not exported.
  
 
 
  
  Contact Number
  
  
  Optional
  
  
  The “Contact Number” is not exported.
  
 
 
  
  Target Fund ABN
  
  
  Mandatory
  
  
  The “Target Fund ABN” is sourced from the ABN of the
  Superannuation Fund for the employee.
  
 
 
  
  Target Product ID
  
  
  Optional
  
  
  The “Target Product ID” is sourced from the Product ID of
  the Superannuation Product for the employee.
  
 
 
  
  Target Fund Name
  
  
  Optional
  
  
  The “Target Fund Name” is sourced from the Fund Name of
  the Superannuation Fund for the employee. 
  
 
 
  
  Target Product Name
  
  
  Optional
  
  
  The “Target Product Name” is sourced from the Product Name
  on the Superannuation Product card for the employee.
  
 
 
  
  Target Super Fund Admin Name
  
  
  Optional
  
  
  The “Target Super Fund Admin Name” is sourced from the
  Contact on the Superannuation Fund card for the employee.
  
 
 
  
  Target BSB
  
  
  Optional
  
  
  The “Target BSB” is sourced from the Bank Branch No. on
  the Superannuation Fund for the employee.
  
 
 
  
  Target Account Number
  
  
  Optional
  
  
  The “Target Account Number” is sourced from the Bank
  Account Number on the Superannuation Fund for the employee.
  
 
 
  
  Target Account Name
  
  
  Optional
  
  
  The “Target Account Name” is sourced from the Bank Account
  Name on the Superannuation Fund for the employee.
  
 
 
  
  Payee Short Name
  
  
  Optional
  
  
  The “Payee Short Name” is not exported
  
 
 
  
  Payment Remitter Identifier
  
  
  Mandatory
  
  
  The “Payment Remitter Identifier” is defaulted to
  “CLICKSUPER”
  
 
 
  
  Payment Reference Number
  
  
  Mandatory
  
  
  The “Payment Reference Number” is defaulted to
  “CLICKSUPER”
  
 
 
  
  Payment Amount
  
  
  Mandatory
  
  
  The “Payment Amount” is total of all contributions for the
  employee.
  
 
 
  
  Payment Creation Date
  
  
  Mandatory
  
  
  The “Payment Creation Date” is the date that is entered in
  the Date Paid to Fund field on the Super Payment Export & Notification
  form.
  
 
 
  
  Source BSB
  
  
  Optional
  
  
  The “Source BSB” is not exported
  
 
 
  
  Source Account Number
  
  
  Optional
  
  
  The “Source Account Number” is not exported
  
 
 
  
  Email
  
  
  Optional
  
  
  The “Email” is sourced from the Remittance Email on the
  Superannuation Fund.
  
 
 
  
  Alternate Addressee
  
  
  Optional
  
  
  The “Alternate Addressee” is not exported
  
 
 
  
  Address Line 1
  
  
  Optional
  
  
  The “Address Line 1” is not exported
  
 
 
  
  Address Line 2
  
  
  Optional
  
  
  The “Address Line 2” is not exported
  
 
 
  
  Suburb
  
  
  Optional
  
  
  The “Suburb” is not exported
  
 
 
  
  State
  
  
  Optional
  
  
  The “State” is not exported
  
 
 
  
  Post Code
  
  
  Optional
  
  
  The “Post Code” is not exported
  
 
 
  
  Country
  
  
  Optional
  
  
  The “Country” is not exported
  
 
 
  
  Contributor Type
  
  
  Mandatory
  
  
  The “Contributor Type” will default to “EMPLOYER”
  
 
 
  
  Contributor ID
  
  
  Optional
  
  
  The “Contributor ID” is sourced from the Fund Employer No.
  on the Superannuation Fund for the employee.
  
 
 
  
  Contributor Business Name
  
  
  Mandatory
  
  
  The “Contributor Business Name” is sourced from the
  Company Name on the Payroll for the employee.
  
 
 
  
  Contributor ABN
  
  
  Mandatory
  
  
  The “Contributor ABN” is sourced from the Company ABN on
  the Payroll for the employee.
  
 
 
  
  Contact Given Name
  
  
  Mandatory
  
  
  The “Contact Given Name” is sourced from the Contact
  Person on the Payroll for the employee.
  
 
 
  
  Contact Family Name
  
  
  Mandatory
  
  
  The “Contact Family Name” is sourced from the Contact
  Person on the Payroll for the employee.
  
 
 
  
  Contact Number
  
  
  Mandatory
  
  
  The “Contact Number” is sourced from the Contact Phone No.
  on the Payroll for the employee.
  
 
 
  
  Email
  
  
  Optional
  
  
  The “Email” is sourced from the Company Email on the
  Payroll for the employee.
  
 
 
  
  Pay Centre ID
  
  
  Optional
  
  
  The “Pay Centre ID” is sourced from the Pay Centre ID on
  the Superannuation Fund for the employee.
  
 
 
  
  Pay Period Start Date
  
  
  Optional
  
  
  The “Pay Period Start Date” is not exported
  
 
 
  
  Pay Period End Date
  
  
  Optional
  
  
  The “Pay Period End Date” is not exported
  
 
 
  
  Payroll Reference No.
  
  
  Optional
  
  
  The “Payroll Reference No.” is sourced from the Employee
  No. on the Payroll Employee table.
  
 
 
  
  Payroll Member Name
  
  
  Optional
  
  
  The “Payroll Member Name” is sourced from the Full Name on
  the Payroll Employee table.
  
 
 
  
  Fund Member No.
  
  
  Optional
  
  
  The “Fund Member No.” is sourced from the Membership No.
  on the Employee Superannuation table.
  
 
 
  
  Status Code
  
  
  Mandatory
  
  
  The “Status Code” is defaulted to “UNKNOWN”.
  
 
 
  
  Given Name
  
  
  Mandatory
  
  
  The “Given Name” is sourced from the First Name and Middle
  on the Payroll Employee table.
  
 
 
  
  Family Name
  
  
  Mandatory
  
  
  The “Family Name” is sourced from the Last Name on the
  Payroll Employee table.
  
 
 
  
  Name Title
  
  
  Optional
  
  
  The “Name Title” is sourced from the Title on the Employee
  table.
  
 
 
  
  Sex
  
  
  Optional
  
  
  The “Sex” is sourced from the Gender on the Employee
  table.
  
 
 
  
  Birth Date
  
  
  Optional
  
  
  The “Birth Date” is sourced from the Birth Date on the
  Employee table.
  
 
 
  
  Email 
  
  
  Optional
  
  
  The “Email” is sourced from the Email on the Employee
  table.
  
 
 
  
  Home Contact Number
  
  
  Optional
  
  
  The “Home Contact Number” is sourced from the Phone No. on
  the Employee table.
  
 
 
  
  Work Contact Number
  
  
  Optional
  
  
  The “Work Contact Number” is sourced from the Work Contact
  Number on the Employee table.
  
 
 
  
  Mobile Contact Number
  
  
  Optional
  
  
  The “Mobile Contact Number” is sourced from the Mobile
  Phone No. on the Employee table.
  
 
 
  
  TFN 
  
  
  Optional
  
  
  The “TFN” is sourced from the Tax File Number on the
  Payroll Employee table.
  
 
 
  
  Alternate Addressee
  
  
  Optional
  
  
  The “Alternate Addressee” is not exported
  
 
 
  
  Address Line 1
  
  
  Optional
  
  
  The “Address Line 1” is not exported
  
 
 
  
  Address Line 2 
  
  
  Optional
  
  
  The “Address Line 2” is not exported
  
 
 
  
  Suburb
  
  
  Optional
  
  
  The “Suburb” is not exported
  
 
 
  
  State
  
  
  Optional
  
  
  The “State” is not exported
  
 
 
  
  Postcode
  
  
  Optional
  
  
  The “Postcode” is not exported
  
 
 
  
  Country
  
  
  Optional
  
  
  The “Country” is not exported
  
 
 
  
  Date Joined Co
  
  
  Optional
  
  
  The “Date Joined Co” is sourced from the Employment Date
  on the Employee table.
  
 
 
  
  Date Left Co
  
  
  Optional
  
  
  The “Date Left Co” is sourced from the Termination Date on
  the Employee table.
  
 
 
  
  Occupation
  
  
  Optional
  
  
  The “Occupation” is not exported
  
 
 
  
  Employment Type
  
  
  Optional
  
  
  The “Employment Type” is not exported
  
 
 
  
  Part Time Hours
  
  
  Optional
  
  
  The “Part Time Hours” is not exported
  
 
 
  
  Salary Amount
  
  
  Optional
  
  
  The “Salary Amount” is not exported
  
 
 
  
  Fund Exit Reason
  
  
  Optional
  
  
  The “Fund Exit Reason” is not exported
  
 
 
  
  Pay Centre ID
  
  
  Optional
  
  
  The “Pay Centre ID” is sourced from the Pay Centre ID on
  the Superannuation Fund for the Employee
  
 
 
  
  Cont. Period Start Date
  
  
  Optional
  
  
  The “Contribution Start Date” field is populated from the
  data that you enter into the Super Payment Export & Notification Form 
  
 
 
  
  Cont. Period End Date
  
  
  Optional
  
  
  The “Contribution End Date” field is populated from the
  data that you enter into the Super Payment Export & Notification Form 
  
 
 
  
  SGC Amount
  
  
  Mandatory
  
  
  The “SGC Amount” is sourced from the Employer SGC
  contributions on the Superannuation Ledger Entry table.
  
 
 
  
  Salary Sacrifice Amount
  
  
  Optional
  
  
  The “Salary Sacrifice Amount” is sourced from the Employee
  Salary Sacrifice contributions on the Superannuation Ledger Entry table.
  
 
 
  
  Non SGC Amount
  
  
  Optional
  
  
  The “Non SGC Amount” is sourced from the Employer Non SGC
  contributions on the Superannuation Ledger Entry table.
  
 
 
  
  Member Voluntary Amount
  
  
  Optional
  
  
  The “Member Voluntary Amount” is sourced from the Employee
  Post Tax on the Superannuation Ledger Entry table.
  
 
 
  
  Spouse Contributions
  
  
  Optional
  
  
  The “Spouse Contributions” is not exported
  
 
 
  
  Salary Sacrifice Voluntary
  
  
  Optional
  
  
  The “Salary Sacrifice” is not exported
  
 
 
  
  Member Regular
  
  
  Optional
  
  
  The “Member Regular” is not exported
  
 
 
  
  Productivity Contributions
  
  
  Optional
  
  
  The “Productivity Contributions” is not exported
  
 
 
  
  Redundancy Contributions
  
  
  Optional
  
  
  The “Redundancy Contributions” is not exported
  
 
 
  
  Member Single Premium
  
  
  Optional
  
  
  The “Member Single Premium” is not exported
  
 
 
  
  Employer Additional
  
  
  Optional
  
  
  The “Employer Additional” is not exported
  
 
 
  
  Additional Invalidity Premium
  
  
  Optional
  
  
  The “Additional Invalidity Premium” is not exported
  
 
 
  
  Other family and friend contributions amount
  
  
  Optional
  
  
  The “Other family and friend contributions amount” is not
  exported
  
 
 
  
  Employer Single Premium
  
  
  Optional
  
  
  The “Employer Single Premium” is not exported
  
 
 
  
  Member Deducted
  
  
  Optional
  
  
  The “Member Deducted” is not exported
  
 
 
  
  Drug and Alcoholism Contributions
  
  
  Optional
  
  
  The “Drug and Alcoholism Contributions” is not exported
  
 




 

 

2.5.6.4    
SuperChoice Payment Format

The fields contained in the
SuperChoice Payment file are:

 




 
  
   
   Field Name
   
   
   Mandatory
   
   
   Description
   
  
 
 
  
  Employee ID
  
  
  Optional
  
  
  The “Employee ID” is sourced from the Employee No. on the
  Employee Superannuation table.
  
 
 
  
  Super Fund Member No.
  
  
  Mandatory
  
  
  The “Super Fund Member No.” is sourced from the Membership
  No. on the Employee Superannuation table.
  
 
 
  
  Title
  
  
  Optional
  
  
  The “Title” is sourced from the Title on the Employee
  table.
  
 
 
  
  Employee First Name
  
  
  Mandatory
  
  
  The “Employee First Name” is sourced from the First Name
  and Middle on the Payroll Employee table.
  
 
 
  
  Employee Surname
  
  
  Mandatory
  
  
  The “Employee Surname” is sourced from the Last Name on
  the Payroll Employee table.
  
 
 
  
  Employee Date of Birth
  
  
  Mandatory
  
  
  The “Birth Date” is sourced from the Birth Date on the
  Employee table.
  
 
 
  
  Gender
  
  
  Mandatory
  
  
  The “Gender” is sourced from the Gender on the Employee
  table.
  
 
 
  
  Employee Address Line 1
  
  
  Mandatory
  
  
  The “Employee Address Line 1” is sourced from the Address
  Line 1 on the Employee table.
  
 
 
  
  Employee Address Line 2
  
  
  Optional
  
  
  The “Employee Address Line 2” is sourced from the Address
  Line 2 on the Employee table.
  
 
 
  
  Suburb
  
  
  Mandatory
  
  
  The “Suburb” is sourced from the City on the Employee
  table.
  
 
 
  
  State
  
  
  Mandatory
  
  
  The “State” is sourced from the State on the Employee
  table.
  
 
 
  
  Post Code
  
  
  Mandatory
  
  
  The “Postcode” is sourced from the Postcode on the
  Employee table.
  
 
 
  
  Mobile Phone No.
  
  
  Optional
  
  
  The “Mobile Phone No.” is sourced from the Mobile Phone
  No. on the Employee table.
  
 
 
  
  Employee Email Address 
  
  
  Optional
  
  
  The “Employee Email Address” is sourced from the Email on
  the Employee table.
  
 
 
  
  Tax File Number
  
  
  Mandatory
  
  
  The “Tax File Number” is sourced from the Tax File Number
  on the Payroll Employee table.
  
 
 
  
  Fund Name
  
  
  Mandatory
  
  
  The “Fund Name” is sourced from the Product Name of the
  Superannuation Product for the employee. 
  
 
 
  
  Unique Superannuation Identifier (USI)
  
  
  Mandatory from 1 July
  
  
  The “Unique Superannuation Identifier (USI)” is sourced
  from the Unique Superannuation Identifier (USI) of the Superannuation Product
  for the employee.
  
 
 
  
  Product ID No. (SPIN)
  
  
  Mandatory for APRA funds
  
  
  The “Product ID No.” is sourced from the Product ID No. of
  the Superannuation Product for the employee.
   
  If the fund has no SPIN the ABN must be provided.
  
 
 
  
  Fund Employer No.
  
  
  Mandatory
  
  
  The “Fund Employer No.” is sourced from the Fund Employer
  No. of the Superannuation Fund for the employee.
  
 
 
  
  Superannuation Fund ABN
  
  
  Mandatory (for SMSF Funds and some APRA)
  
  
  The “Superannuation Fund ABN” is sourced from the
  Superannuation Fund ABN of the Superannuation Fund for the employee. 
  
 
 
  
  Superannuation Fund Bank Name
  
  
  Optional
  
  
  The “Superannuation Fund Bank Name” is sourced from the
  Bank Name on the Superannuation Fund for the employee.
  
 
 
  
  Superannuation Bank Account Number
  
  
  Mandatory
  
  
  The “Superannuation Bank Account Number” is sourced from
  the Bank Account Number on the Superannuation Fund for the employee.
  
 
 
  
  Superannuation BSB
  
  
  Mandatory
  
  
  The “Superannuation BSB” is sourced from the Bank Branch
  No. on the Superannuation Fund for the employee.
  
 
 
  
  Target Electronic Service Address
  
  
  Mandatory
  
  
  The “Target Electronic Service Address is sourced from the
  Electronic Service Address on the Superannuation Fund for the employee.
  
 
 
  
  SGC Amount
  
  
  Mandatory
  
  
  The “SGC Amount” is sourced from the Employer SGC
  contributions on the Superannuation Ledger Entry table.
  
 
 
  
  Employer Additional Amount
  
  
  Optional
  
  
  The “Employer Additional Amount” is sourced from the
  Employer Non SGC contributions on the Superannuation Ledger Entry table.
  
 
 
  
  Salary Sacrifice Amount
  
  
  Optional
  
  
  The “Salary Sacrifice Amount” is sourced from the Employee
  Salary Sacrifice contributions on the Superannuation Ledger Entry table.
  
 
 
  
  Member Voluntary Amount
  
  
  Optional
  
  
  The “Member Voluntary Amount” is sourced from the Employee
  Post Tax on the Superannuation Ledger Entry table.
  
 




 

 

 

2.5.6.5    
SunSuper Payment Format

The fields contained in the
SunSuper Payment file are:

 




 
  
   
   Field Name
   
   
   Mandatory
   
   
   Description
   
  
 
 
  
  Super Product USI
  
  
  Mandatory
  
  
  The “Super Product USI No.” is sourced from the USI field
  on the Superannuation Product for the employee.
  
 
 
  
  Payroll ID
  
  
  Mandatory
  
  
  The “Payroll ID” is sourced from the Employee No. on the
  Payroll Employee card for the employee.
  
 
 
  
  Member ID
  
  
  Mandatory
  
  
  The “Member ID” is sourced from the Membership No. field
  on the Employee Superannuation card for the employee.
  
 
 
  
  Family Name
  
  
  Mandatory
  
  
  The “Family Name” is sourced from the Last Name field on
  the Employee card for the employee.
  
 
 
  
  Given Names
  
  
  Mandatory
  
  
  The “Given Names” is sourced from the First Name field on
  the Employee card for the employee.
  
 
 
  
  Other Given Names
  
  
  Optional
  
  
  The “Other Given Names” is sourced from the Middle Name
  field on the Employee card for the employee. 
  
 
 
  
  Title
  
  
  Mandatory
  
  
  The “Title” is sourced from the Title field on the
  Employee card for the employee.
  
 
 
  
  Name Suffix
  
  
  Optional
  
  
  The “Name Suffix” field is not exported.
  
 
 
  
  Date of Birth
  
  
  Mandatory
  
  
  The “Date of Birth” is sourced from the Birth Date field
  Employee card for the employee.
  
 
 
  
  Gender
  
  
  Optional
  
  
  The “Gender” is sourced from the Gender field on the
  Employee card for the employee.
  
 
 
  
  Superannuation Guarantee Amount
  
  
  Mandatory
  
  
  The “Superannuation Guarantee Amount” is sourced from the
  Employer SGC contributions on the Superannuation Ledger Entry table.
  
 
 
  
  Award or Productivity Amount
  
  
  Optional
  
  
  The “Award or Productivity Amount” field is not exported.
  
 
 
  
  Personal Contributions Amount
  
  
  Optional
  
  
  The “Personal Contributions Amount” is sourced from the
  Employee Post Tax on the Superannuation Ledger Entry table. 
  
 
 
  
  Salary Sacrificed Amount
  
  
  Optional
  
  
  The “Salary Sacrificed Amount” is sourced from the
  Employee Pre Tax on the Superannuation Ledger Entry table.
  
 
 
  
  Voluntary Amount
  
  
  Optional
  
  
  The “Voluntary Amount” is sourced from the Employer
  Non-SGC contributions on the Superannuation Ledger Entry table.
  
 
 
  
  Address Type
  
  
  Mandatory
  
  
  The “Address Type” is defaulted to “POS”.
  
 
 
  
  Address 1
  
  
  Mandatory
  
  
  The “Address 1” is sourced from the Address field on the
  Employee card for the employee.
  
 
 
  
  Address 2 
  
  
  Optional
  
  
  The “Address 2” is sourced from the Address 2 field on the
  Employee card for the employee.
  
 
 
  
  Address 3
  
  
  Optional
  
  
  The “Address 3” is not exported.
  
 
 
  
  Address 4
  
  
  Optional
  
  
  The “Address 4” is not exported.
  
 
 
  
  Locality (Suburb)
  
  
  Mandatory
  
  
  The “Suburb” is sourced from the City field on the
  Employee card for the employee.
  
 
 
  
  State
  
  
  Mandatory
  
  
  The “State” is sourced from the County field on the
  Employee card for the employee.
  
 
 
  
  Post Code
  
  
  Mandatory
  
  
  The “Post Code” is sourced from the Post Code field on the
  Employee card for the employee.
  
 
 
  
  Country
  
  
  Mandatory
  
  
  The “Country” is sourced from the Country field on the
  Employee card for the employee.
  
 
 
  
  TFN
  
  
  Mandatory
  
  
  The “TFN” is sourced from the Tax File No. field on the
  Payroll Employee card for the employee.
  
 
 
  
  Employment Start Date
  
  
  Mandatory
  
  
  The “Employment Start Date” is sourced from the Employment
  Date field on the Employee card for the employee.
  
 
 
  
  Annual Salary for Insurance
  
  
  Optional
  
  
  The “Annual Salary for Insurance” is sourced from the
  Annual Salary from the Employee Pay Rate card for the employee.
  
 
 
  
  Employment End Date
  
  
  Optional
  
  
  The “Employment End Date” is sourced from the Termination
  Date on the Employee card for the employee.
  
 
 
  
  Employment Status
  
  
  Mandatory
  
  
  The “Employment Status” is sourced from the Status field
  on the Employee card for the employee.
  
 
 
  
  Email
  
  
  Optional
  
  
  The “Email” is sourced from the E-mail field on the
  Employee card for the employee.
  
 
 
  
  Mobile
  
  
  Optional
  
  
  The “Mobile” is sourced from the Mobile Phone No. field on
  the Employee card for the employee.
  
 
 
  
  Landline
  
  
  Optional
  
  
  The “Landline” is sourced from the Phone No. field on the
  Employee card for the employee.
  
 




 

 

2.5.6.6    
SuperStream Alternative Payment Format

The fields contained in the SuperStream
Alternative file are:

 




 
  
   
   Field Name
   
   
   Mandatory
   
   
   Description
   
  
 
 
  
  Header section
   
  
 
 
  
  Version
  
  
  Mandatory
  
  
  The “Version” will default to 1.0
  
 
 
  
  Negatives Supported
  
  
  Mandatory
  
  
  The “Negatives Supported” field will default.  These are the guidelines as provided by the
  ATO.
   
  * Mandatory data field. If this field is not populated,
  the value 'false' should be assumed.
  * Boolean data field: value must be 'true' or 'false'
  only.
  * This field is an indicator. 
  - true: this indicates that negative amounts are able to
  be provided in fields and can be processed
  - false: this indicates that negative amounts in fields
  must not be used and should not be processed.
   
  * Principles governing use
  - The default position is that negative values are NOT
  supported.
  - A choice can be made to support negative values in
  fields on an opt-in basis, to suit special, known requirements. This choice
  is exercised on the Fund side.
  - Where a Fund opts to allow negatives, the Fund is
  responsible for specifying the rules governing where and how negative amounts
  can be added, and the implications for associated payments.
  - Where a Fund opts to allow negatives, the Fund is also
  responsible for working with their stakeholders - employers and other service
  providers (for example payroll software companies) - to implement that
  choice.
  
 
 
  
  File ID
  
  
  Optional
  
  
  The “File ID” is populated by what is entered into the
  file name.
  
 
 
  
  Header Section
   
  
 
 
  
  ID
  
  
  Mandatory
  
  
  The “ID” field is defaulted from within the export.
  
 
 
  
  Source Entity ID
  
  
   
  
  
  The “Source Entity ID” field is sourced from the Company
  ABN field on the Payroll card.
  
 
 
  
  Source Entity ID Type
  
  
   
  
  
  The “Source Entity ID Type” field is defaulted to
  http://www.abr.gov.au/abn
  
 
 
  
  Source Electronic Service Address
  
  
   
  
  
  This information is not exported.
  
 
 
  
  Electronic Error Messaging
  
  
   
  
  
  This information is not exported.
  
 
 
  
  Sender Section
   
  
 
 
  
  Sender ABN
  
  
  Mandatory
  
  
  The “Sender ABN” is sourced from the ABN field on the
  Payroll card for the employee.
  
 
 
  
  Organisational Name
  
  
  Mandatory
  
  
  The “Organisation Name” is sourced from the Company Name
  field on the Payroll card for the employee. 
  
 
 
  
  Family Name
  
  
  Mandatory
  
  
  The “Family Name” is sourced from the Last Name field on
  the Employee card for the employee.
  
 
 
  
  Given Name
  
  
  Mandatory
  
  
  The “Given Name” is sourced from the First Name field on
  the Employee card for the employee.
  
 
 
  
  Other Given Name
  
  
  Optional
  
  
  The “Other Given Name” is sourced from the Middle Name
  field on the Employee card for the employee.
  
 
 
  
  E-mail Address
  
  
  Optional
  
  
  The “E-mail Address” is sourced from the E-Mail field on
  the Employee card for the employee.
  
 
 
  
  Telephone No.
  
  
  Optional
  
  
  The “Telephone No.” is sourced from the Phone No. field on
  the Employee card for the employee.
  
 
 
  
  Payer Section
   
  
 
 
  
  Payer ABN
  
  
  Mandatory
  
  
  The “Payer ABN” is sourced from the ABN field on the
  Payroll card for the employee.
  
 
 
  
  Organisational Name
  
  
  Mandatory
  
  
  The “Organisational Name” is sourced from the Company Name
  field on the Payroll card for the employee.
  
 
 
  
  BSB Number
  
  
  Mandatory
  
  
  The “BSB Number” is sourced from the Bank Branch No. field
  on the company Bank Account.
  
 
 
  
  Account Number
  
  
  Mandatory
  
  
  The “Account Number” is sourced from the Bank Account No.
  field on the company Bank Account.
  
 
 
  
  Account Name
  
  
  Mandatory
  
  
  The “Account Name” is sourced from the Name field on the
  company Bank Account. 
  
 
 
  
  Payee/Receiver
  Section
   
  
 
 
  
  Payee/Receiver ABN
  
  
  Mandatory
  
  
  The “Payee/Receiver ABN” is sourced from the ABN field on
  the Superannuation Fund for the employee.
  
 
 
  
  USI
  
  
  Optional
  
  
  The “USI” is sourced from the USI field on the field on
  the Superannuation Product for the employee. 
  
 
 
  
  Organisation Name
  
  
  Mandatory
  
  
  The “Organisation Name” is sourced from the Fund Name
  field on the Superannuation Fund for the employee.
  
 
 
  
  Target Electronic Service Address
  
  
  Mandatory
  
  
  The “Target Electronic Service Address” is sourced from
  the Electronic Service Address field on the Superannuation Fund for the
  employee.
  
 
 
  
  Payment Method Code
  
  
  Mandatory
  
  
  The “Payment Method Code” is defaulted to DIRECT CREDIT
  
 
 
  
  Transaction Date
  
  
  Mandatory
  
  
  The “Transaction Date” is defaulted to the date as entered
  in by the user on the report request form.
  
 
 
  
  Payment/Customer Reference Number
  
  
  Optional
  
  
  The “Payment/Customer Reference Number” is not exported.
  
 
 
  
  Bpay Biller Code
  
  
  Optional
  
  
  The “Bpay Biller Code” is not exported.
  
 
 
  
  Payment Amount
  
  
  Mandatory
  
  
  The “Payment Amount” is the total value of the 
  
 
 
  
  BSB Number
  
  
  Mandatory
  
  
  The “BSB Number” is sourced from the Bank Branch No. field
  on the Superannuation Fund for the employee.
  
 
 
  
  Account Number
  
  
  Mandatory
  
  
  The “Account Number” is sourced from the Bank Account No.
  field on the Superannuation Fund for the employee.
  
 
 
  
  Account Name 
  
  
  Mandatory
  
  
  The “Account Name” is sourced from the Bank Name field on
  the Superannuation Fund for the employee.
  
 
 
  
  Employer Section
   
  
 
 
  
  Employer ABN
  
  
  Mandatory
  
  
  The “Employer ABN” is sourced from the Company ABN field
  on the Payroll card for the employee.
  
 
 
  
  Location ID
  
  
  Optional
  
  
  The “Location ID” is sourced from the Pay Centre ID field
  on the Superannuation Fund card for the employee.
  
 
 
  
  Organisational Name
  
  
  Mandatory
  
  
  The “Organisational Name” is sourced from the Company Name
  field on the Payroll card for the employee.
  
 
 
  
  Superannuation Fund Generated Employer ID
  
  
  Mandatory
  
  
  The “Superannuation Fund Generated Employer ID” is sourced
  from the Fund Employer No. field on the Superannuation Fund card for the
  employee.
  
 
 
  
  Super Fund Member
  Common
   
  
 
 
  
  Superannuation Fund Member TFN
  
  
  Mandatory
  
  
  The “Superannuation Member TFN” is sourced from the Tax
  File No. field on the Payroll Employee card for the employee.
  
 
 
  
  Person Name Title
  
  
  Optional
  
  
  The “Person Name Title” is sourced from the Title field on
  the Employee card for the employee.
  
 
 
  
  Person Name Suffix
  
  
  Optional
  
  
  The “Person Name Suffix” is not exported.
  
 
 
  
  Family Name
  
  
  Mandatory
  
  
  The “Family Name” is sourced from the Last Name field on
  the Employee card for the employee.
  
 
 
  
  Given Name
  
  
  Mandatory
  
  
  The “Given Name” is sourced from the Last Name field on
  the Employee card for the employee.
  
 
 
  
  Other Given Name
  
  
  Optional
  
  
  The “Other Given Name” is sourced from the Middle Name
  field on the Employee card for the employee.
  
 
 
  
  Gender
  
  
  Mandatory
  
  
  The “Gender” is sourced from the Gender field on the
  Employee card for the employee.
  
 
 
  
  Birth Date
  
  
  Mandatory
  
  
  The “Birth Date” is sourced from the Birth Date field on
  the Employee card for the employee.
  
 
 
  
  Address Usage Code
  
  
  Mandatory
  
  
  The “Address Usage Code” field is defaulted to POS.
  
 
 
  
  Address 1
  
  
  Mandatory
  
  
  The “Address 1” is sourced from the Address field on the Employee
  card for the employee.
  
 
 
  
  Address 2
  
  
  Optional
  
  
  The “Address 2” is sourced from the Address 2 field on the
  Employee card for the employee.
  
 
 
  
  Address 3
  
  
  Optional
  
  
  The “Address 3” is not supported.
  
 
 
  
  Address 4
  
  
  Optional
  
  
  The “Address 4” is not supported.
  
 
 
  
  Locality Name
  
  
  Mandatory
  
  
  The “Locality Name” is sourced from the City field on the
  Employee card for the employee.
  
 
 
  
  Post Code
  
  
  Mandatory
  
  
  The “Post Code” is sourced from the Post Code field on the
  Employee card for the employee.
  
 
 
  
  State
  
  
  Mandatory
  
  
  The “State” is sourced from the County field on the
  Employee card for the employee.
  
 
 
  
  Country
  
  
  Mandatory
  
  
  The “Country” is sourced from the Country field on the
  Employee card for the employee.
  
 
 
  
  E-mail Address
  
  
  Mandatory
  
  
  The “E-mail Address” is sourced from the E=Mail field on the
  Employee card for the employee.
  
 
 
  
  Telephone Landline
  
  
  Mandatory
  
  
  The “Telephone Landline” is sourced from the Phone No.
  field on the Employee card for the employee.
  
 
 
  
  Telephone Mobile No.
  
  
  Optional
  
  
  The “Telephone Mobile No.” is sourced from the Mobile No.
  field on the Employee card for the employee.
  
 
 
  
  Member Client Identifier
  
  
  Optional
  
  
  The “Member Client Identifier” is sourced from the
  Membership No. field on the Employee Superannuation card for the employee.
  
 
 
  
  Payroll Number Identifier
  
  
  Optional
  
  
  The “Payroll Number Identifier” is sourced from the
  Employee No. field on the Payroll Employee card for the employee.
  
 
 
  
  Employment End Date
  
  
  Optional
  
  
  The “Employment End Date” is sourced from the Termination
  Date field on the Payroll Employee card for the employee.
  
 
 
  
  Employment End Reason
  
  
  Optional
  
  
  The “Employment End Reason” is sourced from the Grounds
  for Termination Code field on the Employee card for the employee.
  
 
 
  
  Super Fund Member
  Contributions Section
  
 
 
  
  Pay Period Start Date
  
  
  Mandatory
  
  
  The “Pay Period Start Date” is the Contribution Start Date
  as entered by the user in the report request form.
  
 
 
  
  Pay Period End Date
  
  
  Mandatory
  
  
  The “Pay Period End Date” is the Contribution End Date as
  entered by the user in the report request form.
  
 
 
  
  Superannuation Guarantee Amount
  
  
  Optional
  
  
  The “Superannuation Guarantee Amount” is sourced from the
  Employer SGC contributions on the Superannuation Ledger Entry table.
  
 
 
  
  Award or Productivity Amount
  
  
  Optional
  
  
  The “Award or Productivity Amount” is not exported.
  
 
 
  
  Personal Contributions Amount
  
  
  Optional
  
  
  The “Personal Contributions Amount” is sourced from the
  Employee Post Tax on the Superannuation Ledger Entry table. 
  
 
 
  
  Salary Sacrificed Amount
  
  
  Optional
  
  
  The “Salary Sacrificed Amount” is sourced from the
  Employee Pre Tax on the Superannuation Ledger Entry table.
  
 
 
  
  Voluntary Amount
  
  
  Optional
  
  
  The “Voluntary Amount” is sourced from the Employer
  Non-SGC contributions on the Superannuation Ledger Entry table.
  
 
 
  
  Spouse Contributions Amount
  
  
  Optional
  
  
  This information is not exported.
  
 
 
  
  Child Contributions Amount
  
  
  Optional
  
  
  This information is not exported.
  
 
 
  
  Other Third Party Contributions Amount
  
  
  Optional
  
  
  This information is not exported.
  
 
 
  
  Super Fund Member
  Registration Section
   
  
 
 
  
  Employment Start Date
  
  
  Mandatory
  
  
  The “Employment Start Date” is sourced from the Employment
  Date field on the Payroll Employee card for the employee.
  
 
 
  
  At Work Indicator
  
  
  Optional
  
  
  The “At Work Indicator” is not supported.
  
 
 
  
  Annual Salary for Benefits Amount
  
  
  Optional
  
  
  The “Annual Salary Benefits Amount” is not exported.
  
 
 
  
  Annual Salary for Contributions Amount
  
  
  Optional
  
  
  The “Annual Salary for Contributions” is the Annual Salary
  for the employee calculated from the Employee Pay Rate information on the
  Payroll Employee card.
  
 
 
  
  Annual Salary for Contributions Effective Start Date
  
  
  Optional
  
  
  The “Annual Salary Contributions Effective Start Date” is
  not exported.
  
 
 
  
  Annual Salary for Contributions Effective End Date
  
  
  Optional
  
  
  The “Annual Salary for Contributions Effective End Date”
  is not exported.
  
 
 
  
  Annual Salary for Insurance Amount
  
  
  Optional
  
  
  The “Annual Salary for Insurance Amount” is the Annual
  Salary for the employee calculated from the Employee Pay Rate information on
  the Payroll Employee card. 
  
 
 
  
  Weekly Hours Worked Number
  
  
  Optional
  
  
  The “Weekly Hours Worked Number” is sourced from the Hours
  in a Full Week field on the Payroll Employee card for the employee.
  
 
 
  
  Occupation Description
  
  
  Optional
  
  
  The “Occupation Description” is sourced from the Job Title
  field on the Payroll Employee card for the employee.
  
 
 
  
  Insurance Opt Out Indicator
  
  
  Optional
  
  
  The “Insurance Opt Out Indicator” is not exported.
  
 
 
  
  Fund Registration Date
  
  
   
  
  
  The “Fund Registration Date” is sourced from the Date
  Joined Fund field on the Employee Superannuation card for the employee.
  
 
 
  
  Benefit Category 
  
  
  Optional
  
  
  The “Benefits Category” is not exported.
  
 
 
  
  Employment Status
  
  
  Mandatory
  
  
  The “Employment Status” is EMPLOYMENTSTATUS
  
 
 
  
  Superannuation Contribution Commence Date
  
  
  Optional
  
  
  The “Superannuation Contribution Commence Date” is not
  exported.
  
 
 
  
  Superannuation Contribution Cease Date
  
  
  Optional
  
  
  The “Superannuation Contribution Cease Date” is not
  exported.
  
 
 
  
  Member Registration Amendment Reason
  
  
  Optional
  
  
  The “Member Registration Amendment Reason” is not
  exported.
  
 
 
  
  Defined Benefits
  Contributions Section
  
 
 
  
  Defined Benefit Member Pre Tax Contribution
  
  
  Optional
  
  
  The “Defined Benefit Member Pre Tax Contribution” is not
  exported.
  
 
 
  
  Defined Benefit Post Tax Contribution
  
  
  Optional
  
  
  The “Defined Benefit Post Tax Contribution” is not
  exported.
  
 
 
  
  Defined Benefit Notional Employer Contribution
  
  
  Optional
  
  
  The “Defined Benefit Notional Employer Contribution” is
  not exported.
  
 
 
  
  Ordinary Time Earnings
  
  
  Optional
  
  
  The “Ordinary Time Earnings” is not exported.
  
 
 
  
  Actual Periodic Salary or Wages Earned
  
  
  Optional
  
  
  The “Actual Periodic Salary or Wages Earned” is not
  exported.
  
 
 
  
  Superannuable Allowances Paid
  
  
  Optional
  
  
  The “Superannuable Allowances Paid” is not exported.
  
 
 
  
  Notional Superannuable Allowances
  
  
  Optional
  
  
  The “Notional Superannuable Allowances” is not exported.
  
 
 
  
  Service Fraction
  
  
  Optional
  
  
  The “Service Fraction” is not exported.
  
 
 
  
  Service Fraction Effective Date
  
  
  Optional
  
  
  The “Service Fraction Effective Date” is not exported.
  
 
 
  
  Full Time Hours
  
  
  Optional
  
  
  The “Full Time Hours” is not exported.
  
 
 
  
  Contracted Hours
  
  
  Optional
  
  
  The “Contracted Hours” is not exported.
  
 
 
  
  Actual Hours Paid
  
  
  Optional
  
  
  The “Actual Hours Paid” is not exported.
  
 
 
  
  Employee Location Identifier
  
  
  Optional
  
  
  The “Employee Location Identifier” is not exported.
  
 
 
  
  Defined Benefits
  Registration Section
  
 
 
  
  Service Fraction
  
  
  Optional
  
  
  The “Service Fraction” is not exported.
  
 
 
  
  Service Fraction Start Date
  
  
  Optional
  
  
  The “Service Fraction Start Date” is not exported.
  
 
 
  
  Service Fraction End Date
  
  
  Optional
  
  
  The “Service Fraction End Date” is not exported.
  
 
 
  
  Defined Benefit Employer Rate
  
  
  Optional
  
  
  The “Defined Benefit Employer Rate” is not exported.
  
 
 
  
  Defined Benefit Employer Rate Start Date
  
  
  Optional
  
  
  The “Defined Benefit Employer Rate Start Date” is not
  exported.
  
 
 
  
  Defined Benefit Employer Rate End Date
  
  
  Optional
  
  
  The “Defined Benefit Employer Rate End Date” is not
  exported.
  
 
 
  
  Defined Benefit Member Rate
  
  
  Optional
  
  
  The “Defined Benefit Member Rate” is not exported.
  
 
 
  
  Defined Benefit Member Rate Start Date
  
  
  Optional
  
  
  The “Defined Benefit Member Rate Start Date” is not
  exported.
  
 
 
  
  Defined Member Rate End Date
  
  
  Optional
  
  
  The “Defined Member Rate End Date” is not exported.
  
 
 
  
  Defined Benefit Annual Salary 1
  
  
  Optional
  
  
  The “Defined Benefit Annual Salary 1” is not exported.
  
 
 
  
  Defined Benefit Annual Salary 1 Start Date
  
  
  Optional
  
  
  The “Defined Benefit Annual Salary 1 Start Date” is not
  exported.
  
 
 
  
  Defined Benefit Annual Salary 1 End Date
  
  
  Optional
  
  
  The “Defined Benefit Annual Salary 1 End Date” is not
  exported.
  
 
 
  
  Defined Benefit Annual Salary 2
  
  
  Optional
  
  
  The “Defined Benefit Annual Salary 2” is not exported.
  
 
 
  
  Defined Benefit Annual Salary 2 Start Date
  
  
  Optional
  
  
  The “Defined Benefit Annual Salary 2 Start Date” is not
  exported.
  
 
 
  
  Defined Benefit Annual Salary 2 End Date
  
  
  Optional
  
  
  The “Defined Benefit Annual Salary 2 End Date” is not
  exported.
  
 
 
  
  Defined Benefit Annual Salary 3
  
  
  Optional
  
  
  The “Defined Benefit Annual Salary 3” is not exported.
  
 
 
  
  Defined Benefit Annual Salary 3 Start Date
  
  
  Optional
  
  
  The “Defined Benefit Annual Salary 3 Start Date” is not
  exported.
  
 
 
  
  Defined Benefit Annual Salary 3 End Date
  
  
  Optional
  
  
  The “Defined Benefit Annual Salary 3 End Date” is not
  exported.
  
 
 
  
  Defined Benefit Annual Salary 4
  
  
  Optional
  
  
  The “Defined Benefit Annual Salary 4” is not exported.
  
 
 
  
  Defined Benefit Annual Salary 4 Start Date
  
  
  Optional
  
  
  The “Defined Benefit Annual Salary 4 Start Date” is not
  exported.
  
 
 
  
  Defined Benefit Annual Salary 4 End Date
  
  
  Optional
  
  
  The “Defined Benefit Annual Salary 4 End Date” is not
  exported.
  
 
 
  
  Defined Benefit Annual Salary 5
  
  
  Optional
  
  
  The “Defined Benefit Annual Salary 5” is not exported.
  
 
 
  
  Defined Benefit Annual Salary 5 Start Date
  
  
  Optional
  
  
  The “Defined Benefit Annual Salary 5 Start Date” is not
  exported.
  
 
 
  
  Defined Benefit Annual Salary 5 End Date
  
  
  Optional
  
  
  The “Defined Benefit Annual Salary 5 End Date” is not
  exported.
  
 
 
  
  Leave Without Pay Code
  
  
  Optional
  
  
  The “Leave Without Pay Code” is not exported.
  
 
 
  
  Leave Without Pay Code Start Date
  
  
  Optional
  
  
  The “Leave Without Pay Code Start Date” is not exported.
  
 
 
  
  Leave Without Pay Code End Date
  
  
  Optional
  
  
  The “Leave Without Pay Code End Date” is not exported.
  
 
 
  
  Annual Salary for Insurance Effective Date
  
  
  Optional
  
  
  The “Annual Salary for Insurance Effective Date” is not
  exported.
  
 
 
  
  Annual Salary for Benefits Effective Date
  
  
  Optional
  
  
  The “Annual Salary for Benefits Effective Date” is not
  exported.
  
 
 
  
  Employee Status Effective Date
  
  
  Optional
  
  
  The “Employee Status Effective Date” is not exported.
  
 
 
  
  Employee Benefit Category Effective Date
  
  
  Optional
  
  
  The “Employee Benefit Category Effective Date” is not
  exported.
  
 
 
  
  Employee Location Identifier
  
  
  Optional
  
  
  The “Employee Location Identifier” is not exported.
  
 
 
  
  Employee Location Identifier Start Date
  
  
  Optional
  
  
  The “Employee Location Identifier Start Date” is not
  exported.
  
 
 
  
  Employee Location Identifier End Date
  
  
  Optional
  
  
  The “Employee Location Identifier End Date” is not
  exported.
  
 




 

 

2.5.6.7    
QuickSuper Payment Format

The fields contained in the Quick
Super file are:

 




 
  
   
   Field Name
   
   
   Mandatory
   
   
   Description
   
  
 
 
  
  Your File Reference
  
  
  Mandatory
  
  
  This is your file reference, it needs to be different for
  each file you upload to QuickSuper.
   
  Most employers base their file reference on the date.
   
  It will be sourced from the Contribution End date when the
  file is generated.
  
 
 
  
  Your File Date
  
  
  Mandatory
  
  
  This is the date you upload your file to QuickSuper.  The date you enter must be the same for
  every employee.
  
 
 
  
  Contribution Period Start Date
  
  
  Mandatory
  
  
  This is the start date of your contribution period.  
  
 
 
  
  Contribution Period End Date
  
  
  Mandatory
  
  
  This is the end date of your contribution period.  
  
 
 
  
  Employer ID
  
  
  Mandatory
  
  
  Your employer ID as registered within QuickSuper.
  
 
 
  
  Payroll ID
  
  
  Mandatory
  
  
  Your Payroll ID is the number you use to identify your
  employees.
  
 
 
  
  Name Title
  
  
  Mandatory
  
  
  Titles must be entered in UPPERCASE.  The “Name Title” will be sourced from the
  “Title” field on the Employee card.
  
 
 
  
  Family Name
  
  
  Mandatory
  
  
  Family name is known as Last Name or Surname.  The “Family Name” field will be sourced
  from the “Last Name” field on the Employee card.
  
 
 
  
  Given Name
  
  
  Mandatory
  
  
  Enter the full name of your employee, not just the first
  initial.  
  The “Given Name” field will be sourced from the “First
  Name” field on the Employee card.
  
 
 
  
  Name Suffix
  
  
  Optional
  
  
  This information is relevant to very few employees, and
  the field can be left blank.
  
 
 
  
  Date of Birth
  
  
  Mandatory
  
  
  This field must be completed for every employee, in every
  upload file.
   
  The “Date of Birth” information will be sourced from the
  Birth Date field on the Employee card.
  
 
 
  
   Gender
  
  
  Mandatory
  
  
  The “Gender” information will be sourced from the Gender
  field on the Employee card.
  
 
 
  
  Tax File Number
  
  
  Mandatory
  
  
  You employee’s TFN will be passed to AustralianSuper by
  secure file delivery or by post to other funds.  TFNs will only be sent on the first time
  they are provided for an employee.
   
  The “TFN” information will be sourced from the “Tax File
  Number” field on the Payroll Employee card.
  
 
 
  
  Phone Number
  
  
  Optional
  
  
  It is not necessary to provide and employee phone number,
  but if you do it must be entered in the following format;
    [Area code] [Phone
  number]
   
  The “Phone Number” information will be sourced from the
  “Phone Number” field on the Employee card.
  
 
 
  
  Mobile Number
  
  
  Optional
  
  
  Mobile numbers must be entered in this format (with
  spaces):
  xxx xxx xxx.
   
  The “Mobile Number” information will be sourced from the “Mobile
  Number” field on the Employee card.
  
 
 
  
  Email Address
  
  
  Optional
  
  
  You can enter an employee’s email address. 
   
  The “Email Address” information will be sourced from the
  Employee card.
  
 
 
  
  Address 1
  
  
  Mandatory
  
  
  The “Address 1” is sourced from the Address field on the
  Employee card for the employee.
  
 
 
  
  Address 2 
  
  
  Optional
  
  
  The “Address 2” is sourced from the Address 2 field on the
  Employee card for the employee.
  
 
 
  
  Address 3
  
  
  Optional
  
  
  The “Address 3” is not exported.
  
 
 
  
  Address 4
  
  
  Optional
  
  
  The “Address 4” is not exported.
  
 
 
  
  Suburb
  
  
  Mandatory
  
  
  You must complete this field for employees with Australian
  addresses.  For international
  addresses, leave this field blank. 
   
  The “Suburb” is sourced from the City field on the
  Employee card for the employee.
  
 
 
  
  State
  
  
  Mandatory
  
  
  You must complete this field for employees with Australian
  addresses.  For international
  addresses, leave this field blank. 
   
  The “State” is sourced from the County field on the
  Employee card for the employee.
  
 
 
  
  Post Code
  
  
  Mandatory
  
  
  You must complete this field for employees with Australian
  addresses.  For international
  addresses, leave this field blank.
   
  The “Post Code” is sourced from the Post Code field on the
  Employee card for the employee.
  
 
 
  
  Country
  
  
  Mandatory
  
  
  Complete this field for both Australian or international addresses.
   
  The “Country” is sourced from the Country field on the
  Employee card for the employee.
  
 
 
  
  Employment Start Date
  
  
  Mandatory
  
  
  Enter the date your employee started working for your
  company.
   
  The “Employment Start Date” information will be sourced
  from the Employment Date field on the Employee card.
  
 
 
  
  Employment End Date
  
  
  Optional
  
  
  Enter the date your employee finished working for you.
   
  The “Employment End Date” is sourced from the Termination
  Date on the Employee card for the employee.
  
 
 
  
  Employment End Reason
  
  
  Optional
  
  
  Enter in the general reason why your employee stopped
  working with your company.
   
  The “Employment End Reason” information will be sourced
  from the Grounds of Termination Reason code on the Employee card.
  
 
 
  
  Fund ID
  
  
  Mandatory
  
  
  The Fund ID is the SPIN for the employee’s super fund,
  this will be provided on your employee’s Standard Choice form.  
   
  The “Fund ID” information will be sourced from the SPIN
  number contained on the Employee Superannuation card.
  
 
 
  
  Fund Name
  
  
  Mandatory
  
  
  Enter the full name of the Fund you are paying to.
   
  The “Fund Name” information will be sourced from the
  Superannuation Fund Name on the Employee Superannuation card.
  
 
 
  
  Fund Employer ID
  
  
  Optional
  
  
  This field can be populated if you’ve been given an
  Employer Number from the Fund that you are paying to.
   
  The “Fund Employer ID” information will be soured from the
  Employer ID field on the Employee’s Superannuation Fund card.
  
 
 
  
  Member ID
  
  
  Mandatory
  
  
  You must complete this field for every employee, in every
  file you upload.  This is the member
  number given to your employee by their super fund.
   
  The “Member ID” information will be sourced from the
  Member No. field on the Employee Superannuation card.
  
 
 
  
  Employer Super Guarantee Amount
  
  
  Mandatory
  
  
  The field contains the Super Guarantee (SG) amount being
  paid for each employee.
   
  
 
 
  
  Employer Additional Amount
  
  
  Optional
  
  
  This field contains the employer contribution amount being
  paid above the minimum SG amount for each employee (excluding salary
  sacrifice amounts).
  
 
 
  
  Member Salary Sacrifice
  
  
  Optional
  
  
  This field contains the salary sacrifice (before-tax)
  amount being paid on behalf of an employee.
  
 
 
  
  Member Additional Amount
  
  
  Optional
  
  
  This field contains any voluntary after-tax amount being
  paid by an employee.
  
 
 
  
  Other Contribution Type
  
  
  Optional
  
  
  Enter SPOUSE into this field to indicate that the amount
  entered under the Member Additional Amount column is a spouse contribution.
   
  If the Member Additional Amount column is left blank, or
  the amount entered is not a spouse contribution, leave this field blank.
  
 
 
  
  Other Contributor Name
  
  
  Optional
  
  
  If a Spouse contribution is being made, please provide the
  full name of the spouse.  If there is
  no spouse contribution, leave this field blank.
  
 
 
  
  Your Contribution Reference
  
  
  Optional.
  
  
  Your Contribution Reference will help you to identify each
  of the funds you are paying into.  This
  field can be left blank.
  
 




 

