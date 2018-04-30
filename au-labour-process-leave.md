# How to: setup and process leave 

1.         
Introduction

This document has been prepared
as a training manual for users of the Dynamics NAV2017 Labour Hire Suite
module.

 

Leave processing within the
Dynamics NAV Payroll and Labour Hire modules encompasses the following
functions:  

 

SetupLeave
Types and AccrualsEmployee Leave Entitlement Calculation and  Reporting This document will specifically
discuss how to use the Leave Processing function within Dynamics NAV.  For further information relating to the setup
of each of these areas, please refer to the Dialog – Training – LH – Payroll
Setup Configuration document. The activities discussed are: Mass Adjust Leave BalancesCalculate & Post ProvisionEmployee Leave Entitlement Report  

























2.      
leave  Processing

1   
 

2   
 



2.1    Mass
Adjust Leave Balance

 

1. 

The Mass Adjust Leave Balance function is used
to adjust leave entitlements or pro rata balances in the employee leave ledger
to correct leave balances.  It is also
used to enter entitlements when implementing a new Payroll system.  You can choose to post the Leave to the
General Ledger or only update the Payroll Employee Leave Ledger entries.

To access the Mass Adjust Leave Balance task, go
to the following menu:

Departments/Payroll/EOM Processing/Leave
Processing/ Mass Adjust Leave Balance



 

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  Employee No
  
  
  Select the Employee No. from the “ArrowDown”.
  
 
 
  
  Leave Type
  
  
  Select the Leave Type from the “ArrowDown”.
  
 
 
  
  Leave Code
  
  
  Select the Leave Code from the “ArrowDown”.
  
 
 
  
  Document Type
  
  
  Select the Document Type from the “ArrowDown”. 
  (
  Entitlement, Pro Rata, Pro Rata Vae, or Value Only ).
  
 
 
  
  Leave Period Posting
  Date
  
  
  Enter the Leave Period Posting Date of the leave
  adjustment.  The Leave Period Posting
  Date identifies the Leave Anniversary period the transaction will appear in. 
  
 
 
  
  Posting Date
  
  
  Enter the Posting Date of the leave
  adjustment.
  
 
 
  
  Document No.
  
  
  Enter the Document No of the leave
  adjustment.
  
 
 
  
  No. of Hours ( Adj )
  
  
  Enter the number of hours and minutes (If
  the Payroll card “Show Leave in Hours” is ticked) you wish to adjust the
  leave. Eg. -40, 25.5, etc.
  
 
 
  
  No. of Days ( Adj )
  
  
  Enter the number of days (If the Payroll
  card “Show Leave in Hours” is not ticked) you wish to adjust the leave.
  
 
 
  
  Value
  
  
  This field will populate automatically from
  the No. of Hours / Days entered.
  
 
 
  
  Adjustment Description
  
  
  Enter a “Description” of the leave adjustment.
  
  
 
 
  
  Tick Data Take-On
  Column
  
  
  Tick this option to only affect the Payroll
  leave balances and not to post the adjustment to the General Ledger. This
  option is used to enter leave balances for a payroll implementation. Leave
  this option blank to post the provision to the General Ledger.
  
 
 
  
  Un-tick Data Take-On
  Column
  
  
  Select this option to post the provision to
  the General ledger.
  
 
 
  
  On 
  completion of the above fields then press the “Post” button – this option posts the Leave adjustment to the Employee Leave
  Sub-Ledger and General Ledger Leave Provision accounts.
  
 


 

 

2.2       Calculate
and Post Provision

 

The Calculate Leave
Provision calculates the Leave Accrual and Entitlements and posts them to the
General Ledger Granule of Microsoft Dynamics Nav Financials.

 

This Report uses
the current Leave Days accrued and entitled for each Employee and multiplies
these by each current Employee rate to calculate the provision value for each
Employee.

 

To access the Calculate and Post Provision task, go to the following
menu:

