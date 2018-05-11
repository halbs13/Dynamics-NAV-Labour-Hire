# How to setup and process leave 

Leave processing within the Dynamics NAV Payroll and Labour Hire modules encompasses the following functions:  

- Setup Leave Types and Accruals
- Calculating & Posting Leave Provisions
- Employee Leave Entitlement Reporting

This section pecifically discusses how to use the Leave Processing function within Dynamics NAV.  The activities discussed are:

- [Mass Adjust Leave Balances](#mass-adjust-leave-balance)
- [Calculate and Post Provision](#calculate-and-post-provision)
- [Employee Leave Entitlement Report](#employee-leave-entitlement-report)


# LEAVE  PROCESSING

### Mass Adjust Leave Balance

The Mass Adjust Leave Balance function is used to adjust leave entitlements or pro rata balances in the employee leave ledger to correct leave balances.  It is also used to enter entitlements when implementing a new Payroll system.  You can choose to post the Leave to the General Ledger or only update the Payroll Employee Leave Ledger entries.

1. To access the **Mass Adjust Leave Balance**, go to the following menu:  *Departments/Payroll/EOM Processing/Leave Processing/ Mass Adjust Leave Balance*

2.  Fill in the fields as described in the following table.
 
|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Employee No**|Select the Employee No. from the **ArrowDown**.|
|**Leave Type**|Select the Leave Type from the **ArrowDown**.|
|**Leave Code**|Select the Leave Code from the **ArrowDown**.|
|**Document Type**|Select the Document Type from the **ArrowDown**.  The Options are *Entitlement, Pro Rata, Pro Rata Value, or Value Only* ).|
|**Leave Period Posting Date**|Enter the Leave Period Posting Date of the leave adjustment.  The Leave Period Posting Date identifies the Leave Anniversary period the transaction will appear in. |
|**Posting Date**|Enter the Posting Date of the leave adjustment.|
|**Document No.**|Enter the Document No of the leave adjustment.|
|**No. of Hours ( Adj )**|Enter the number of hours you wish to adjust the leave by.|
|**No. of Days ( Adj )**|Enter the number of days if you are accruing leave in days.|
|**Value**|This field will populate automatically from the No. of Hours / Days entered.|
|**Adjustment Description**|Enter a **Description** of the leave adjustment.|

3.  Once you have entered in the adjustments, you can select the **Data Take-On Column** icon, based on the following;

- **Tick Data Take-On Column** - select this option to only affect the Payroll leave balances and not to post the adjustment to the General Ledger. This option is used to enter leave balances for a payroll implementation. Leave this option blank to post the provision to the General Ledger.  
- **Un-tick Data Take-On Column** - select this option to post the provision to the General ledger.

4.  On completion of the above fields then press the **Post** icon – this option posts the Leave adjustment to the Employee Leave Sub-Ledger and General Ledger Leave Provision accounts.

[GoToTop](#how-to-setup-and-process-leave)

## Calculate and Post Provision

The Calculate Leave Provision calculates the Leave Accrual and Entitlements and posts them to the General Ledger module of Dynamics Nav Financials.

This Report uses the current Leave Days accrued and entitled for each Employee and multiplies these by each current Employee rate to calculate the provision value for each Employee.
 
1.  To access the Calculate and Post Provision task, go to the following menu: *Departments/Payroll/EOM Processing/Leave Processing/ Calculate & Post Provision*

2.  On the **Options** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Date of Calculation**|Enter the date the calculation will affect the general ledger.|
|**Document No.**|Enter the **Document No.** to assign to the posted transactions.|
|**Post to G/L**|Tick this field to post the provision to the General Ledger.|

3.  On the **Leave Type** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Code**|Select the Leave Type you wish to process. If left blank then all leave types are processed.|

4.  On the **Payroll Employee** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Employee No.**|Select the Employee No. from the **ArrowDown**. If left blank all employees are selected.|

5.  Tf you wish to preview the report to screen, you should ensure that you un-check **Post to GL** and then click **Preview**. 

6.  If you wish to post the Leave Accruals to the General Ledger, you should ensure that **Post to GL** is **TICKED** and print the report.   You can send the report to a printer or save as a pdf.  Click **Print** and select the relevant option.

[GoToTop](#how-to-setup-and-process-leave)
 
## Employee Leave Entitlement Report

The Employee Leave Entitlement Report provides you with a list of employees who have leave accruals assigned.   

1.  To access the Employee Leave Entitlement Report, go to the following menu: *Departments/Payroll/EOM Processing/Leave Processing/Employee Leave Entitlement Report*

2.  On the **Options** FastTab, fill the fields as described in the following table.
 
### Edit: Employee Leave Entitlement 

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**As At Date**|Enter in the date you wish to generate the report.|
||You can only enter in a date where transactions have been posted to the Leave Accrual Ledger Entry.|
|**Exclude Zero Accruals**|Select this field if you wish to exclude accruals with a zero balance.|
|**Group by Global Dimension 1**|Select this field if you wish to group employees by Global Dimension 1.|
|**Print Leave As:**|You can nominate how you wish the leave accruals to appear in the report.  The options you have available are: *Decimal Hours, Hours & Minutes,Days*.|
|**Exclude LSL not Provisioned**|Select this field if you wish to exclude LSL not yet provisioned.|

3.  On the **Leave Type** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Code**|Select the Leave Code for the Leave Types you wish to report on. If left blank all Leave Type codes are selected.|

4.  On the **Payroll Employee** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Payroll No.**|Enter in the Payroll No. you wish to report on, otherwise leave blank for all.|
|**Employee No.**|Enter in the Employee No. you wish to report on, otherwise leave blank for all.|
|**Branch Code**|Enter in the Payroll Branch Code you wish to report on, otherwise leave blank for all.|
|**Division Code**|Enter in the Payroll Division Code you wish to report on, otherwise leave blank for all.|

5.  If you wish to preview the report to screen, click **Preview**.

6.  If you wish to print the report to a printer or save as a pdf, click **Print** and select the relevant option.

[GoToTop](#how-to-setup-and-process-leave)
