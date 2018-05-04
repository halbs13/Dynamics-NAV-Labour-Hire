# How to Setup Commissions

This document will contain
information relating to the setup of Commissions and contains the following
sections:

- Account Manager Setup
- Commission Plans
- Commission Calculation
- Commission Reports
  - Account Manager Summary Report – Section 1
  - Account Manager Summary Report – Section 2     
     
# Account Manager Setup

Account Managers must be set up in the Sales
& Marketing granule. 

To access the salespeople records go to:

*Departments/Sales & Marketing/Sales/Salespeople*

To add a new record, click on the “New” icon.

|Field Name|Description|
|----------------------------------------------|----------------------------------|
|**GENERAL FASTTAB**||
|**Code**|Enter in a unique identifier.  The format can be alpha or numeric, or a combination of both.|
|**Name**|Enter in the name of the Account Manager|
|**Initials**|Enter in the Initials of the Account Manager|
|**Job Title**|Enter in the Job Title of the Account Manager|
|**Commission %**|The commission percentage is not used at this level|
|**Phone No.**|Record the phone number if applicable|
|**Email**|Record the Email address if applicable|  
|**INVOICING FASTTAB**|| 
|**Global Dimension 1**|This field is used to select the Global Dimension 1 Code. |
||Select the Global Dimension 1 Code from the “ArrowDown”.|
|**Global Dimension 2**|This field is used to select the Global Dimension 2 Code.|
||Select the Global Dimension 2 Code from the “ArrowDown”.|



# Commission Plans
 
When Account Managers are set up duringinitial implementation or as new Account Managers are hired they will need tohave a Commission Plan selected.  Thevalues found in this table will tell the Commission calculation program how tocalculate commission for this Account Manager.
To access the Commission Plans table, go to:

*Departments/Labour Hire/End of Period Processing/Commission Processing/Commission Plans*

|Field Name|Description|
|----------------------------------------------|----------------------------------|
|**Commission Type**|This calculation method applies to which commission type.  An Account Manager may have several entries that specify how to calculate commission on Permanent Placements and have different entries that specify how to calculate commission of Contractor/Temp Placements.  The options available are Perm and Temp.|
|**Account Manager Code**|Code used to identify the Account Manager.|
|**Account Manager Name**|The Account Managers full name| 
|**Perm Placement Fee Range Begin**|If Perm Placement fees are used to determine the commission percentage for this Account Manager then enter the starting range here.  For example, if a parameter is $0 - $6000 then $0 is entered here.|
|**Perm Placement Fee Range End**|If Perm Placement fees are used to determine commission percentage for this Account Manager then enter the ending range here.  For example, if a parameter is $0 - $6000 then $6000 is entered here.|
|**No. Contractors Range Begin**|If number of contractors paid this period is used to determine the commission percentage, then enter the starting range here.  For example, if a parameter is 0 – 9 contractors, then enter 0 here.|
|**No. Contractors Range End**|If number of contractors paid this period is used to determine the commission percentage, then enter the ending range.  For example, if a parameter is 0 – 9 contractors, then enter 9 here.|
|**Temp Margin Range Begin**|If Temporary Contractors Margin is used to determine the commission percentage, enter the starting range here.| 
|**Temp Margin Range End**|If Temporary Contractors Margin is used to determine the commission percentage, enter the ending range here.|
|**Total Perm/Margin Range Begin**|If Perm Fees plus Temporary Margins added together are used to determine commission percentage, enter the starting range here.| 
|**Total Perm/Margin Range End**|If Perm Fees plus Temporary Margins added together are used to determine the commission percentage, enter the ending range here.|
|**Commission Percentage**|Enter the commission percentage value that applies to this record.|
|**Deduction Amount**|If the Account Manager gets salary deducted from the calculated commission then enter the salary amount per calculation period.  (Enter on each line for that Account Manager).|
|**Prorate Temp/Perm**|If a Total Perm/Margin Range is used to calculate the percentage but the calculated amounts need to be split into separate Temp and Perm values then tick the Prorate field.|
|**Accrual Rate**|This is a Boolean field, which is used to indicate which line will be used to determine the highest rate for this Account Manager for commission accrual purposes.  There will be one perm line ticked and one Temp line ticked.|


# Commission Calculation
       
## Report Selection Criteria

To run the Commission Summary Report go to:

*Departments/Labour Hire/End of Period
Processing/Commission Processing/Commission Summary Report*

