# How to: setup Resources & Jobs

1      INTRODUCTION

1.1      
Configuration Overview

The Dynamics
NAV Labour Hire module comprises and requires various areas within Dynamics NAV
to be configured in order for it to operate. 
Those areas include:

General LedgerSales &
ReceivablesPurchase &
PayablesResources &
JobsHuman Resources
& PayrollLabour Hire











 

This document will discuss the following Resources &
Jobs Setup areas required to operate the Dynamics NAV Labour Hire module.

 


 Resources Setup
 Job Setup
 Job Posting Groups


 

.

 

2     
RESOURCES SETUP

2.1      
Resources Setup

A number series must be setup for Resource
records, regardless of whether the number will be manually entered into
Dynamics NAV or transferred via the interface.

To access the Resource Setup, go to the following
menu:

Departments/Resource Planning/Setup/Resources Setup



2.1.1    
“Resources Setup” window

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  Resource Nos. 
  
  
  Select the Resources No. series from the “ArrowDown”.
  If there is integration with AXiOM, the
  Employee Numbers will be generated from within AXiOM and transfer into NAV, however
  this field should still be configured. 
  **Note:
  The No. Series should be setup first. 
  You will need to create a new No. series if one does not exist.
  
 
 
  
  Time Sheet No.s
  
  
  This feature relates specifically to standard
  time sheets using Resources and Machines and should not be confused with Time
  Sheet Entry used in the Labour Hire module or TimeKeeper.
  
 
 
  
  Time Sheet First Week Day
  
  
  This feature relates specifically to standard
  time sheets using Resources and Machines and should not be confused with Time
  Sheet Entry used in the Labour Hire module or TimeKeeper.
  
 
 
  
  Time Sheet By Job Approval
  
  
  This feature relates specifically to standard
  time sheets using Resources and Machines and should not be confused with Time
  Sheet Entry used in the Labour Hire module or TimeKeeper.
  
 
 
  
  Click “OK” after
  you have completed your selection.
  
 


3     
JOBS SETUP

3.1      
Jobs Setup

A number series must be setup for Job records,
regardless of whether the number will be manually entered into Dynamics NAV or
transferred via the interface.

To access the Job Setup, go to the following
menu:

Departments/Jobs/Setup/Setup



3.1.1    
“Jobs Setup” window

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  GENERAL FASTTAB
  
 
 
  
  Automatic Update Job Item Cost 
  
  
  This field is used to automatically adjust cost
  changes each time the “Adjust Cost – Item Entries” batch job is run.
  This field is not used in Labour Hire.
  
 
 
  
  Apply Usage Link by Default
  
  
  This field indicates whether job ledger entries
  are linked to job planning lines by default. 
  Select this check box if you want to apply this setting to all new
  jobs that you create.
  This field is not used in Labour Hire.
  
 
 
  
  Default WIP Method
  
  
  This field specifies the default method to be
  used for calculating work in progress (WIP). 
  It is applied whenever you create a new job, but you can modify the
  value on the job card.
  This field is not used in Labour Hire.
  
 
 
  
  Default WIP Posting Method
  
  
  This field specifies how the default WIP method
  is to be applied when posting work in progress (WIP) to the general
  ledger.  By default, it is applied per
  job.
  This field is not used in Labour Hire.
  
 
 
  
  Default Job Posting Group
  
  
  This field specifies the default posting group
  to be applied when you create a new job. 
  This group is used whenever you create a job, but you can modify the
  value on the job card.
  This field is not used in Labour Hire. 
  
 
 
  
  NUMBERING FASTTAB
  
 
 
  
  Job Nos.
  
  
  Select the Job No. series from the “ArrowDown”.  
  If there is integration with AXiOM, the Job
  Numbers will be generated from within AXiOM and transfer into NAV, however
  this field should still be configured. 
  **Note:
  The No. Series should be setup first. 
  You will need to create a new No. series if one does not exist.
  
 
 
  
  Job WIP Nos.
  
  
  Select the Job WIP No. series from the “ArrowDown”.  
  This field is not used in Labour Hire.
  
 
 
  
  Click “OK” after
  you have completed your selection.
  
 


 

3.2      
Job Posting Group

Job Posting Groups are used through the Labour Hire module to set
defaults such as Dimensions, Payroll Branch and Division and Product Posting
Groups.  Where there is integration into
the AXiOM product, the Job Posting Group it is transferred across as the “Cost
Centre” code which can be later selected on the Order.

To setup the Job Posting Groups, go to the
following menu:

Departments/Jobs/Setup/Job Posting Groups

 

