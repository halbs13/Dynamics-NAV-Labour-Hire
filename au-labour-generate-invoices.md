

# Invoice Processing Overview

Dynamics NAV Labour Hire’s Sales Invoice and Sales CR/Adj Note generation function has been designed to automatically generate invoice for customers using data transferred from the Time Sheet Line table.  The data entered and processed from the Time Sheet Line table will update the Job Planning Lines ready for customer invoices and credit notes to be generated.  

The Invoice and CR/Adj Note Generation function has been designed to cater for the following requirements:
-	Generation Selection: Ability to select which customers to generate invoices for.
-	Invoice Frequency: Generate invoices at different intervals depending on customer    choice.
-	Invoice Consolidation: Different levels of consolidation can be selected for customers.  Examples of consolidation are one invoice for each sell to customer or one invoice for just the bill to customer, which represents a parent or umbrella type company.

These features allow users to set up all of the required parameters at a customer level.  When it comes time to generate invoices, they will simply have to select an option and filter on some choices if required and the invoices and credit notes will automatically be generated correctly for each customer.
The document is designed to specifically discuss the process for generating invoices manually from the job planning lines and using the “Generate Sales Invoice” Option.  For further information relating to Sales Invoice Setup, please refer to “Dialog – Training – LH Invoice Processing Setup” document.

 # Invoice Processing Overview
 
This section will discuss two (2) methods in which invoices can be generated:
-	 Generate Invoice 
-	 Manually generating Invoices from the Customer and Job Cards
	
## Generate Invoice

This function generates both Invoices and CR/Adj Notes.  To generate invoices and CR/Adj notes, go to the following menu:
To generate invoices, go to the following menu:
*Departments/Labour Hire/Invoice Processing/Generate Invoice/Generate Invoice*

##  “Invoice/Credit Generate” window

|**Field Name**|**Description*
|------------------------------------|---------------------------------------------------------------------------------------|
|Posting Date|This date will be used as the “Posting Date on all generated Invoices and Credit Notes and sales records will be posted to the relevant ledger using this date.|
|Generate|From the “Generate” field, select your option. Each customer will have set up with an Invoice
  Frequency, so this should be selected depending on which batch of invoices you are generating.  All customers with a matching frequency will have invoices generated if they have trainings waiting to be invoiced.
  The Adhoc option allows you to generate invoices for all customers regardless of frequency.|
 |**Click on the “Generate” button after you have completed your selection.|
  
 ### “Edit – Sales Invoice/Credit Note Generation Customer FastTab” window
There are a number of filters which you can enter to further filter information:

Field Name
Description
   Customer No.
  
 Select a   “Customer No.” or leave blank for all customers with the same frequency.
  Click the “OK” button.
  
# Generated Invoices

To view generated Invoices, go to the following menu:
Departments/Labour Hire/Invoice Processing/Lists/Sales Invoice
A list of all the sales invoices generated will appear from which you can select to view each invoice individually.  Alternatively you can post the batch of invoices by selecting the “Post Batch” or post individually by nominating the “Post” button.
To check invoices individually, double-click on a Sales Invoice and the “Edit – Sales Invoice” window will appear.

## “Edit – Sales Invoice” window