|Field Name|Description|
|-------------------------------------|---------------------------------------------------|
|**SALESPERSON/PURCHASE FASTTAB**|
|**Code**|Select and Account Manager or leave it blank to run for all Account Managers|  
|When you have completed your selection, you can either click “Print” to send the report to a printer or “Preview” to view the report to the screen.|
    
# Commission Reports 

There are 2 reports that are produced by this
process.

- Account Manager Summary Report
- Account Manager Audit Report

This first report is a summary report broken
into 2 sections that shows the following information in section 1

## Account Manager Summary Report – Section 1

COMMISSION SUMMARY REPORT

Account Manager Section

 

 

Commission for -                                                 Jo Bisa

Contracting Period -                                            01/04/01 – 29/04/01

Permanent Placement Period -                                    01/04/01 – 29/04/01

 

Total Contracting Margin                                                                     $33,697.10

Calculated at 10%                                                                                $15,000.00                              $1,500.00

Calculated at 15%                                                                                $18,697.10                              $2,804.56

 

Total Contracting Commission                                                                                                           $4,304.56

 

 

Total Permanent Placement Fees                                                       $20,000.00                              

Calculated at X%                                                                                 $10,000.00                              $2,000.00

Calculated at X%                                                                                 $10,000.00                              $2,046.40

 

Total Permanent Commission                                                                                                             $4,046.40

 

 



Total
Commission Payable                                                                                                                 $8,350.96

|Field Name|Description|
|-------------------------------------|---------------------------------------------------|
|**Commission For**|This is the Account Manager’s Name.|
|**Contracting Period**|Date range selected when the report is run.|
|**Permanent Placement Period**|Date range selected when the report is run.|
|**Total Contracting Margin**|Shows Total Margin Amounts for Temp placements for the period with the Account Manager’ s Commission percentages applied.|
|**Total Contracting Commission Value**|Total of Contracting Margin amounts.|
|**Total Perm Placement Fees**|Total amount of Permanent Placement fees for the period with the Account Manager’s Commission percentages applied.|
|**Total Permanent Commission Value**|Total of Perm Placement amounts.|
|**Total Commission Payable**|Total of Permanent and Contracting Commission totals.|
|**When you have completed your selection, you can either click “Print” to send the report to a printer or “Preview” to view the report to the screen.**||


The information contained in the lower section is as follows:

## Account Manager Summary Report – Section 2

 

#### Administration Section

|Department|Project|Permanent|Contract|Total|
|--------------|---------------|----------------|-------------------|------------------|
|NSW|IMB||2389.03|2389.03|
|NSW|GERNERAL|1000.00|1864.31|2864.31|
|NSW|OPTUS|3046.40|51.22|3097.62|
|Totals||4046.40|4304.56|8350.96|

To enable the breakup of amounts required in
the second section of the report above, we will need to capture department and
project for each transaction being included in the calculation and then split
the end commission values accordingly.

For example if the base contracting
transactions were split between Optus – 38%, IBM – 27.5% and General – 34.5%
and the commission calculated for an account manager for contract transactions
was $5000 then this total amount will be split accordingly between the three
projects.

 

### Account Manager Audit Report

The second report that is printed for each
Account Manager is the audit or detailed report that shows all of the
transactions that his/her commission has been calculated on for the period.

The report is formatted in 2 sections, the
first is the Temp Contractor details and the second is the Permanent Placement
details.

The following information will be shown for
the Contractor Details section:

- Period of Calculation
- Account Manager Name
- Client Code/Name
- Contractor Code Contractor Name
- Period Ending
- Units Paid/Worked
- Unit Frequency
- Pay Rate
- Gross Pay
- Charge Rate
- Invoiced Amount
- Workers Comp
- Payroll Tax
- Superannuation
- Commission Percentage
- Margin (Invoiced – Gross – On Costs)
- Subtotals for each Global Dimension combination   

The Permanent Placement Section includes the following:

- Period Of Calculation
- Account Manager Name
- Client Code/Name
- Placement Number
- Resource Name
- Start Date
- Creation Date
- Package Value
- Fee Rate
- Placement Fee
- Account Manager ownership percentage
- Account Manager Fee (Placement Fee * Account Manager %)
- Credit AmountDate Credited
- Commission Amount
- Account Managers (If others exist, code will be shown only)
- Subtotals for each Global Dimension combination

































 

