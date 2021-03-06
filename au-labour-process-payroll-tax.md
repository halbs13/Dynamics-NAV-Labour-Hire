# How to process Payroll Tax


Payroll Tax processing within the Dynamics NAV Payroll and Labour Hire modules encompasses the following functions:  

- Setup
  - Payroll Tax State Codes
  - Payroll Tax Groups
  - Payroll Tax State Rates
  - Allocating Payroll Tax State Codes to Payroll Branches
  - Payroll Tax Transactions allocated to Pay Transaction Types
- Payroll Tax Reporting

This section will specifically discuss how to use the Payroll Tax Report within Dynamics NAV.  

## Payroll Tax Overview

Payroll Tax is calculated as a percentage of the Employee’s Pay. The Pay Transactions used in the calculation contain a Payroll Tax Transaction Accumulator setup in the Payroll Tax option. Superannuation is also included in the Payroll Tax report.

To ensure that each of the employee pay transactions applicable to Payroll Tax are calculated you must ensure every Employee has a **Branch** assigned to their record on Payroll Employee card on the **Posting** FastTab and every Branch has a Payroll Tax code assigned to the Branch.

# CALCULATE PAYROLL TAX

1.  To access the Calculate Payroll Tax task, go to the following menu: *Departments/Payroll/EOM Processing/Payroll Tax Processing/Calculate Payroll Tax*

2.  On the **Options** FastTab, fill the fields as described in the following table.
 
|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Payroll No.**|Select the **Payroll No.** you wish to use to calculate Payroll Tax otherwise leave blank for all payrolls.|
|**Payroll Tax Code**|Select the Payroll Tax Code that you wish to calculate Payroll Tax otherwise leave blank for all Payroll Tax codes.|
|**Start Month Date**|Select the first day of the month that you wish to include in your payroll tax calculation.|
|**End of Month Date**|The **End of Month Date** defaults once you have entered the **Start of Month Date** field. The values in this field cannot be changed.|
|**Print Branch Summary**|Select this field to print a summarised cost allocation for each Branch.|
|**Print Department Summary**|Select this field to print a summarised cost allocation for each Department.|

3.  If you wish to preview the report to screen, click **Preview**.

4.  If you wish to print the report to a printer or save as a pdf, click **Print** and select the relevant option.

## Payroll Tax Report

The Payroll Tax report will contain each of the Pay Transaction Types which are applicable to the relevant Payroll Tax code.  The Posted Payroll Summary Report, if produced in detail will be used to verify the value on the transactions on the Payroll Tax report.  

The fields on the Calculate Payroll Tax Report are:

|Report Field|Field No.|Obtained from|
|------------------------------------|-----------|---------------------------------------------------|
|**State Code**|(1)|This is the State Code|
|**State Description**|(2)|This is the State Description|
|**Transaction Code**|(3)|This is the Pay Transaction Type Code which has been defined as being applicable to Payroll Tax.|
|**Transaction Description**|(4)|This is the Description of the Pay Transaction Type Code.|
|**Amount (LCY)**|(5)|This is a sum of the Amount of all the Pay Transaction Type codes.|
|**Employer SGC/Non SGC**|(6)|This is the sum of the Employer SGC and Non SGC amounts for the Payroll Tax state.|
|**Salary Sacrifice**|(7)|This is the sum of the Salary Sacrifice or Pre Tax Superannuation Deduction amount for the Payroll Tax state.|
|**Fringe Benefits Estimate**|(8)|This is the value of the Fringe Benefits Estimate as setup on the Payroll Tax Rates record.|
|**Grand Total**|(9)|This is the sum of values in the **Transaction Detail**, **Superannuation Summary** and **Other Amounts Summary** sections.|
|**Australia Wide Wages**|(10)|This is the sum of all wages Australia Wide.|
|**State Wide Wages**|(11)|This is the sum of all wages applicable for the Payroll Tax within the Payroll Tax State.|
|**Gross Taxable Wages**|(12)|This is the sum of all Gross Taxable Wages applicable to Payroll Tax.|
|**Plus Adjustment**|(13)|This is the value of the Adjustment as setup on the Payroll Tax Rates record.|
|**Less Deduction**|(14)|This is the value of the Monthly Deduction as setup on the Payroll Tax Rates record.|
|**Net Taxable Wages**|(15)|This is the sum of the **Gross Taxable Wages** and **Plus Adjustment**, **Less Deduction**.  If the value is negligible then zero will be represented in this field.|
|**Tax Rate**|(16)|This is the Tax Rate as setup on the Payroll Tax Rates record.|
|**Payroll Tax Payable**|(17)|This is the value of the Payroll Tax Payable for the State.|

- The lower section of the first page will contain a breakdown of the calculated information.

- The second page of the report contains a breakdown of the Gross Taxable Wages and Payroll Tax Payable by Payroll Branch and Division.

- The last page of the report will contain a breakdown of the Gross Taxable Wages and Payroll Tax Payable by Dimension.

[GoToTop](#how-to-process-payroll-tax)