The “Sales Invoice” contains the following tabs and information:

 Field Name
 Description
   GENERAL FASTTAB – The General FastTab contains
  information such as Invoice No., Customer Contact, Salesperson and Address
  information
    Posting Date
  
  
  This is the Posting Date entered used to generate the invoice
  
  Document Date
  
  This is the date the invoice is generated and is used to determine the “Due Date” on the invoice
    
  External Document No.
  
  
  This will be left blank but can be used as a reference number for the customer
  
 

  Invoice/Cr. Memo Format Code  This is the Sales Invoice Format code sourced from the Customer Card
  
  LINES FASTTAB – The Lines FastTab contains the
  invoice lines generated from the Job Planning Lines
 
  Type
  
  This will default to “Resource”  No This is the “Resource No.”
  
  Description
 This field will populate from the Pay
 Transaction Type code as a description
    Quantity
    This field will contain the quantity or number of hours
  Unit of Measure Code
  This field contains the Unit of Measure Code 
  
  Unit Price Excl. GST
  This field contains the “Charge Rate” 
  Line Amount Excl. GST  
  This field contains the Line Amount (Quantity *
  “Unit Price Excl. GST)
  INVOICING FASTTAB – The Invoicing FastTab
  contains information of where the invoice will be sent to
  Invoice Type
  This option will default to “Times”
  Payment Terms Code  
  The Payment Terms code will be sourced from the
  Customer Card 
  Due Date 
  This field is populated calculated from the
  “Document Date” 
  Payment Method Code
  
  The Payment Method code will be sourced from the Customer Card
  
 GST Bus. Posting Group
   The GST Bus. Posting Group will be sourced from the Customer Card
  
 
## Printing a Test Report 

You can print a test report to preview invoice information prior to posting the invoice. 
To print a Test Report from the Sales Invoice,
Click on the “Actions ribbon> Posting> Test Report”.

If the report indicates any errors or lack of information, you can correct the problem and then reprint the test report again before posting the invoice.

## Posting the Invoice 

The Invoice lines have been generated from the information that is processed from the Timesheets.  If there are any adjustments to be made, then adjusting timesheet entries should be made rather than making adjustment to the invoice lines.  The system will however permit adjustment to entries directly on an invoice line prior to posting.
Invoices can be checked via the Test Report and should be posted once checking is complete.  
If the posting routine finds any errors while posting, the process will be interrupted by an error message and can be restarted once the error has been rectified.
To post the invoice from within the Sales Invoice, Click on “Post” or “Post and Print” buttons.

## Post Button

Click on the “Post” button if you want to post the invoices individually without printing the Sales Invoice.
Once you select this option, a response window will appear “Do you want to post the Invoice?”.  Select “Yes” to post the invoice.
Upon completion, the “Posted Invoice List” will print.

### Post and Print Button

Click on the “Post and Print” button if you want to post the invoices individually.
Once you select this option, a response window will appear “Do you want to post and print the Invoice?” .Select “Yes” to post and print the invoice.
Upon completion, the “Sales Invoice” and “Posted Invoice List” will print.

### Post Batch

Click on the “Post Batch” button if you want to post a batch of invoices.
Once you select this option, the “Edit – Batch Post Sales Invoices” window will appear:


Field Name 
 Description
   OPTIONS FASTTAB 
  Posting Date
  Enter in a Posting Date if you wish to override
  the Posting Date used to generate the invoice, otherwise leave this blank.
  Replace Posting Date
  Tick this field if you wish to replace the
  Posting Date on the invoices generated. 
    Replace Document Date
  Tick this field if you wish to replace the
  Document Date on the invoices generated.
    SALES INVOICE FASTTAB – This is where you can
  enter in additional filters to select the sales invoices you wish to post
 No.
  Enter in the Invoice No. range you wish to
  post.  ** Note – you may have to make
  note of this prior to selection
    Click “OK” once you have
  completed your selection.
  
Upon completion, the “Posted Invoice List” window will appear where you can print, preview or cancel the report.  

## Reviewing Posted Invoices 

Once invoices are posted they can be accessed from within the following areas:
-	Using the Navigation function from within the Customer Ledger Entries on the Customer Card
-	From the Posted Invoices Menu

### Using the Navigation Function from Customer Ledger Entries

You can preview posted invoices from within the Customer Ledger Entries area of the Customer card.
First go to the Customer Card by accessing the following menu:
Departments/Labour Hire/Candidate Processing/Customers 
-	  Select the Customer record from the Customer List by searching and clicking on the record.
-	  Once you have selected your customer record, click on the “Navigate ribbon/Ledger Entries”       and select the invoice you wish to preview.
-	  Click on the “Navigate” Button and select “Posted Sales Invoice”
-	  If you wish to Preview the record click on “Show Posted Document”. 
 
### Posted Invoices

