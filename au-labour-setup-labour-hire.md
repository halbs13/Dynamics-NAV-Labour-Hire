# How to setup Labour Hire

2.1	Labour Hire Setup
You use the Labour Hire Setup to establish certain basic rules to be used in the Labour Hire application area.  
To access the Labour Hire Setup, go to the following menu:
Departments/Payroll/Setup/Labour Hire/Administration/Labour Hire Setup
 
2.1.1	“Edit – Labour Hire Setup” window

Field Name	Description
GENERAL FASTTAB 
Job Contract Posting Method	This option defines when invoices can be generated once timesheets are processed. 
The options available are;
•	Payroll – if this option is selected then sales invoices will be available for generation once Payroll has been processed and posted.
•	Timesheet – if this option is selected then sales invoices will be available for generation once Timesheets have processed to payroll. 
Placement No.s	The Placement No.s are used to allocate Placement No.s when using the Placement Entry screen.
Select the Placement No.s from the “ArrowDown”.   
This option is not used if there is integration to Axiom.
Use Interface	The “Use Interface” field if selected, can be used to restrict fields being updated in various tables within NAV as defined in the Interface Options table.
PERMANENT PLACEMENT FASTTAB 
No. Days/Weeks To Calculate Invoice Generation Date	The “No. Days/Weeks To Calculate Invoice Generation Date” field is used to define when Permanent Placement invoices are to be generated.
Days/Weeks	The “Days/Weeks” field is used to define if Permanent Placement invoices are generated days or weeks after the Permanent Placement.
Start/Create Date	The “Start/Create Date” field is used to define if Permanent Placement invoices are generated from the Start Date or Creation Date of the Permanent Placement.
Before/After	The “Before/After” field is used to define if Permanent Placement invoices are generated Before or After the date of the Permanent Placement. 
Placement Flat Fee Type Code	The “Placement Flat Fee Type Code” field is used to define the GL account the Placement Flat Fees will be posted to.
Plcmt. Salary % Fee Type Code	The “Plcmt. Salary % Fee Type Code” field is used to define the GL account the Placement Salary % Fee will be posted to. 
TIMESHEET FASTTAB
Automatic Timesheet Line	The “Automatic Timesheet Line” check box is used to define if timesheets are automatically generated when payrolls are posted and pay periods are closed.
Timesheet Unit Validation	The Timesheet Unit Validation feature is used to define the number of hours worked on a daily basis.  It is generally used for reporting to clients or for internal reasons that allows your organisation to record the number of hours an employee works on a daily basis.
The “Timesheet Unit Validation” check box is used to define if timesheet unit validation is required. 
Dup. Timesheet Check Frequency	The “Dup. Timesheet Check Frequency” defines the frequency of when duplicate timesheets are checked.
The options available are; Weekly or Daily.
Duplicate timesheets are checked based on the following;
•	Alternate Date or Pay Period End Date
•	Transaction Type
INVOICING FASTTAB
Default Job Invoice Grouping	The “Default Job Invoice Grouping” field is used to define how invoices will be generated.  The options available are;
•	Blank 
•	Alternate Date – if you select this option then invoices will be grouped by Alternate Date when generated.
•	Job Posting Group – if you select this option then invoices will be grouped by Job Posting Group when generated. 
•	Job Bill-To Contact – if you select this option then invoices will be grouped by Job Bill-To Contact when generated. 
•	Job No. – if you select this option then invoices will be grouped by Job No. when generated.
•	Job Task No. – if you select this option then invoices will be grouped by Job Task No. when generated.
Click “OK” after you have completed your selection.

2.2	Rate Frequency Conversion
The Rate Frequency Conversion window is used to establish one or more different type of rate frequencies used on Order Rate Sets. 
The Rate Frequency Conversion factors are generally used when Placement Entry is being used.  

To access the Rate Frequency Conversions, go to the following menu:
Departments/Payroll/Setup/Labour Hire/Administration/Rate Frequency Conversion
 
2.2.1	“Edit – Rate Frequency Conversion” window
Field Name	Description
To create a new record, click on the “New” button.
Frequency	Select the “Frequency” type from the “ArrowDown”.  The options available are;
•	Hour
•	Day
•	Week
•	Month
•	Unit
Hourly Conversion Rate	Enter in the value to convert the hourly rate.
Maximum	Enter in the maximum number of units.
Unit of Measure Code	 Select the “Unit of Measure Code” from the “ArrowDown”.
Click “OK” after you have completed your selection.

