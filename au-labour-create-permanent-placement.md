# How to create Permanent Placements

This section contains information relating to Permanent Placements/Requirements Billing:

- [Permanent Placement Overview](#permanent-placement-overview) 
  - [Fee Types](#fee-types)
  - [Permanent Placement via Placement Entry](#permanent-placement-via-placement-entry) 
  - [Permanent Placement Cards](#permanent-placement-cards) 
  
- [Permanent Placement Invoicing](#permanent-placement-invoicing)
  - [Permanent Placement Invoice Parameters](#permanent-placement-invoice-parameters) 
  - [Generating Permanent Placement Invoices](#generating-permanent-placement-invoices)

- [Requirements Invoicing Overview](#requirements-invoicing-overview)
  - [Requirements Invoicing Setup](#requirements-invoice-setup)
  - [Requirements Invoice Parameters](#requirements-invoice-parameters)
  - [Generating Requirements Invoices](#generating-requirements-invoices)

## PERMANENT PLACEMENT OVERVIEW
Permanent Placements are candidates who apply for positions advertised by recruitment agencies on behalf of their clients with the intention of being permanently placed.

Permanent Placement records can be setup from within the Placement Entry area of the Labour Hire module with information such as the expected salary the candidate will receive, placement fees, the guarantee period and placement fee information. 
 
[GoToTop](#how-to-create-permanent-placements)

## Fee Types
Fee Types are setup to identify where the revenue for the fees will post to within the General Ledger.

1. In the **Search** box, enter **Fee Types**, and then choose the related link. Or go to the following menu: *Departments/Payroll/Setup/Labour Hire/Administration/Fee Types*  

2. On the **General** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Code** |This field is used to setup a unique code for the Fee Type.|
|**Description**|This field is used to describe the Fee Type.|
|**Fee Type**|This field is used to identify whether the Fee Type is a Placement Fee or Requirement Fee.|
|**G/L Account No.**|This field is used to specify the General Ledger Account.|

[GoToTop](#how-to-create-permanent-placements)

## Permanent Placement via Placement Entry
Permanent Placement records are setup within the Placement Entry area of the Labour Hire module.  The following FastTabs are used when creating a new Permanent Placement record:

- Client (Customer) FastTab
- Perm Placement FastTab
 

Upon transferring data from this area, the following records are created within various areas of Dynamics NAV:
  - Resource Card
  - Job Card
  - Job Placement Fee
  - Customer Card 

1. In the **Search** box, enter in **Placement Entry**, and then choose the related link.  Or go to the following menu: *Departments/Labour Hire/Candidate Processing/Placement Entry* 

2.  To create a new record, select the **New** icon on the **Home** ribbon.

3.  On the **Client** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Customer No.**|From the **ArrowDown** button, select the customer No. from the Customer List.  If the Customer exists within the list, then the following fields will be available for editing, otherwise to create a new customer you will need to complete the following fields.|
|**Name**|This field is used to record the Customer’s name.|
|**Name 2**|This field is used to record the Customer’s Name if the first field is not long enough to record the Customer’s full name.|
|**A.B.N**|This field is used to record the Customer’s Australian Business Number (A.B.N).|
|**Address**|This field is used to record the physical address of the Customer.|
|**Address 2**|This field is used to record the additional address information for the Customer if the first field is not long enough to record the Customer’s address.|
|**City**|From the **ArrowDown** button, select the City.|
|**Post Code**|From the **ArrowDown** button, select the Post Code. If you select the **City** first, the Post Code will populate from the Post Code table.|
|**Country**|From the **ArrowDown** button, select the Country code.|
|**Contact No.**|This field is used to record the phone number of the Contact of the Customer.|
|**Contact**|This field is used to record the Contact’s Name of the Customer.|
|**Phone No.**|This field is used to record the Customer’s Phone No.|
|**Fax No.**|This field is used to record the Customer’s Fax No.|
|**E-Mail:**|This field is used to record the Customer’s E-Mail address.|

4.  In the **Contract Invoice Details Section** of the **Clients** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Bill-to-Customer No.**|This field is populated if this customer transactions are being billed to another Customer.  An example of where this is implemented is when a Customer has multiple locations and they are setup as separate customers, however their invoicing and other statements are sent to a Head Office.|
|**Payment Terms Code**|This field is used to record the Payment Terms.|
|**Customer Invoicing Frequency**|This field is used to record the frequency in which the customer is invoiced.  The following options are available; - Weekly, - Fortnightly, - Semi-Monthly, - Calendar Month, - 4 Week Month|
|**Invoice/Cr. Format Code**|From the **ArrowDown**, select the Invoice/Cr. Format Code|
|**Job Invoice Consolidation Type**|This field determines how the Job transactional lines are consolidated on an invoice for this Customer.  The options available are; - Bill-to Customer No. + Sell-to Customer No., - Bill-to Customer No.|
|**Cust. Contact Job Title**|This field is used to record the Job Title of the Customer Contact|
|**Perm. Invoice/Cr. Format Code**|This field is used to record the Permanent Placement Invoice format.  From the **ArrowDown**, select the appropriate code.|
|**Perm Placement Payment Terms**|This field is used to record the Permanent Placement Payment Terms.  From the **ArrowDown** button, select the appropriate code.|

5.  On the **Candidate Details Section** of the **Perm Placement** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Placement Type**|This field is used to identify the placement being created.  To create the Permanent Placement, select **Permanent**.|
|**Employee No.**|This field is used to create an Employee No. on the Resource Card.  Enter in a unique number for the Candidate.|
|**First Name**|This field is used to record the First Name of the Candidate.|
|**Last Name**|This field is used to record the Last Name of the Candidate.|

6.  On the **Job Details Section** of the **Permanent Placement** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Job No.**|This field is used to record the Job. No. for the Permanent Placement record.|
|**Job Task No.**|This field is used to record the Job Task No. for the Permanent Placement record.|
|**Job Description**|This field is used to record the description of the Job.|
|**Job Starting Date**|This field is used to record the starting date of the Job.|
|**Job Purchase Order No.**|This field is used to record the purchase order no. for the Job.|
|**Job Revenue Type**|This field is used to record the Revenue Type or where the value of the Permanent Placement will be posted to within the General Ledger.|
|**Job Posting Group for Job**|This field is used to record the Posting Group for the Job which will determine the Dimensions for reporting purposes.|

7.  On the **Job Invoice Details Section** of the **Permanent Placement** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Job Bill-To Contact**|This field is used to record the Contact’s Name for the Job.|
|**Job Bill-to Contact No.**|This field is used to record the contact number for the Contact of this Job.|
|**Job Bill-to Name**|This field is used to record the Bill-to Name.  This will default from the Customer Card.|
|**Job Bill-to Address**|This field is used to record the Bill-to Address.  This will default from the Customer Card.|
|**Job Bill-to Address 2**|This field is used to record the Bill-to Address 2.  This will default from the Customer Card.|
|**Job Bill-to City**|This field is used to record the Bill-to City.  This will default from the Customer Card.|
|**Job Bill-to Post Code**|This field is used to record the Bill-to Post Code.  This will default from the Customer Card.|
|**Job Bill-to Country Code**|This field is used to record the Bill-to Country.  This will default from the Customer Card.|
|**Job Bill-to Contact Job Title**|This field is used to record the Bill-to Contact Job Title.  This will default from the Customer Card.|

8.  On the **Permanent Placement Details Section** of the **Permanent Placement** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Candidate Source**|This field identifies how the Candidate was sourced for this Permanent Placement and can be used for reporting purposes.  The options available are; - Newspaper/Magazine, - Internet, - Database, - Referral.|
|**Agreed Salary**|This field is used to record the Agreed Salary for this placement.|
|**Superannuation**|This field is used to record the Superannuation component of the package for this placement.|
|**Benefits**|This field is used to record if there are any other monetary benefit components of the package for this placement.|
|**Total Package**|This field is populated with the sum of **“Agreed Salary”, “Superannuation” and “Benefits”**.|
|**Placement Fee**|This field is used to record the Placement Fee for this placement.|
|**Fee Rate (%)**|This field is populated when the Placement Fee field is updated for this placement.  The formula of this field is **“Total Package”/”Placement Fee”**.|
|**Perm. Placement Payment Terms**|This field is populated from the Customer Card.|
|**Guarantee Period Days**|This field is used to record the no. of days for Guarantee Period for this placement.|
|**Guarantee Period Expiry**|This field is used to record the expiry date of the Guarantee Period for this placement.|

9.  On the **Salespeople Section** of the **Permanent Placement** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Salesperson Code 1**|This field is used to record the Salesperson for this placement.  Select the Salesperson from the **ArrowDown**.|
|**Name**|This field will populate from the Salesperson record you have selected for this placement.|
|**Initials**|This field will populate from the Salesperson record you have selected for this placement.|
|**E-Mail**|This field will populated from the Salesperson record you have selected for this placement.|
|**Commission**|This field is used to record the percentage value which can be later used to calculate Commission payments for Sales people within your organisation.|
|**Salesperson Code 2.. Salesperson Code 3**|You can record up to 3 Sales people commission payment percentages on this placement.|

10. Once you have completed the relevant information, click **Transfer** icon on the **Home** ribbon.

[GoToTop](#how-to-create-permanent-placements)

## Permanent Placement Cards

Permanent Placements are created once the transactions entered into Placement Entry are transferred.

1.  To access the Permanent Placement Card, go to the following menu: *Departments/Labour Hire/Candidate Processing/Permanent Placements* 

2.  On the **General** FastTab, it contains the fields described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**No.**|This is the Placement No. which is automatically generated by Dynamics NAV.|
|**Resource No.**|This field is the Resource/Employee No. as entered in Placement Entry.|
|**Resource Name**|This field is the Resource/Employee Name as entered in Placement Entry.|
|**Job Title**|This field is the Job Title as entered in Placement Entry.|
|**Customer No.**|This field is the Customer No. as entered in Placement Entry.|
|**Customer Name**|This field is the Customer Name as entered in Placement Entry.|
|**Customer Contact Name**|This field is the Customer Contact Name as entered in Placement Entry.|
|**Customer Contact Title**|This field is the Customer Contact Title as entered in Placement Entry.|
|**Placement Type**|This field is the Placement Type as entered in Placement Entry.|
|**Job Posting Group**|This field is the Job Posting Group as entered in Placement Entry.|

3.  On the **Permanent Placement** FastTab, it contains the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Salesperson Code**|This is the Salesperson Code as entered in Placement Entry.|
|**Placement No.**|This is the Placement No. as allocated when the records were transferred from Placement Entry.|
|**Salesperson Name**|This is the Salesperson Name as selected in Placement Entry.|
|**Percentage**|This is the Commission % value as entered in Placement Entry.|
|**Amount**|This is the Amount field which is a system calculated field.|
|**E-Mail**|This is the E-Mail address of the Salesperson as selected in Placement Entry.|
|**Initials** |This is the Initials of the Salesperson as selected in Placement Entry.| 

4.  On the **Placement Details** FastTab, it contains the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Creation Date**|This field records the date the Permanent Placement record was created.|
|**Start Date**|This field is the Start Date as entered in Placement Entry.|
|**Candidate Source**|This field is the Candidate Source as entered in Placement Entry.|
|**Agreed Salary**|This field is the Agreed Salary as entered in Placement Entry.|
|**Superannuation**|This field is the Superannuation value as entered in Placement Entry.|
|**Benefits**|This field is the Benefits value as entered in Placement Entry.|
|**Total Package**|This is the Total Package value as calculated within Placement Entry.|
|**Notes**|This field is used to record Notes of the Permanent Placement record.|
|**Guarantee Period Days**|This field is the Guarantee Period Days as entered in Placement Entry.|
|**Guarantee Period Expiry**|This field is the Guarantee Period Expiry date as entered in Placement Entry.|
|**Candidate Source Text**|This field is used to record the Candidate Source Text information relating to the Permanent Placement record.|
|**Perm Placement Type**|This field is used to record the Perm Placement Type information relating to the Permanent Placement record.|

5.  On the **Posting** FastTab, it contains the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Purchase Order No.**|This field is the Purchase Order No. as entered in Placement Entry. |
|**Placement Fee**|This field is the Placement Fee as entered in Placement Entry.|
|**Fee Package Percentage Rate**|This field is the Fee Package Percentage rate as calculated in Placement Entry.|
|**Department Code (Global Dimension 1)**|This field will represent the Global Dimension 1 setup in your Dynamics NAV Company.  This information is populated from the Job Posting Group.|
|**Project Code (Global Dimension 2)**|This field will represent the Global Dimension 2 setup in your Dynamics NAV Company. This information is populated from the Job Posting Group.|

6.  On the **Invoice/Credit** FastTab, it contains the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Date to Generate Invoice**|This field is a calculated field to identify when the invoice should be generated.  This value is determined by other setup within Dynamics NAV.|
|**Invoice Generated**|This field is updated when the Invoice has been generated.|
|**Invoice Generate Date**|This field is updated with the date the Invoice is generated.|
|**Payment Due Date**|This field is calculated based on the Date the Invoice is generated and the Payment Terms code.|
|**Invoice No.**|This field displays the Invoice No.|
|**Invoice Amount**|This field is updated to record the Invoice Amount.|
|**Credit Generated**|This field is updated if a Credit Memo is generated.|
|**Credit Generation Date**|This field is updated with the date the Credit Memo is generated.|
|**Credit Memo No.**|This field displays the Credit Memo No. if one has been generated.|
|**Credit Amount**|This field displays the value of the amount credited.|

[GoToTop](#how-to-create-permanent-placements)

# PERMANENT PLACEMENT INVOICING
Permanent Placement invoices can be generated once the Permanent Placement record has been created.   Various parameters are established to determine when invoices are generated, invoice formats and payment terms if they are different to normal payment terms.

[GoToTop](#how-to-create-permanent-placements)

## Permanent Placement Invoice Parameters

Permanent Placement Invoice parameters are maintained within the following areas of the Labour Hire module:

- Labour Hire Setup – Permanent Placement FastTab
- Customer Card – Invoice Formats - Invoicing FastTab
- Customer Card – Payment Terms - Payments FastTab

[GoToTop](#how-to-create-permanent-placements)

### Labour Hire Setup – Permanent Placement FastTab

1.  To access the Permanent Placement FastTab on the Labour Hire Setup card, go to the following menu; *Departments/Payroll/Setup/Labour Hire/Administration/Labour Hire Setup* 

2.  On the **Permanent Placement** FastTab, fill in the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**No. Days/Weeks To Calculate Invoice Generation Date**|This field is used to determine the number of days or weeks when Permanent Placement invoices should be generated after the placement.  If Permanent Placement invoices are generated 1 day after the placement date, then you would enter 1.00 in this field.|
|**Days/Weeks**|This field is used to identify whether part of the invoice generation formula is based on Days or Weeks.  If Permanent Placement invoices are generated 1 day after the placement date, then you would select “Days”.|
|**Start/Create Date**|This field is used to identify whether part of the invoice generation formula is based on the placement Start Date or Creation Date.  If Permanent Placement invoices are generated 1 day after the Start date of the placement, then you would select “Start Date”.|
|**Before/After**|This field is used identify whether part of the invoice generation formula is based Before the placement date, or After the placement date.  If Permanent Placement invoices are generated 1 day after the Start date of the placement, then you would select “After”.|
|**Placement Flat Fee Type Code**|This field determines where the revenue for the Permanent Placement Fees will be posted to within the General Leger.  From the **ArrowDown**, select the appropriate code.|
|**Plcmt. Salary % Fee Type Code**|This field determines where the revenue for the Permanent Placement Fees will be posted to within the General Leger.  From the **ArrowDown**, select the appropriate code.|

[GoToTop](#how-to-create-permanent-placements)

### Customer Card – Invoicing FastTab
Permanent Placement invoices will have a specific invoice format to present the information back to the client.  

The Permanent Placement Invoice format is maintained on the **Invoicing** FastTab in the **Perm. Invoice/Cr. Format Code** field.
 

[GoToTop](#how-to-create-permanent-placements)


### Customer Card – Payments FastTab
Permanent Placement invoices may have different payment terms to the general invoicing.  

The Permanent Placement Payment Terms code is maintained on the **Payments** FastTab in the **Perm. Placement Payment Terms** field. 
 
[GoToTop](#how-to-create-permanent-placements)

## Generating Permanent Placement Invoices 

1.  To generate Permanent Placement Invoices, go to the following menu; *Departments/Labour Hire/Invoice Processing/Generate Invoice/ Generate Permanent Invoices* 

2.  On the **Options** FastTab, fill the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**From Date**|This field allows you to specify a date range to allow for the invoices to be generated.|
|**To Date**|This field allows you to specify a date range to allow for the invoices to be generated.|

3.  Click on the **OK** icon, after you have completed your selection.

[GoToTop](#how-to-create-permanent-placements)

# REQUIREMENTS INVOICING OVERVIEW
Requirements invoicing is a term used to describe invoices generated for expenses incurred when positions are advertised prior to candidates being selected.

This feature is only available where integration with third party “front end” systems are established, however Requirement invoices can be manually generated and posted against the appropriate General Ledger account if there is no integration with a front end Recruitment system.

[Fee Types](#fee-types) which allows for the different types of expenses to be posted to the appropriate General Ledger account.

When these types of expenses are created within the Recruitment system, a line item will be created and setup similar to a Permanent Placement record where the fees will be available from within the Job card.

[GoToTop](#how-to-create-permanent-placements)

## Requirements Invoice Setup
Requirements are created as Jobs within the Labour Hire module where 3rd party integration exists.    

1.  To review a Requirements record, go to the following menu: *Departments/Labour Hire/Candidate Processing/Jobs*

2.  On the Job Card window, the **Requirement Fees** icon is accessable via the **Home** ribbon.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Job Task No.**|This field will reflect the Job Task No. as transferred from the front end system.|
|**Fee Type Code**|This field will contain the Fee Type Code as specified within the setup.|
|**Fee Description**|This field will contain a description of the Fee Type Code.|
|**Amount**|This field will contain the amount of the fee.|
|**Ready to Post**|This field will be checked to mark that the invoice is ready to generate.|

[GoToTop](#how-to-create-permanent-placements)

## Requirements Invoice Parameters
Requirement Invoice parameters are maintained within the following areas of the Labour Hire module:

- Interface Options - Integration FastTab
- Customer Card - Invoice Formats - Invoicing FastTab


### Interface Options – Integration FastTab

1.  To access the Integrations FastTab on the Interface Options card, go to the following menu: *Departments/Payroll/Setup/Labour Hire/Interface Integration/Interface Options*

2.  On the **Integration** FastTab, fill in the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Perm. Bill. Expense Code**|This field is used to identify the Fee Type for this type of expense.|
|**Perm. Bill. Shortlist Fee Code**|This field is used to identify the Fee Type for shortlist fees.|
|**Perm. Bill. Retainer Fee Code**|This field is used to identify the Fee Type for the retainer fees.|

[GoToTop](#how-to-create-permanent-placements)

### Customer Card – Invoicing FastTab
Requirements invoices will have a specific invoice format to present the information back to the client.  

The Requirements Invoice format is maintained on the **Invoicing** FastTab in the **“Req. Inv./Cr. Format Code”** field.

[GoToTop](#how-to-create-permanent-placements)

## Generating Requirements Invoices 

1.  Requirements Invoices are generated from the following menu: *Departments/Labour Hire/Invoice Processing/Generate Invoice/ Generate Perm. Req. Invoice* 

2.  On the **Job** FastTab, fill in the fields as described in the following table.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Bill-to Customer No.**|This field allows you to nominate a specific customer you wish to generate invoices for, otherwise this field can be left blank to generate all outstanding Requirements invoices.|

3.  Click on the **OK** button after you have completed your selection. 

[GoToTop](#how-to-create-permanent-placements)