You can preview posted invoices from within the
Posted Invoices area.  You can access the Posted Invoices from:
Departments/Labour Hire/Invoice Processing/Lists/Posted Invoices
-	  Select the Invoice No. by searching and clicking on the record,
.  -       Click on “Print”. 

## Emailing Invoices

Within Dynamics NAV you have the ability to email invoices to customers.  The “E-Mail
Invoice/Cr. Memo” flag must be set and “Invoice Customer E-Mail List” must be updated.  
To email the invoice, go to the following menu:
*Departments/Labour Hire/Invoice Processing/Tasks/E-Mail Invoice List*


### “Edit – E-Mail Invoice List” window

 Field Name
  Description 
OPTIONS FASTTAB
  
  Message 
   You can enter in a message to print out on the invoice.
  **Note: you must have a “Message” section on your invoice for this information to print.
  SALES INVOICE HEADER FASTTAB
  Sell-to Customer No.
   From the ArrowDown button, select or enter in the Customer No. you wish to email to
  No. From the ArrowDown button, select or enter in the Invoice No. you wish to 
  You can also enter in other filters as necessary, otherwise click on the “OK” after you have completed your selection.
  
 ## Generating Manual Invoices
 
Invoices can be generated manually either from the Customer Card or directly from the Job Planning lines, however the automated generation invoice process is recommended as it will contain relevant job information which may be overlooked if information is manually entered.

### Customer Card

You can create a manual invoice directly from the Customer card.  First go to the Customer
Card by accessing the following menu:
*Departments/Labour Hire/Candidate Processing/Customers*

-	 Select the Customer record from the Customer List by searching and clicking on the record. 
-	 Once you have selected your customer record, click on the “Sales Invoice” button to create a blank invoice and click “Enter” Customer Card.  The Posting and Document Date will default from today’s date.
-	In the “Lines” Tab complete the following information at a minimum.
 Field Name
  Description
   
LINES FASTTAB
 Type
  If you are producing a manual invoice for a contractor, select from the options “Resource”
  No.
  If you have selected “Resource” as the Type, in this field you will be able to select the appropriate Contractor Number from  the Lookup button.
  
 Description
  Enter in the Description which will appear in the Invoice Description.  This will default to the Resources Name but can be overwritten
  Quantity
  Enter in the number of units/hours Unit of Measure Code
 This information will default from the Resource Card
  GST Prod Posting Group This information will default from the Resource Card
  Unit Price Excl. GST Enter in the Charge Rate
-	  Continue to enter in lines using the abovementioned steps, otherwise click on the ‘Post” or “Post and Print” button to print the invoice. 

### Job Card

You can create a manual invoice directly from the Job card.  First go to the Job Card by accessing the following menu:
Departments/Labour Hire/Candidate Processing/Jobs

-	 Select the Job record from the Job List by searching and clicking on the record. 
-	 Once you have selected your job record, click on the Home ribbon, and “Create Job Sales   Invoice” button to create an invoice 	 for the Job. 
   -     In the “Edit – Job Create Sales Invoice” window complete the following information.
 Field Name
   Description
   OPTIONS FASTTAB
   Posting Date The date will default to today’s date but can be changed where applicable.
  Create Invoice Per         You can nominate to create the invoice by Job or Job Task 
    JOB TASK FASTTAB
   Job No.          If you wish to create an invoice by Job No., enter or select the Job No. from the ArrowDown button.
Job Task No.       If you wish to create an invoice for a particular Job Task No. of a Job, enter in the Job Task No. by clicking on the ArrowDown button.
 You can also enter in other filters as necessary
-	 When completed, click “OK”.  If there are no invoice lines to generate then a message will    appear “There is nothing to invoice”, otherwise you will receive a message “1 invoice is created”.
-	 To review the Job created invoice, go to the following menu: 
Departments/Labour Hire/Invoice Processing/Lists/Sales Invoice
-	  To finalise and post the invoice refer to 2.4 – Posting the Invoice

# Sales CR/Adj Notes Processing Overview