2.3	Fee Types
The Fee Types window is used to establish the Fee Types that are used within your organisation.  An example of how this might be used is where you have Permanent Placement Fee overhead charges such as setup fees which can be mapped through to a relevant General Ledger account.
To access the Fee Types, go to the following menu:
Departments/Payroll/Setup/Labour Hire/Administration/Fee Types
 

2.3.1	“Edit – Fee Types” window
Field Name	Description
To create a new record, click on the “New” button.
Code	Select the “Fee Type” Code from the “ArrowDown”.
Description	Enter in a Description to describe the Fee Type.
Fee Type	Enter in the Fee Type.  The options available are;
•	Placement
•	Requirement
G/L Account No.	Enter in the GL account number where the placement fee type value will post to in the General Ledger.
Click “OK” after you have completed your selection.
	
2.4	Placement Types
The Placement Types window is used to set up codes for each set of Placement Types you process within your organisation.
To access the Placement Type, go to the following menu:
Departments/Payroll/Setup/Labour Hire/Administration/Placement Type
 
2.4.1	“Edit – Placement Types” window
Field Name	Description
To create a new record, click on the “New” button.
Code	Enter in a Placement Type. You can enter a maximum of 10 characters, both numbers and letters.
Description	Enter in the text that describes the Placement Type.
Placement Category	Enter in the Placement Category which describes the Placement Type.  The options available are;
•	Permanent 
•	Contractor
Exclude from Integration	The “Exclude from Integration” field is used to identify whether this transaction will be excluded from the integration to Axiom.
Click “OK” after you have completed your selection.


2.5	Interface Options
The Interface Options window is used to specify the integration behavior between NAV and Axiom and NAV and TimeKeeper.
To access the Interface Options, go to the following menu:
Departments/Payroll/Setup/Labour Hire/Administration/Interface Options
 