3.2.1    
“Job Posting Groups” window

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  To create a new record, click on the “New” button.
  
 
 
  
  Code
  
  
  Enter in a Code that uniquely identifies the
  Job Posting Group.  The Code field
  allows for up to 10 characters.
  
 
 
  
  WIP Costs Account
  
  
  The WIP account
  for the calculated cost of the job WIP which is a Balance sheet capital asset
  account. 
  This field is not used in Labour Hire.
  
 
 
  
  WIP Accrued Costs Account
  
  
  An account for
  the Cost Value or Cost of Sales method of WIP calculation which is a Balance
  sheet accrued expense liability account. This will be posted to when the WIP adjustment
  requires usage costs posted to the income statement be increased.
  This field is not used in Labour Hire
  
 
 
  
  Job Costs Applied Account
  
  
  The balancing
  account to WIP Cost Account which is a contra for negative expense account.
  This field is not used in Labour Hire.
  
 
 
  
  Job Costs Adjustment Account
  
  
  The balancing
  account to WIP Accrued Costs account which is an expense account.
  This field is not used in Labour Hire.
  
 
 
  
  G/L Expense Acc. (Contract)
  
  
  The sales
  account to be used for G/L expenses in job tasks with this posting group. If
  left empty, the G/L account entered on the planning line will be used.
  This field is not used in Labour Hire.
  
 
 
  
  WIP Accrued Sales Account
  
  
  The WIP account
  for the calculated sales value of the WIP which is a Balance Sheet Accrued
  Revenue account. This will be posted to when the WIP adjustment requires the
  recognised revenue to be increased.
  This field is not used in Labour Hire.
  
 
 
  
  WIP Invoiced Sales Account
  
  
  The account for
  the invoiced sales value of the WIP which is not able to be recognised. It is
  a Balance Sheet Unearned Revenue account.
  This field is not used in Labour Hire.
  
 
 
  
  Job Sales Applied Account
  
  
  The balancing
  account to WIP Invoiced Sales account which is a contra income account.
  This field is not used in Labour Hire.
  
 
 
  
  Job Sales Adjustment Account
  
  
  The balancing
  account to WIP Sales Account which is an income account.
  This field is not used in Labour Hire.
  
 
 
  
  Recognised Costs Account
  
  
  The expense
  account containing the recognised costs for the job. It is a DR expense
  account normally.
  This field is not used in Labour Hire.
  
 
 
  
  Recognised Sales Account
  
  
  The income
  account containing the recognised income for the job. It is a CR income
  account normally.
  This field is not used in Labour Hire.
  
 
 
  
  Description
  
  
  Enter in a Description which accurately
  describes the Job Posting Group.
  ** The description field will be transferred
  into Cost Centre field within AXiOM.
  
 
 
  
  Payroll No.
  
  
  Select the Payroll No. from the “ArrowDown” which this Job Posting Group transaction
  belongs to.  
  The Payroll No. is restricted to 6
  characters.  
  
 
 
  
  Payroll Group
  
  
  The Payroll Group field is used to group the
  Cost Centre codes for selection in AXiOM by transferring to the “Ledger Code”.   
  Enter in a Code with a maximum of 6 characters.
  
 
 
  
  Branch Code
  
  
  Select the Branch Code from the “ArrowDown” for this Job Posting Group transaction.
  
 
 
  
  Division Code
  
  
  Select the Division Code from the “ArrowDown” for this Job Posting Group transaction.
  
 
 
  
  Global Dimension 1
  
  
  Select the Dimension Code from the “ArrowDown” for this Job Posting Group transaction.
  
 
 
  
  Global Dimension 2
  
  
  Select the Dimension Code from the “ArrowDown” for this Job Posting Group.
  
 
 
  
  Gen. Prod. Posting Group
  
  
  From the AssistButton button, select the Gen.
  Prod. Posting Group for this Job Posting Group.
  
 
 
  
  Exclude from Integration
  
  
  This field is used to identify transactions
  which should no longer be included in the transfer of data to AXiOM.
  
 
 
  
  Click “OK” after
  you have completed your selection.
  
 


 

3.2.2    
Additional Dimensions – “Edit – Default
Dimensions”

 

Additional dimensions can be setup by clicking on the “Dimensions” button.  

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  To create a new record, click on the “New” button.
  
 
 
  
  Dimension Code
  
  
  Select the additional dimension you wish to add
  from the “ArrowDown”.
  
 
 
  
  Dimension Value Code
  
  
  Select the additional dimension value you wish
  to add from the “ArrowDown”.
  
 
 
  
  Value Posting
  
  
  This option is not required at this level and
  is generally setup and maintained on G/L Accounts.
  
 
 
  
  Click “OK” after
  you have completed your selection.
  
 


 