This section will discuss two (2) methods in which Sales CR/Adj Notes can be generated:
-	  Generate Invoice 
-	  Manually generating CR/Adj   notes 

## Generate Invoice

This function generates both Invoices and CR/Adj Notes.  To generate invoices and CR/Adj notes, go to the following menu:

*Departments/Labour Hire/Invoice Processing/Generate Invoice/Generate Invoice*

### “Invoice/Credit Generate” window

   Field Name
  
  Description
   Posting Date 
 Fill in the “Posting Date” field with the posting date.  
  This date will be used as the “Posting Date on all generated Invoices and Credit Notes and sales records will be posted to the relevant ledger using this date.
    Generate
  From the “Generate” field, select your option.
  Each customer will have set up with an Invoice
  Frequency, so this should be selected depending on which batch of invoices
  you are generating.  All customers with
  a matching frequency will have invoices generated if they have trainings
  waiting to be invoiced.
  The Adhoc option allows you to generate
  invoices for all customers regardless of frequency.
    Click on the “Generate” button after you have completed your selection.
  
### "Edit – Sales Invoice/Credit Note Generation Customer FastTab” window

 There are a number of filters which you can enter to further filter information:
Field Name
   Description
   Customer No.
  Select a   “Customer No.” or leave blank for all customers with the same frequency.
  Click the “OK” button.
 
## Generated Sales CR/Adj Notes

To view generated Sales CR/Adj Notes, go to the following menu:
*Departments/Labour Hire/Invoice Processing/Lists/Sales CR/Adj Notes*

A list of all the sales CR/Adj notes generated will appear from which you can select to view each CR/Adj note individually.  
To check CR/Adj notes, double-click on a Sales CR/Adj and the “Edit – Sales Invoice” window will appear.

### “Edit – Sales CR/Adj Note” window

The “Sales CR/Adj Note” contains the following tabs and information:

Field Name
   Description
   
  GENERAL FASTTAB – The General FastTab contains   information such as CR/Adj Note No., Customer Contact, Salesperson and Address information
  Posting Date       This is the Posting Date entered used to generate the invoice
   Document Date
  This is the date the invoice is generated and is used to determine the “Due Date” on the invoice
  External Document No.
  This will be left blank but can be used as a reference number for the customer
  
  Invoice/Cr. Memo Format Code
    This is the Sales CR/Adj Note Format code sourced from the Customer Card
  
 LINES FASTTAB – The Lines FastTab contains the
  invoice lines generated from the Job Planning Lines
  
 Type  This will default to “Resource”
   No.
   This is the “Resource No.”
    Description
    This field will populate from the Pay Transaction Type code as a description
   Quantity   This field will contain the quantity or number of hours
  
Unit of Measure Code   This field contains the Unit of Measure Code 
  
Unit Price Excl. GST  This field contains the “Charge Rate” 
  
  Line Amount Excl. GST    This field contains the Line Amount (Quantity *   “Unit Price Excl. GST)
  
 INVOICING FASTTAB – The Invoicing FastTab contains information of where the CR/Adj Note will be send to
  Invoice Type  This option will default to “Times”
  Payment Terms Code  The Payment Terms code will be sourced from the
  Customer Card  Due Date This field is populated calculated from the “Document Date”   
Payment Method Code The Payment Method code will be sourced from  the Customer Card
  GST Bus. Posting Group  The GST Bus. Posting Group will be sourced from the Customer Card
 APPLICATION FASTTAB – The Application FastTab  contains information of the invoice the CR/Adj Note will be applied against
  
Applies to Doc. Type This option will default to “Invoice” if it has  been applied the time of entering the adjustment via Timesheet Entry
  
ADJUSTMENT DETAILS FASTTAB – The Adjustment Details FastTab contains information adjustment details and the reason why  the CR/Adj Note has been created
  
Adjustment This field will be automatically flagged the highlight the CR/Adj Note will be applied as an adjustment
  