2.5.1	“Edit – Interface Options Card” window
Field Name	Description
Integration Server	The “Integration Server” field is used to establish the Server Name where Axiom resides.
Integration Database	The “Integration Database” field is used to establish the Database Location of the Axiom database.  
This is to allow for mapping through to Live and Test environments.
Default Integration Company	The “Default Integration Company” field if selected identifies that this is the default Integration company.  This will identify that the integration settings for the current NAV company as the global setting in multi-company interface integration.
Include Company in Integration	The “Include Company in Integration” field if selected identifies that this current NAV company is included in the interface integration.
Timekeeper	The “Timekeeper” field if selected is used to extract Timekeeper specific fields.
Order Invoice Address	The “Order Invoice Address” field if selected will use the Customer’s Physical address as the Mailing address.
Transfer Order with Placement	The “Transfer Order with Placement” field if selected will extract the related Order, Requirement, Rate Set and Customer with the Placement when it is created.
Requirement Category	The “Requirement Category” field if selected will extract the Requirement categories and share them in the integration.
Long Description	The “Long Description” field if selected will extract the Long Description stored against the Requirement from Axiom.
Permanent Placement	The “Permanent Placement” field if selected will create Permanent Placements from Job Tasks where applicable.
Salesperson	The “Salesperson” field if selected will extract the Salesperson for the Placements from Axiom.
Rate Set Award Classification	The “Rate Set Award Classification” field if selected will extract the Award & Classifications for the Order Rate Sets in Axiom.
Inc. Comp. Name with Division	The “Inc. Comp. Name with Division” field if selected will prefix the Division name with the NAV Company Name field in Axiom. 
Site Address	The “Site Address” field if selected will extract the Site Address from the Worksite or Long Description fields from within Axiom.
Employee	The “Employee” field if selected will validate the Employee when information is extracted from Axiom.
Payroll Employee	The “Payroll Employee” field if selected will validate the Payroll Employee No. when information is extracted from Axiom.
Prospective Customer Category	The “Prospective Customer Category” field if updated will extract all Orders for customers who have changed to a Client Category.  
Perm. Bill. Expense Code	The “Perm. Bill. Expense Code” field is used to identify the Expense Code for billing purposes.  The Expense code will have been previously mapped through to a relevant GL account. 
Perm. Bill Shortlist Fee Code	The “Perm. Bill Shortlist Fee Code” field is used to identify the Shortlist Fee Code for billing purposes.  The Shortlist Fee code will have been previously mapped through to a relevant GL account.
Perm. Bill. Retainer Fee Code	The “Perm. Bill. Retainer Fee Code” field is used to identify the Retainer Fee Code for billing purposes.  The Retainer Fee code will have been previously mapped through to a relevant GL account.
INTERFACE FASTTAB
Prefix Jobs with O/R	The “Prefix Jobs with O/R” field is used to prefix Jobs and Job Tasks with on “O” or “R” depending on whether it is an Order or Requirement.
Update Employee Payroll No.	The “Update Employee Payroll No.” field if selected will update the Employee’s Payroll No. for existing records
Res. Dims from Job Posting Group	The “Res. Dims from Job Posting Group” field if selected will populate the Resource Dimensions based on the setup of the Job Posting Group.
Job Dims from Job Posting Group	The “Job. Dims from Job Posting Group” field if selected will populate the Job Dimensions based on the setup of the Job Posting Group.
Emp. Dims from Job Posting Group	The “Emp. Dims from Job Posting Group” field if selected will populate the Employee Dimensions based on the setup of the Job Posting Group.
Pay Emp Dims from Job Posting Group	The “Pay Emp Dims from Job Posting Group” field if selected will populate the Payroll Employee Dimensions based on the setup of the Job Posting Group.
Perm Place Dims from Job Posting Group	The “Perm Place Dims from Job Posting Group” field if selected will populate the Permanent Placement Dimensions based on the setup of the Job Posting Group.
Transfer Customer Contact	The “Transfer Customer Contact” field if selected creates a Customer Contact for the Customer.
Default Cust Inv Consolidation	The “Default Cust Inv Consolidation” field will identify the default setting of the Invoice Consolidation for the Customer.
The options available are;
•	Bill-To Customer No. + Sell-To Customer No. – if this option is selected then the invoices will be generated based on the Sell-To Customer details
•	Bill-To Customer No. – if this option is selected then the invoices will be generated based on the Bill-To Customer details.  This option allows you to map associated customers to one main customer for invoicing.
Click “OK” after you have completed your selection.

2.6	Interface Defaults
The Interface Defaults window is used to define the behavior of integrated fields from Axiom/Placement Entry into NAV.  
To access the Interface Defaults, go to the following menu:
Departments/Payroll/Setup/Labour Hire/Administration/Interface Defaults
 
2.6.1	“Edit – Interface Defaults” window
Field Name	Description
To create a new record, click on the “New” button.
Table No.	From the “ArrowDown” select the Table No. of the table to be included in the interface.
Table Name	The “Table Name” field will display the name of the Table selected in the Table No. field.
Field No.	From the “ArrowDown” select the Field No. of the table to be included in the interface.
Field Name	The “Field Name” field will display the name of the Field selected in the Table No. field.
Field Type	The “Field Type” field will display what type of field it is that you have selected.
Field Length	The “Field Length” will display the length of the field that you have selected.
Maintain By The Interface	The “Maintain By The Interface” field if selected will be maintained by the interface.
Not a Default	The “Not A Default” field if selected no default will be assigned.  
Default Value Text	The “Default Value Text” field is used when the “Not A Default” field is set to True.
Default Value Code	The “Default Value Code” field is used when the “Not A Default” field is set to True.
Default Value Boolean	The “Default Value Boolean” field is used when the “Not A Default” field is set to True.
Default Value Decimal	The “Default Value Decimal” field is used when the “Not A Default” field is set to True.
Default Value Integer	The “Default Value Integer” field is used when the “Not A Default” field is set to True.
Default Value Date	The “Default Value Date” field is used when the “Not A Default” field is set to True.
Default Value Time	The “Default Value Time” field is used when the “Not A Default” field is set to True.
Click “OK” after you have completed your selection.
	
2.6.2		Interface Defaults Setup Recommendation

The attached spreadsheet contains a recommended setup to use to import into a newly created database.  It will require testing to confirm that the defaults have been setup according to the requirements of your organisation.

 