Departments/Payroll/EOM
Processing/Leave Processing/ Calculate & Post Provision

 



 

 


 
  
   
   Field Name
   
   
   
   Description
   
   
  
 
 
  
  OPTIONS FASTTAB – Only the standard fields are covered. A full list
  of fields available as filters can be used by selecting the first blank line
  and clicking the “ArrowDown”.
  
  
 
 
  
  Date of Calculation
  
  
  
  Enter the date the calculation will affect the general ledger.
  
  
 
 
  
  Document No.
  
  
  
  Enter the “Document No.” to assign to the posted transactions. 
  
  
 
 
  
  Post to G/L
  
  
  
  Tick this field to post the provision to the General Ledger.
  
  
 
 
  
  LEAVE TYPE FASTTAB – Only the standard fields are covered. A full
  list of fields available as filters can be used by selecting the first blank
  line and clicking the “ArrowDown”.
  
  
 
 
  
  Code
  
  
  
  Select the Leave Type you wish to process. If left blank then all
  leave types are processed.
  
  
 
 
  
  PAYROLL EMPLOYEE FASTTAB – Only the standard fields are covered. A
  full list of fields available as filters can be used by selecting the first
  blank line and clicking the “ArrowDown”.
  
  
 
 
  
  Employee No.
  
  
  
  Select the Employee No. from the “ArrowDown”.
  If left blank all
  employees are selected.
  
  
 
 
  
  If you wish to preview the report to screen,
  you should ensure that you un-click “Post to GL” and then
  click “Preview”.
  If you wish to post the Leave Accruals to
  the General Ledger, you should ensure that “Post to GL” is TICKED and print the report.   You can send the report to a printer or
  save as a pdf, click “Print” and select the relevant option.
  
  
 


 



 

2.3       Employee
Leave Entitlement Report

The Employee Leave Entitlement Report provides
you with a list of employees who have leave accruals assigned.   

To access the Employee Leave Entitlement Report,
go to the following menu:

Departments/Payroll/EOM Processing/Leave
Processing/Employee Leave Entitlement Report



2.3.1    
Edit: Employee Leave Entitlement 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  OPTIONS
  FASTTAB
  
 
 
  
  As At Date
  
  
  Enter in the date you wish to generate the
  report.  
  You can only enter in a date where
  transactions have been posted to the Leave Accrual Ledger Entry.  
  
 
 
  
  Exclude Zero Accruals
  
  
  Select this field if you wish to exclude accruals
  with a zero balance.
  
 
 
  
  Group by Global
  Dimension 1
  
  
  Select this field if you wish to group
  employees by Global Dimension 1.
  
 
 
  
  Print Leave As:
  
  
  You can nominate how you wish the leave
  accruals to appear in the report.  The
  options you have available are:
  ·        
  Decimal Hours
  ·        
  Hours &
  Minutes
  ·        
  Days
  
 
 
  
  Exclude LSL not
  Provisioned
  
  
  Select this field if you wish to exclude LSL
  not yet provisioned.
  
 
 
  
  LEAVE
  TYPE FASTTAB - Only the standard fields are covered. A full list of fields
  available as filters can be used by selecting the add filter.
  
 
 
  
  Code
  
  
  ·        
  Select the Leave Code for the Leave Types you wish to report on. If
  left blank all Leave Type codes are selected. 
  
 
 
  
  PAYROLL
  EMPLOYEE FASTTAB - Only the standard fields are covered. A full list of
  fields available as filters can be used by selecting the add filter.
  
 
 
  
  Payroll No.
  
  
  Enter in the Payroll No. you wish to report
  on, otherwise leave blank for all.
  
 
 
  
  Employee No.
  
  
  Enter in the Employee No. you wish to report
  on, otherwise leave blank for all.
  
 
 
  
  Branch Code
  
  
  Enter in the Payroll Branch Code you wish to
  report on, otherwise leave blank for all.
  
 
 
  
  Division Code
  
  
  Enter in the Payroll Division Code you wish
  to report on, otherwise leave blank for all.
  
 
 
  
  If
  you wish to preview the report to screen, click “Preview”. 
  If you wish to print the report to a printer or save as a pdf, click “Print” and select the relevant option.
  
 


 

 