BAS Adjustment This field will automatically be flagged the highlight the CR/Adj Note will be applied as a BAS adjustment
    Adjustment Applies-to  This field will contain the sales invoice noy the CR/Adj Note will be applied to if entered via Timesheet Entry
    Reason Code This field will only be completed if a “Reason Code” has been filled in the Labour Hire Setup.    If this field is blank, click on the “ArrowDown” and select the reason why the CR/Adj Note
  is being generated
         
## Printing a Test Report 

You can print a test report to preview CR/Adj Note information prior to posting the CR/Adj Note. 
To print a Test Report from the Sales CR/Adj Note click on the “Actions Button>Posting>Test Report”.
If the report indicates any errors or lack of information, you can correct the problem and then reprint the test report again before posting the CR/Adj Note.

## Posting the CR/Adj Note

The CR/Adj Note lines have been generated from the information that is processed from the Timesheets.  If there are any adjustments to be made, then adjusting timesheet entries should be made rather than making adjustment to the CR/Adj Note lines.  The system will however permit adjustment to entries directly on an CR/Adj Note line prior to posting.

If the posting routine finds any errors while posting, the process will be interrupted by an error message and can be restarted once the error has been rectified.

To post the CR/Adj Note from within the Sales CR/Adj Note, Click on “Post”  or “Post and Print” buttons.

### Post Button

Click on the “Post” button to post the CR/Adj Notes. Once you select this option, a response window
will appear  “Do you want to post the CR/Adj Note?”.  Select “Yes” to post the CR/Adj Note.

### Post and Print Button

Click on the “Post and Print” button if you want to post the invoices individually.
Once you select this option, a response window will appear “Do you want to post and print the CR/Adj Note?”.  Select “Yes” to post and print the CR/Adj note.
Upon completion, the “Sales CR/Adj Note” will print.

## Reviewing Posted CR/Adj Notes

Once CR/Adj notes are posted they can be accessed from within the following areas:
-	Using the  Navigation function from within the Customer Ledger Entries on the Customer Card
-	From the Posted CR/Adj Notes Menu
 
### Using the Navigation Function from Customer Ledger Entries

You can preview posted invoices from within the Customer Ledger Entries area of the Customer card.
First go to the Customer Card by accessing the following menu:
Departments/Labour Hire/Candidate Processing/Customers
-	Select the Customer record from the Customer List by searching and clicking on the record.
-	Once you have selected your customer record, click on the “Navigate ribbon” and select “Ledger Entries” and select the CR/Adj note you wish to preview.
-	Click on the “Navigate” Button and select “Posted Sales CR/Adj Note”
-	If you wish to Preview the record click on “Show”, otherwise click on “Print”. 

### Posted CR/Adj Notes

You can preview posted CR/Adj notes from within the Posted CR/Adj Notes area.  You can access the Posted CR/Adj Notes from:
Departments/Labour Hire/Invoice Processing/Lists/Posted CR/Adj Notes
-	Select the CR/Adj No. by searching and clicking on the record.
-	Click on “Print”. 
-	
## Generating Manual CR/Adj Notes 

here are a number of ways to create a CR/Adj note within Dynamics NAV.  This section will discuss manually creating CR/Adj notes from the Sales CR/Adj areas using the Copy Document function.  

### Sales CR/Adj Notes

You can create a manual CR/Adj note from the Sales CR/Adj Notes menu.  
Departments/Labour Hire/Invoice Processing/Lists/Sales CR/Adj Notes

