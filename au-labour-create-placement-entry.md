# How to create Placements in Placement Entry 

This section contains information relating to Placement Entry:

- [Placement Entry](#placement-entry)
- [Creating a New Temporary Placement](#creating-a-new-temporary-placement)
- [Record Maintenance](#record-maintenance)
- [Examples of Updates](#examples-of-updates)

## PLACEMENT ENTRY
Placement Entry is designed to be used as interface to Dynamics NAV for Recruitment organisations where integration from the front-end system into Dynamics NAV is not operational.   

Placement Entry allows for both Temporary and Permanent Placements to be entered and creates various records within Dynamics NAV to facilitate the Payroll and Billing processes associated with the Labour Hire module.  

1.  To access Placement Entry, go to the following menu; *Departments/Labour Hire/Candidate Processing/Placement Entry*

[GoToTop](#how-to-create-placements-in-placement-entry) 

## Creating a New Temporary Placement
All new placements are entered into the Placement Entry page.  Follow the steps below to correctly setup the Person (Employee/Contractor), Client (Customer) and Placement (Job and Resource Allocation).

1.  To create a new record, select the **New** icon on the **Home** ribbon.

2.  In the **Contractor Details Section** of the **Person** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------| 
|**Placement Type**|This is a mandatory field.  From the **ArrowDown**, select one of the following options; - Contractor – Temporary Placement, - Permanent – Permanent Placement.|
|**Candidate No.**|The Candidate No. will be the Employee/Contractor’s number.  This number should be created based on the number allocated from the front-end system, otherwise this number can be generated automatically from Dynamics NAV.|
|**Employment Date**|This is a mandatory field.  This field is used to record the Employee/Contractor’s start date with your organisation.|
|**Title**|This field is used to record the Employee/Contractor’s Title. e.g. Miss, Mrs, Mr.|
|**First Name**|This field is used to record the First Name of the Employee/Contractor.|
|**Last Name**|This field is used to record the Last Name of the Employee/Contractor.|
|**Middle Name**|This field is used to record the Middle Name of the Employee/Contractor.|
|**Sex**|This field is used to record the Gender of the Employee/Contractor.|
|**Address**|This field is used to record the Address of the Employee/Contractor.|
|**Address 2**|This field is used to record the extended address of the Employee/Contractor.|
|**City**|This field is used to record the City/Suburb of the Employee/Contractor’s address.|
|**Post Code**|This field is used to record the Post Code of the Employee/Contractor’s address. If the City/Suburb has been selected, the Post Code will default from the selection.|
|**County**|This field is used to record the County/State of the Employee/Contractor’s address. If the City or Post Code has been selected, the County will default from the selection.|
|**Phone No.**|This field is used to record the Phone No. of the Employee/Contractor.|
|**Work Phone No.**|This field is used to record the Work Phone No. of the Employee/Contractor.|
|**Mobile No.**|This field is used to record the Address of the Employee/Contractor.|
|**Home E-Mail Address**|This field is used to record an external E-Mail Address of the Employee/Contractor.  The information entered into this field will be used as the Primary E-Mail address to distribute Payment Summaries and Pay Advices.|
|**SMS**|This field is used to record the SMS Contact Address for messages to be sent to the Employee/Contractor.|
|**Company E-Mail**|This field is used to record the Company E-Mail of the Employee/Contractor.|
|**Other**|This field is used to record Other Contact information for the Employee/Contractor.|
|**Employee Type Code**|This is a mandatory field.  This field is used to identify in what capacity the Employee/Contractor is employed.  The value selected within the field also determines that type of Payment Summary the Employee/Contractor will receive.|
|**Timesheet Reminder**|This field is used to identify if a Timesheet Reminder is required for this Employee/Contractor.|
|**E-Mail Pay Advice**|This field is used to identify if Pay Advices are to be E-Mailed to the Employee/Contractor.|

3.  In the **Tax Details Section** of the **Person** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Tax Scale No.**|This field is used to record the Tax Scale No. of the Employee/Contractor.|
|**Tax File No.**|This field is used to record the Tax File Number of the Employee/Contractor.|
|**Birth Date**|This is a mandatory field.|
||This field is used to record the Birth Date of the Employee/Contractor.|
|**HELP Debt**|This field is used to record if the Employee/Contractor has a HELP debt.|
|**Student Loan (SFSS)**|This field is used to record if the Employee/Contractor has a Student Loan debt. |
|**Include for Payroll Tax**|This field is used to record if Payroll Tax is not applicable for this Employee/Contractor.  An example of where this might be used is if the employee is an Apprentice or trading as an Incorporated Company.|

4.  In the **Superannuation Details Section** of the **Person** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Superannuation Company Code**|This field is used to record the nominated Superannuation Fund of the Employee/Contractor.|
|**Membership No.**|This field is used to record the Employee/Contractor’s Superannuation Membership No.|
|**Date Joined Fund**|This field is used to record the Date the Employee/Contractor joined the Superannuation Fund.|

5.  In the **Financial Details Section** of the **Person** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Employee Job Posting Group**|This field is used to determine the Employee/Contractor’s Dimensions on the Payroll Employee Card.  The information entered here can be different to the Job Posting Group which is entered against the Placement.  However, there are also settings which will allow for the Dimensions to be sourced from the Job.|
|**Payroll No.**|This is a mandatory field.  This field is used to record the Payroll No. the Employee/Contractor’s pays will be processed in.|
|**Payment Method**|This is a mandatory field.  This field is used to record the Payment Method of which the Employee/Contractor will be paid.|

6.  If the Contractor is an Incorporated company, complete the **Incorporated Company Section** of the **Person** FastTab.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**A.B.N.**|This field is used to record the A.B.N. of the Employee/Contractor if they are trading as an Incorporated Company.|
|**Company Name**|This field is used to record the Company Name of the Employee/Contractor if they are trading as an Incorporated Company.|
|**Workers Comp Policy No.**|This field is used to record the Workers Comp Policy No. of the Employee/Contractor if they are trading as an Incorporated Company.|
|**Workers Comp Expiry Date**|This field is used to record the Expiry date of the Workers Comp Policy N. of the Employee/Contractor if they are trading as an Incorporated Company.|
|**Workers Comp Company Name**|This field is used to record the Workers Comp Company’s Name. of the Employee/Contractor’s Workers Comp policy if they are trading as an Incorporated Company.|

7.  In the **Bank Details Section** of the **Person** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**BSB Number**|This field is used to record the BSB Number of the Employee/Contractor.|
|**Bank Account Number**|This field is used to record the Bank Account Number of the Employee/Contractor.|
|**Bank Account Name**|This field is used to record the Bank Account Name of the Employee/Contractor.|

8.  On the **Client** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Customer No.**|From the **ArrowDown**, select the customer No. from the Customer List.  If the Customer exists within the list, then the following fields will be available for editing, otherwise to create a new customer you will need to complete the following fields.|
|**Name**|This field is used to record the Customer’s name.|
|**Name 2**|This field is used to record the Customer’s Name if the first field is not long enough to record the Customer’s full name.|
|**A.B.N**|This field is used to record the Customer’s Australian Business Number (A.B.N).|
|**Address**|This field is used to record the physical address of the Customer.|
|**Address 2**|This field is used to record the additional address information for the Customer if the first field is not long enough to record the Customer’s address.|
|**City**|From the **ArrowDown** button, select the City.|
|**Post Code**|From the **ArrowDown** button, select the Post Code.  If you select the “City” first, the Post Code will populate from the Post Code table.|
|**Country**|From the **ArrowDown** button, select the Country code.|
|**Contact No.**|This field is used to record the phone number of the Contact of the Customer.|
|**Contact**|This field is used to record the Contact’s Name of the Customer.|
|**Phone No.**|This field is used to record the Customer’s Phone No.|
|**Fax No.**|This field is used to record the Customer’s Fax No.|
|**E-Mail:**|This field is used to record the Customer’s E-Mail address.|

9.  In the **Contract Invoice Details Section** of the **Client** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Bill-to-Customer No.**|This field is populated if this customer transactions are being billed to another Customer. An example of where this is implemented is when a Customer has multiple locations and they are setup as separate customers, however their invoicing and other statements are sent to a Head Office.|
|**Payment Terms Code**|This field is used to record the Payment Terms.|
|**Customer Invoicing Frequency**|This field is used to record the frequency in which the customer is invoiced.  The following options are available; - Weekly, - Fortnightly, - Semi-Monthly, - Calendar Month, - 4 Week Month.|
|**Invoice/Cr. Format Code**|From the **ArrowDown**, select the Invoice/Cr. Format Code|
|**Job Invoice Consolidation Type**|This field determines how the Job transactional lines are consolidated on an invoice for this Customer.  The options available are; - Bill-to Customer No. + Sell-to Customer No., - Bill-to Customer No.|
|**Cust. Contact Job Title**|This field is used to record the Job Title of the Customer Contact|
|**Perm. Invoice/Cr. Format Code**|This field is used to record the Permanent Placement Invoice format.  From the **ArrowDown**, select the appropriate code.|
|**Perm Placement Payment Terms**|This field is used to record the Permanent Placement Payment Terms.  From the **ArrowDown**, select the appropriate code.|

10.  In the **Job Details Section** of the **Placement** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Placement Type**|This field is used to identify the placement being created.  The options available are; - Contractor – Temporary Placement, - Permanent – Permanent Placement.|
|**Job No.**|This field is used to record the Job. No. for the Placement record.|
|**Job Task No.**|This field is used to record the Job Task No. for the Placement record.|
|**Job Description**|This field is used to record the description of the Job.|
|**Job Starting Date**|This field is used to record the starting date of the Job.|
|**Job Ending Date**|This field is used to record the ending date of the Job.|
|**Job Purchase Order No.**|This field is used to record the purchase order no. for the Job.|
|**Job Revenue Type**|This field is used to record the Revenue Type or where the value of the revenue will be posted to within the General Ledger.|
|**Hiring Manager Name**|This field is used to record the name of the Hiring Manager|
|**Payroll Tax Code**|This field is used to record the Payroll Tax Code against the Job. If this field is populated with a Payroll Tax Code then the Payroll Tax Code will be taken from the Job No. for Employee transactions, otherwise it will be sourced from the Branch attached to the Employee.|

11.  In the **Financial Details Section** of the **Placement** FastTab, fill the fields as described in the folllowing table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Job Posting Group for Job**|This field is used to record the Posting Group for the Job which will determine the Dimensions for reporting purposes.|

12.  In the **Award Details Section** of the **Placement** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Classification Code**|This field is used to record the Classification Code for the Rateset information.|

13.  In the **Rateset Details Section** of the **Placement** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Transaction Type**|From the **ArrowDown** select the Transaction Type.|
|**Description**|This field will default to the Description of the Transaction Type that you select.|
|**Pay Rate**|This field is the Pay Rate to the Employee/Contractor.|
|**Charge Rate**|This field is the Charge Rate to the Client/Customer.|
|**Frequency**|This field is the Unit Rate Frequency of the Transaction Type.  The options are; - Hour, - Day, - Week, - Month, - Unit.|
|**Date Effective**|This field is the Date the Rateset is effective.|

14.  In the **Job Invoice Details Section** of the **Placement** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Job Bill-To Contact**|This field is used to record the Contact’s Name for the Job.  |
|**Job Bill-to Contact No.**|This field is used to record the contact number for the Contact of this Job.|
|**Job Bill-to Name**|This field is used to record the Bill-to Name.  This will default from the Customer Card.|
|**Job Bill-to Address**|This field is used to record the Bill-to Address.  This will default from the Customer Card.|
|**Job Bill-to Address 2**|This field is used to record the Bill-to Address 2.  This will default from the Customer Card.|
|**Job Bill-to City**|This field is used to record the Bill-to City.  This will default from the Customer Card.|
|**Job Bill-to Post Code**|This field is used to record the Bill-to Post Code.  This will default from the Customer Card.|
|**Job Bill-to Country Code**|This field is used to record the Bill-to Country.  This will default from the Customer Card.|
|**Job Bill-to Contact Job Title**|This field is used to record the Bill-to Contact Job Title.  This will default from the Customer Card.|

15.  In the **Work Site Section** of the **Placement** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Work Site Code**|This field is used to record the Work Site Code for the Job if this information is being reported to the Client/Customer.|
|**Work Site Address**|This field is used to record the Work Site Address for the Job if this information is being reported to the Client/Customer.|
|**Work Site Country/Region Code**|This field is used to record the Work Site Country/Region Code for the Job if this information is being reported to the Client/Customer.|
|**Work Site Post Code**|This field is used to record the Work Site Post Code for the Job if this information is being reported to the Client/Customer.|

16.  In the **Salespeople Section** of the **Salesperson** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Salesperson Code 1**|This field is used to record the Salesperson for this placement.  Select the Salesperson from the **ArrowDown**.|
|**Name**|This field will populate from the Salesperson record you have selected for this placement.|
|**Initials**|This field will populate from the Salesperson record you have selected for this placement.|
|**E-Mail**|This field will populated from the Salesperson record you have selected for this placement.|
|**Commission**|This field is used to record the percentage value which can be later used to calculate Commission payments for Sales people within your organisation.|
|**Salesperson Code 2.. Salesperson Code 3**|You can record up to 3 Sales people commission payment percentages on this placement.|

17.  Once you have completed entering the information, click **Transfer** icon on the **Home** ribbon.


[GoToTop](#how-to-create-placements-in-placement-entry)


## RECORD MAINTENANCE
Placement Entry is used to update information relating to the Job and the Ratesets associated to the Job, otherwise maintenance should occur in the following areas:

- Resources – Resource Card
- Human Resources – Employee Card
- Payroll – Payroll Employee Card
- Jobs – Job Card
- Customer – Customer Card


## Resources
The types of information you will update on the Resource Card will be discussed in this section.  It will not contain an explanation of all fields only those relative to the Labour Hire module.

To access the Resources Card, go to the following menu:

*Departments/Labour Hire/Candidate Processing/Resources* 

### Edit – Resource Card window
|Field|Description|
|------------------------------------------|--------------------------------------------------------------------| 
|**GENERAL FASTTAB**||
|**Name**|The name field appears on the Customer Invoice.|
|**Type**|The value in the Type field should be setup as “Person”|
|**Base Unit of Measure**|The value in the Base Unit of Measure field should be setup as “Hour”|
|**Job Posting Group**|This field is the Job Posting Group as entered in Placement Entry.|


|Field|Description|
|------------------------------------------|--------------------------------------------------------------------| 
|**INVOICING FASTTAB**||
|**Gen. Prod. Posting Group**|This field is used to determine what type of Product the Resource is for posting purposes.|
|**VAT/GST Prod. Posting Group**|This field is used to determine what type of Product the Resource is for GST purposes.|


|Field|Description|
|------------------------------------------|--------------------------------------------------------------------| 
|**PERSONAL FASTTAB**||
|**Address**|It is not necessary to update this field in the Resource Card as it is not currently used in the Labour Hire module.|
|**Post Code**|It is not necessary to update this field in the Resource Card as it is not currently used in the Labour Hire module.|
|**City**|It is not necessary to update this field in the Resource Card as it is not currently used in the Labour Hire module.|
|**Employment Date**|It is not necessary to update this field in the Resource Card as it is not currently used in the Labour Hire module.|
 

## Human Resources
The types of information you will update on the Employee Card will be discussed in this section.  It will not contain an explanation of all fields only those relative to the Labour Hire module.

To access the Employee Card, go to the following menu:

*Departments/Labour Hire/Candidate Processing/Employees*
 
### Edit – Employee Card window 

|Field|Description|
|------------------------------------------|--------------------------------------------------------------------| 
|**GENERAL FASTTAB**||
|**Title**|The Title field is used to specify the title of the Employee. E.g. Miss, Mrs, Mr, etc|
|**First Name**|The First Name field displays on all Payroll and Employee related reports for the Employee/Contractor.|
||If you update the Employee Card, the relevant fields will also be updated in the Payroll Employee card and vice versa.|
|**Last Name**|The Last Name field displays on all Payroll and Employee reports for the Employee/Contractor.|
||If you update the Employee Card, the relevant fields will also be updated in the Payroll Employee card and vice versa.|
|**Address**|The Address field displays on all relevant Payroll and Employee reports for the Employee/Contractor.|
||If you update the Employee Card, the relevant fields will also be updated in the Payroll Employee card and vice versa.|
|**Post Code, City, County, Country/Region Code**|These fields display on all relevant Payroll and Employee reports for the Employee/Contractor.|
||If you update the Employee Card, the relevant fields will also be updated in the Payroll Employee card and vice versa.|


|Field|Description|
|------------------------------------------|--------------------------------------------------------------------| 
|**COMMUNICATION FASTTAB**||
|**Mobile Phone No./Phone No.**|These fields display on all relevant Payroll and Employee reports for the Employee/Contractor.|
||If you update the Employee Card, the relevant fields will also be updated in the Payroll Employee card and vice versa.|
|**E-Mail**|This field is used to distribute pay advices and payment summaries via E-Mail.|


|Field|Description|
|------------------------------------------|--------------------------------------------------------------------| 
|**ADMINISTRATION FASTTAB**||
|**Status**|This field can be updated to Terminated should the Employee/Contractor leave your organisation.|


|Field|Description|
|------------------------------------------|--------------------------------------------------------------------|
|**PERSONAL FASTTAB**||
|**Birth Date**|This is a mandatory field. |
||The Birth Date is used in the calculation of Superannuation.  The Birth Date must be over 13 & 9 Months.|
 

## Payroll Employee
The types of information you will update on the Payroll Employee Card will be discussed in this section.  It will not contain an explanation of all fields only those relative to the Labour Hire module.

To access the Payroll Employee Card, go to the following menu:

*Departments/Labour Hire/Candidate Processing/Payroll Employees*
 
### Edit – Payroll Employee Card window 


|Field|Description|
|------------------------------------------|--------------------------------------------------------------------|
|**GENERAL FASTTAB**||
|**First Name**|The First Name field displays on all Payroll and Employee related reports for the Employee/Contractor.|
||If you update the Employee Card, the relevant fields will also be updated in the Payroll Employee card and vice versa.|
|**Last Name**|The Last Name field displays on all Payroll and Employee related reports for the Employee/Contractor.|
||If you update the Employee Card, the relevant fields will also be updated in the Payroll Employee card and vice versa.|
|**Address**|The Address field displays on all relevant Payroll and Employee reports for the Employee/Contractor.|
||If you update the Employee Card, the relevant fields will also be updated in the Payroll Employee card and vice versa.|
|**Post Code, City, County, Country/Region Code**|These fields display on all relevant Payroll and Employee reports for the Employee/Contractor.|
||If you update the Employee Card, the relevant fields will also be updated in the Payroll Employee card and vice versa.|
|**Employee Type Code**|The Employee Type code field determines what type of Payment Summary the Employee/Contractor will receive.|
|****|An example of when you might update this field is if an employee is changing from a PAYG Contractor to Incorporated Company.|
|**Payment Method**|The Payment Method field determines how the employee will be paid.|
||An example of when you might update this field is if an employee has not supplied banking details.|
|**Payroll No.**|The Payroll No. determines the frequency in which an employee is paid.|
||An example of when you might update this field is when an employee is changed from being paid on a weekly basis to monthly.|
|**Timesheet Reminders**|The Timesheet Reminders field identifies that this Employee/Contractor will receive timesheet reminders.|
|**E-Mail Pay Advice/E-Mail Payment Summaries**|These fields determine if the Employee/Contractor will receive their pay advices and payment summaries by E-Mail.|
||If you are selecting this field for the first time, you must ensure that the E-Mail address is populated on the Employee Card.|


|Field|Description|
|------------------------------------------|--------------------------------------------------------------------|
|**POSTING FASTTAB**||
|**Branch**|This field is used to record the Branch that the Employee/Contractor is employed it.|
|**Division**|This field is used to record the Division that the Employee/Contractor is employed it.|


|Field|Description|
|------------------------------------------|--------------------------------------------------------------------|
|**TAX FASTTAB**||
|**Tax Scale No.**|This field is used to record the Tax Scale No. as nominated by the Employee/Contractor.|
||Click on the “ArrowDown” button to select the appropriate Tax Scale.|
|**HELP Debt**|This field is used to record if the Employee/Contractor has a HELP Debt.|
|**Student Loan (SFSS)**|This field is used to record if the Employee/Contractor has a Student Loan.|
|**Fixed Tax Rate Applicable**|This field is used to record if the Employee/Contractor has a Fixed Tax Rate.  |
||If you check this box, you will be able to update the following fields;|
||·         Fixed Tax Rate Valid Until Date|
||·         Fixed Tax Rate|
|**Fixed Tax Rate Valid Until Date**|This field is used to record the Date the Fixed Tax Rate is valid until.|
|**Fixed Tax Rate**|This field is used to record the Fixed Tax Rate.  If it is 20%, then enter in 20.00.|
|**Medicare Reduction Applicable**|This field is used to record if the Medicare Reduction is applicable for the  Employee/Contractor. |
|**Number of Dependants**|This field is used to record the number of dependants the Employee/Contractor has.|
|**Payroll Tax Exempt**|This field is used to record if the wages for this Employee/Contractor are exempt from Payroll Tax.|
|**G.S.T Exempt**|This field is used to record if the wages for this Employee/Contractor are exempt from GST. |
||This information is only applicable for Employee/Contractor’s who operate as Incorporated Companies.|
|**Inc. Company Tax Inv. Not Req**|This field is used to record if a Tax Invoice is not required from the Employee/Contractor.|
||This information is only applicable for Employee/Contractor’s who operate as Incorporated Companies.|


|Field|Description|
|------------------------------------------|--------------------------------------------------------------------|
|**DECLARATION FASTTAB**||
|**Resident**|This field is used to record if the Employee/Contractor is a resident for taxation purposes.|
|**Tax Status**|This field is used to identify whether the Employee/Contractor is;|
||·         Australian Resident|
||·         Foreign Resident|
||·         Working Holiday Maker|
|**Tax Free Threshold Claimed**|This field is used to identify if the Employee/Contractor is claiming the Tax Free threshold.|
|**Claim FTB**|This field is used to identify if the Employee/Contractor is claiming the Family Tax Benefit.|
|**Claim Zone Allowance**|This field is used to identify if the Employee/Contractor is claiming a Zone Allowance.|
|**Zone**|This field is used to identify what type of Zone Allowance is being claimed.|
|**HELP Debt**|This field is used to identify if the Employee/Contractor has a HEP Debt.|
|**Student Loan (SFSS)**|This field is used to identify if the Employee/Contractor has a Student Loan.|
|**Claim Pension Rebate**|This field is used to identify if the Employee/Contractor is claiming a Pension Rebate.|
|**Use TFN for Super**|This field is used to identify if the Employee/Contractor has specified to send the Tax File Number to the Superannuation Fund.|
|**Senior Australians Tax Offset Claimed**|This field is used to identify if the Employee/Contractor is claiming the Senior Australians Tax Offset.|
|**Rebates Amt. Claimed**|This field is used to identify the Rebate Amounts being claimed by the Employee/Contractor.|
|**A.B.N**|This field is used to record the A.B.N if the Employee/Contractor is operating as an Incorporated Company.|
|**Incorporated Company Name**|This field is used to record the Incorporated Company Name if the Employee/Contractor is operating as an Incorporated Company.|
|**Tax File No.**|This field is used to record the Tax File Number of the Employee/Contractor.|
|**Birth Date**|This field is used to record the Birth Date of the Employee/Contractor.|
|**Date Declaration Signed**|This field is used to record the date the Employment Declaration form was signed by the Employee/Contractor.|
|**Payee Signature**|This field is used to identify if the Employment Declaration form was signed by the Employee/Contractor.|
|**Declaration Lodged**|This field is used to identify that the Declaration was extracted to be lodged with the Australian Taxation Office.|
 

|Field|Description|
|------------------------------------------|--------------------------------------------------------------------|
|**WORK COVER FASTTAB**||
|**Work Cover Code**|This field is used to record if the Work Cover Code for the Employee/Contractor.|
||It is used to calculate a Work Cover provision.|
|**Work Cover Location Code**|This field is used to record the Work Cover Location Code for the Employee/Contractor.|
||It is used to calculate a Work Cover provision.|
|**Workers Comp Policy No.**|This field is used to record the Workers Comp Policy No. for the Employee/Contractor if they are operating as an Incorporated Company.|
|**Workers Comp Insurer**|This field is used to record the Workers Comp Insurer for the Employee/Contractor if they are operating as an Incorporated Company.|
|**Policy Expiration Date**|This field is used to record the Workers Comp Policy Expiration Date for the Employee/Contractor if they are operating as an Incorporated Company.|
  
## Payroll Employee – Pay Dissections
You can update the Employee/Contractor’s bank details from the Pay Dissections menu on the Payroll Employee Card.

To access the Pay Dissections, go to the following menu:

*Departments/Labour Hire/Candidate Processing/Payroll Employees/Pay Dissections*

 
### Edit – Employee Pay Dissections Card window


 |Field|Description|
|------------------------------------------|--------------------------------------------------------------------|
|**Pay Transaction Type**|Select the Pay Transaction Type code from the “ArrowDown” button.|
||The Net Pay Transaction Type is setup on the Payroll Setup Card.|
|**Pay Dissection Type**|This field identifies whether the Bank Account details is the Main account or a Part account where a set amount of percentage of the net income can be disbursed to. |
|**Bank Account No.**|This field is used to record the Employee/Contractor’s Bank Account No. |
||It is restricted to 9 digits.|
|**Bank Account Name**|This field is used to record the Employee/Contractor’s Bank Account Name.|
|**Pay Bank State Branch No.**|This field is used to record the Employee/Contractor’s Pay Bank State Branch No. (BSB)|
|**Standard Amount**|This field is used to record the value of monies to be disbursed into the account.|
||Populate this field if you are adding an additional account which will have a “Pay Dissection Type” = “Part”.|
|**Standard %**|This field is used to record the percentage of the net income to be disbursed into the account.|
||Populate this field if you are adding an additional account which will have a “Pay Dissection Type” = “Part”.|
|**Not Used**|This field is used to suspend the transaction for one pay period only.|
||When the pay period is closed, the check mark is removed making it available again in the next pay.|


## Payroll Employee – Deductions
You can update the Employee/Contractor’s deduction details from the Deductions menu on the Payroll Employee Card.

To access the Deductions, go to the following menu:

*Departments/Labour Hire/Candidate Processing/Payroll Employees/Deductions*

### Edit – Employee Deductions Card window
 
|Field|Description|
|------------------------------------------|--------------------------------------------------------------------|
|**Transaction Type Code**|Select the Pay Transaction Type code from the “ArrowDown” button.|
|**Shift Code**|This field is used to identify if this deduction is to generate when a certain Shift Code is selected.|
||This field is optional and will be dependent upon the setup.|
|**Priority**|This field is used to determine the priority in which the deduction will be deducted from the Employee/Contractor’s pay.|
||This is useful when and Employee/Contractor has a schedule of deductions.|
|**Start Date**|This field is used to record the Start Date of when the Deduction should start.|
|**End Date**|This field is used to record the End Date of when the Deduction should cease.|
|**Description**|This field is used to describe the Deduction and will default from the Pay Transaction Type Code. |
||You can update the description if required to something more meaningful as reference for the Employee/Contractor.|
|**Standard Amount**|This field is used to record the amount of the Deduction per pay period.|
|**Standard %**|This field is used to record the standard percentage of the Deduction per pay period.|
|**Details**|This field is used to record any reference information relating to the Deduction.|
|**Total Deduction**|This field is used to record the Total Amount of the Deduction.|
||This field is used to accommodate reducing balance deductions.|
|**LTD Amount**|This field will display the “Life-To-Date” amount of the Deduction.|
|**Not Used**|This field is used to suspend the transaction for one pay period only.|
||When the pay period is closed, the check mark is removed making it available again in the next pay.|

 
## Payroll Employee – Superannuation
You can update the Employee/Contractor’s Superannuation details from the Superannuation menu on the Payroll Employee Card.

To access the Superannuation, go to the following menu:

*Departments/Labour Hire/Candidate Processing/Payroll Employees/Superannuation*

 
### Edit – Employee Superannuation List window 
 |Field|Description|
|------------------------------------------|--------------------------------------------------------------------|
|**Superannuation Code**|Select the Pay Transaction Type code from the “ArrowDown” button.|
|**Membership No.**|This field is used to record the Employee/Contractor’s Membership No. for their Superannuation fund.|
|**Date Joined Fund**|This field is used to record the Date the Employee/Contractor’s Joined their fund.|
|**Starting Date**|This field is used to record the Starting Date of the Superannuation fund.|
|**Ending Date**|This field is used to record the Ending Date of the Superannuation fund.|
|**Employer SGC Amt.**|This field is used to record the Employer SGC Amt.  This value can default from the setup on the Superannuation fund. (Superannuation Product Card).|
|**Employer SGC %**|This field is used to record the Employer SGC % value.  This value can default from the setup on the Superannuation fund (Superannuation Product Card).|
|**Employer Factor**|This field is used to record the Employer Factor value.  This value can default from the setup on the Superannuation fund (Superannuation Product Card).|
|**Employer Non-SGC Amt.**|This field is used to record the Employer Non-SGC Amt value.  This value can default from the setup on the Superannuation fund or specifically setup in this area if it relates to this Employee/Contractor only.|
|**Employer Non-SGC %**|This field is used to record the Employer Non-SGC % value.  This value can default from the setup on the Superannuation fund or specifically setup in this area if it relates to this Employee/Contractor only.|
|**Employee Salary Sacrifice Amt**|This field is used to record the Employee Salary Sacrifice Amount value as nominated by the Employee/Contractor.|
|**Employee Salary Sacrifice %**|This field is used to record the Employee Salary Sacrifice % value as nominated by the Employee/Contractor.|
|**Employee Post-Tax Std. Amt.**|This field is used to record the Employee Post-Tax Standard Amount as nominated by the Employee/Contractor.|
|**Employee Post-Tax Standard %**|This field is used to record the Employee Post-Tax Standard % as nominated by the Employee/Contractor.|


## Payroll Employee – Employer On Costs
You can update the Employee/Contractor’s Employer On Cost details from the Accumulation Calculations menu on the Payroll Employee Card.

To access the Employer On Costs, go to the following menu:

*Departments/Labour Hire/Candidate Processing/Payroll Employees/Accumulation Calculations/Employer On Costs*

 
### Edit – Employee Accum. Calc. Rates window 
 |Field|Description|
|------------------------------------------|--------------------------------------------------------------------|
|**Transaction Type Code**|Select the Pay Transaction Type code from the “ArrowDown” button.|
|**Start Date**|This field is used to record the Start Date of the Employer On Cost Transaction.|
|**End Date**|This field is used to record the End Date of the Employer On Cost Transaction.|
|**Pay Rate**|This field is used to record the Pay Rate as a % value and expressed in decimal format.|
||If the value is 9.5%, then enter in 0.095.|
|**Superannuation Code**|This field is used to record the Employee/Contractor’s Superannuation Code.  |
||Click on the “ArrowDown” button to select the Superannuation Fund.|
|**Not Used**|This field is used to suspend the transaction for one pay period only.|
||When the pay period is closed, the check mark is removed making it available again in the next pay.|


## Jobs
The types of information you will update on the Jobs Card will be discussed in this section.  It will not contain an explanation of all fields only those relative to the Labour Hire module.  

The types of information you may update on the Jobs Card are:
• Hiring Manager via the Invoice FastTab
• Account Managers/Salespeople via the Home ribbon

To access the Jobs Card, go to the following menu:

*Departments/Labour Hire/Candidate Processing/Jobs*
 
## Customers

The types of information you will update on the Customer Card will be discussed in this section.  It will not contain an explanation of all fields only those relative to the Labour Hire module.  

The types of information you may update on the Customer Card are:
- Name
- Address
- Phone Numbers
- Contact Information
- Invoice Format
- Job Invoice Consolidation Type
- Invoice Frequency
- Permanent Placement Invoice Format-• Payment Terms Code
- Perm Placement Payment Terms Code
- Customer Specific Fields

To access the Customer Card, go to the following menu:

*Departments/Labour Hire/Candidate Processing/Customer*

### Edit – Customer Card window 
 |Field|Description|
|------------------------------------------|--------------------------------------------------------------------|
|**GENERAL FASTTAB**||
|**Name**|This field is used to store the name of the Customer.|


 |Field|Description|
|------------------------------------------|--------------------------------------------------------------------|
|**ADDRESS & CONTACT FASTTAB**||
|**Address**|This field is used to record the Address of the Customer.|
|**Phone No.**|The Customer Phone Number is stored on the Contact Card.|


|Field|Description|
|------------------------------------------|--------------------------------------------------------------------| 
|**INVOICING FASTTAB**||
|**Invoice/Cr. Memo Format Code**|This field is used to record the Customer’s Invoice/Cr. Memo Format.|
||Click on the “ArrowDown” button to select an appropriate code.|
|**Perm. Invoice/Cr. Format Code**|This field is used to record the Customer’s Perm Invoice/Cr. Memo Format.|
||Click on the “ArrowDown” button to select an appropriate code.|
|**Req. Inv./Cr. Format Code**|This field is used to record the Customer’s Invoice/Cr. Memo Format.|
||Click on the “ArrowDown” button to select an appropriate code.|
|**Job Invoice Consolidation Type**|This field is used to record the Job Invoice Consolidation Type.  The options are;|
||·         Bill-To Customer No.|
||·         Bill-To Customer No. + Sell-to Customer No.|
|**Job Invoice Grouping**|This field is used to identify how the invoices will group.  The following options are;|
||·         Alternate Date|
||·         Job Posting Group|
||·         Job Bill-To Contact|
||·         Job No. |
||·         Job Task No.|
 

|Field|Description|
|------------------------------------------|--------------------------------------------------------------------| 
|**PAYMENTS FASTTAB**||
|**Payment Terms Code**|This field is used to record the Customer’s standard Payment Terms.|
||Click on the “ArrowDown” button to select an appropriate code.|
|**Perm. Placement Payment Terms**|This field is used to record the Customer’s Permanent Placement Payment Terms.|
||Click on the “ArrowDown” button to select an appropriate code.|




|Field|Description|
|------------------------------------------|--------------------------------------------------------------------| 
|**USER DEFINED FASTTAB**||
|**Field No. 1 Required..Field No. 10 Required**|This field is used to record whether additional reporting is being captured from the Employee/Contractor’s timesheet. |
||If one of the fields are selected, then a heading must be entered in the Field 1 Label, etc.|

[GoToTop](#how-to-create-placements-in-placement-entry)

## EXAMPLES OF UPDATES
This section will outline examples of when information is updated and where these updates should occur.

### Placement Entry

Placement Entry is used to update information relating to the Job and the Ratesets.  These areas are;

- Extending a Contract
- Updating the Rate sets

### Extending a Contract

Extending Contracts is performed in Placement Entry.  You will also need to know the Employee/Contractor, the Customer No. and the Job and Job Task No. to update the information successfully.

To access Placement Entry, go to the following menu:

*Departments/Labour Hire/Candidate Processing/Placement Entry*

 Use the following steps to perform this process:

1. Click on the “New” icon on the Home ribbon.

2. Go the Person FastTab, select the Placement Type in the “Placement Type” field.

3. Go the “Candidate No.” field and click on the “ArrowDown” and select the Employee.


Once you retrieve the Employee record, there will be some “greyed” out fields which means that these fields are not editable from within the Placement Entry window.   

When you see this screen, then proceed to the “Client” FastTab.

1. Go to the Customer No. field and click on the “ArrowDown” and select the Customer.

Once you retrieve the Customer record, there will be some “greyed” out fields which means that these fields are not editable from within the Placement Entry window.   When you see this screen, then proceed to the “Placement” FastTab.


1. Go to the Job No. field, click on the “ArrowDown” and select the Job No.

2. Go to the Job Task No. field, click on the “ArrowDown” and select the Job Task No. for this Job.

3. Once you select the first two fields, other fields will be populated accordingly.

4. If you are extending a Contract, update the End Date of the record.  Do not update the Starting Date as this will create a new record.4.1.2 Update the Rateset


1. New Ratesets are entred in the “Placement Entry Rates” window.

2. Enter you in the Transaction Type Code.
3. Enter in the Pay & Charge Rate.
4. Go to the Frequency field and click on the “ArrowDown” and select the frequency.
5. Go to the Date Effective field and enter in the a new effective date.After you have updated this information, then click on the “Transfer” icon to update the various tables within Dynamics NAV.

## Non-Placement Entry

There is other maintenance which are performed directly on the card.  Some of the examples of these updates are:
- Employee/Contractor Terminates
- Transfer from PAYG Contractor to Company

### Contractor Terminates

If an Employee/Contractor terminates employment then the updates should occur as follows:

1. Update the Ending Date on the Job via Placement Entry.  This will ensure that no timesheets will generate for the Employee/Contractor.

2. Update the following fields on the Administration FastTab of the Employee Card:
 
   * Status – update to Terminated
   * Terminated Date – enter in the Termination Date
   * Grounds for Term. Code – click on the “ArrowDown” button and select the Termination Reason code.

### Transfer from PAYG to Company

If an Employee/Contractor transfers from being a PAYG Contractor to an Incorporated Company, then the updates should occur as follows.  As a general rule, these updates should not occur part way through a pay period and should be effective as at the first day of the next pay period if at all possible.


1. Update the following FastTabs on the Payroll Employee Card:
   * General FastTab – Employee Type Code – update this from PAYG to Incorporated Company.
   * Tax FastTab – Tax Scale – update the Tax Scale value to be GST.
   * Declaration FastTab
     * A.B.N – update the A.B.N accordingly,
     * Incorporated Company Name – update the Incorporated Company Name.
   * Work Cover FastTab – Enter in the Workers Comp Insurer, Policy No. and Policy Expiration Date   

2. You may also need to update the Rateset details on the Job so you will need to perform this via Placement Entry using the same process as described in the previous section.

[GoToTop](#how-to-create-placements-in-placement-entry)