-	Click on the “New” button and click “Enter” to create a new CR/Adj note.   When you click “Enter” the information on the         “General” Tab will populate the Posting and Document Date with today’s date.
-	Click on the ArrowDown button in the “Sell-to Customer No.” field and select the Customer No. you wish to create a CR/Adj note for and then click “Enter”.  When you click “Enter” the information on the “General” Tab will populate with various information from the Customer Card.
-	 If you are crediting an invoice which has been posted to the Customer Ledger entry, you can use the “Copy Document” function to retrieve the previously posted lines.  To do this, click on the “Copy Document” button.  
-	The “Edit – Copy Sales Document” window will open.  It should be updated as follows:  


 
  
   
   Field Name
   Description
   OPTIONS FASTTAB
  Document Type
  You can select the information to be copied from an invoice which has not yet been posted or from the posted invoice.  From the ArrowDown button, click on “Invoice” or “Posted Invoice”
    Document No.    From the ArrowDown button, you can nominate which Invoice or Posted Invoice you wish to copy the information from.   Once you have made your selection, click on “OK”.
  Sell-to Customer No. This is a non-editable field and will default from the record information you have selected.
   Sell-to Customer Name  This is a non-editable field and will default  from the record information you have selected.
    Include Header This will be automatically ticked and will include the header information from the record you have selected.
    Recalculate Lines  If you wish to have the lines recalculated then you can tick this field, otherwise leave it blank.
   Posting Date If the CR/Adj note is to have a new Posting Date, then enter in the new posting date into this field.
  Replace Posting Date  If you enter in a new Posting Date, this field will automatically be ticked.  
    Replace Document Date If you enter in a new Posting Date, this field will automatically be ticked.  
  Click the “OK”  button.
   If you changed the Posting Date as part of your selection, you will receive the following message:
   “You have changed Posting Date on the sales header, but it has not been changed on the existing sales lines.  The change may affect the exchange rate used in the price calculation of the sales lines.”  
  Click “OK” to continue.  

The CR/Adj note and lines will be populated with various information from the sales invoice or document you selected in the Copy Document process.  The following information will have been generated from a Contractor invoice. 

|**Field Name**|**Description**|
|--------------------------------------|----------------------------------------------------------------------------------------|
||**GENERAL FASTTAB – The General FastTab contains information such as CR/Adj Note No., Customer Contact, Salesperson and Address information generated from the Copy Document Process**| 
|**Posting Date**|This is the Posting Date entered used to generate the CR/Adj note from the Copy Document process|
|Document Date|This is the Document Date entered used to generate the CR/Adj note from the Copy Document process
|**External Document**No.|This will be left blank but can be used as reference number for the customer>
|**Invoice/Cr. Memo Format Code**|This is the Sales CR/Adj Note Format code  sourced from the Customer Card|
  
  LINES FASTTAB – The Lines FastTab contains the  invoice lines generated from the document nominated in the Copy Document Process
  Type.   This will default to “Resource”
   No. This is the “Resource No.”
   Description This field will populate from the Pay  Transaction Type code as a description
    Quantity This field will contain the quantity or number of hours
 Unit of Measure Code  This field contains the Unit of Measure Code 
  Unit Price Excl. GST This field contains the “Charge Rate” 
   Line Amount Excl. GST  This field contains the Line Amount (Quantity *
  “Unit Price Excl. GST)
  INVOICING FASTTAB – The Invoicing FastTab contains information of where the CR/Adj Note will be send to Invoice Type  This option will default to “Times”
  Payment Terms Code The Payment Terms code will be sourced from the Customer Card
   Due Date This field is populated calculated from the  “Document Date” 
   Payment Method Code The Payment Method code will be sourced from  the Customer Card
  GST Bus. Posting Group The GST Bus. Posting Group will be sourced from the Customer Card
  APPLICATION FASTTAB – The Application FastTab contains information of the invoice the CR/Adj Note will be applied against
  Applies to Doc. Type  This option will default to “Invoice” 
  Applies-to Doc. No.  This will default from the Invoice No. selected   from the Copy Document Process
    ADJUSTMENT DETAILS FASTTAB – The Adjustment Details FastTab contains information adjustment details and the reason why  the CR/Adj Note has been created
    Adjustment  This field will be automatically flagged to highlight the CR/Adj Note will be applied as an adjustment
 Adjustment Applies-to This field will contain the sales invoice no.  the CR/Adj Note will be applied to selected from the Copy Document Process
   Reason Code Select the reason from the “ArrowDown” why the CR/Adj Note is being generated
  To finalise and post the CR/Adj note refer to 3.4 - Posting the CR/Adj Note



































