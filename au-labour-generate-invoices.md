

# Invoice Processing Overview

Dynamics NAV Labour Hire’s  Sales Invoice and Sales CR/Adj Note generation function has been designed to automatically generate invoice  for customers using data transferred from the Time Sheet Line table.  The data entered and processed from the Time Sheet Line table will update the Job Planning Lines ready for customer invoices and credit notes to be generated.  

The Invoice and CR/Adj Note Generation function has been designed to cater for the following requirements:

   -   Generation Selection: Ability to select which customers to generate invoices for.

   -   Invoice Frequency: Generate invoices at different intervals depending on customer choice.

   -   Invoice Consolidation: Different levels of consolidation can be selected for customers.  Examples of consolidation are one              invoice for each sell to customer or one invoice for just the bill to customer, which represents a parent or umbrella type              company.

These features allow users to set up all of the required parameters at a customer level.  When it comes time to generate invoices, they will simply have to select an option and filter on some choices if required and the invoices and credit notes will automatically be generated correctly for each customer.

The document is designed to specifically discuss the process for generating invoices manually from the job planning lines and using the “Generate Sales Invoice” Option.  For further information relating to Sales Invoice Setup, please refer to “Dialog – Training – LH Invoice Processing Setup” document.

.

#	INVOICE PROCESSING OVERVIEW
This section will discuss two (2) methods in which invoices can be generated:

   -    Generate Invoice 
   -    Manually generating Invoices from the Customer and Job Cards

##	Generate Invoice
This function generates both Invoices and CR/Adj Notes.  To generate invoices and CR/Adj notes, go to the following menu:

To generate invoices, go to the following menu:

Departments/Labour Hire/Invoice Processing/Generate Invoice/ Generate Invoice
 
###	“Invoice/Credit Generate” window

INSERT TABLE


 
###	“Edit – Sales Invoice/Credit Note Generation Customer FastTab” window
There are a number of filters which you can enter to further filter information:

INSERT FIELD

##	Generated Invoices
To view generated Invoices, go to the following menu:

Departments/Labour Hire/Invoice Processing/Lists/Sales Invoice

A list of all the sales invoices generated will appear from which you can select to view each invoice individually.  Alternatively you can post the batch of invoices by selecting the “Post Batch” or post individually by nominating the “Post” button.

To check invoices individually, double-click on a Sales Invoice and the “Edit – Sales Invoice” window will appear.
 
### “Edit – Sales Invoice” window
The “Sales Invoice” contains the following tabs and information:

INSERT FIELD


##	Printing a Test Report 
You can print a test report to preview invoice information prior to posting the invoice. 

To print a Test Report from the Sales Invoice, click on the “Actions ribbon> Posting> Test Report”.

If the report indicates any errors or lack of information, you can correct the problem and then reprint the test report again before posting the invoice.
 

##	Posting the Invoice 
The Invoice lines have been generated from the information that is processed from the Timesheets.  If there are any adjustments to be made, then adjusting timesheet entries should be made rather than making adjustment to the invoice lines.  The system will however permit adjustment to entries directly on an invoice line prior to posting.

Invoices can be checked via the Test Report and should be posted once checking is complete.  

If the posting routine finds any errors while posting, the process will be interrupted by an error message and can be restarted once the error has been rectified.

To post the invoice from within the Sales Invoice, Click on “Post”  or “Post and Print” buttons.

###	Post Button
Click on the “Post” button if you want to post the invoices individually without printing the Sales Invoice.

Once you select this option, a response window will appear “Do you want to post the Invoice?”.  Select “Yes” to post the invoice.
Upon completion, the “Posted Invoice List” will print.
 
###	Post and Print Button
Click on the “Post and Print” button if you want to post the invoices individually.
Once you select this option, a response window will appear “Do you want to post and print the Invoice?”.  Select “Yes” to post and print the invoice.

Upon completion, the “Sales Invoice” and “Posted Invoice List” will print.
 
###	Post Batch
Click on the “Post Batch” button if you want to post a batch of invoices.
 
Once you select this option, the “Edit – Batch Post Sales Invoices” window will appear:
 
INSERT TABLE

Upon completion, the “Posted Invoice List” window will appear where you can print, preview or cancel the report.  

##	Reviewing Posted Invoices 
Once invoices are posted they can be accessed from within the following areas:

   -   Using the Navigation function from within the Customer Ledger Entries on the Customer Card
   
   -   From the Posted Invoices Menu
   
###	Using the Navigation Function from Customer Ledger Entries
You can preview posted invoices from within the Customer Ledger Entries area of the Customer card.

First go to the Customer Card by accessing the following menu:

Departments/Labour Hire/Candidate Processing/Customers

   -   Select the Customer record from the Customer List by searching and clicking on the record.
 
   -  	Once you have selected your customer record, click on the “Navigate ribbon/Ledger Entries” and select the invoice you wish to            preview.
 
   -   Click on the “Navigate” Button and select “Posted Sales Invoice”
 
   -   If you wish to Preview the record click on “Show Posted Document”. 
 
###	Posted Invoices
You can preview posted invoices from within the Posted Invoices area.  You can access the Posted Invoices from:

Departments/Labour Hire/Invoice Processing/Lists/Posted Invoices

   -   Select the Invoice No. by searching and clicking on the record.
   
   -   Click on “Print”. 
   
## Emailing Invoices

Within Dynamics NAV you have the ability to email invoices to customers.  The “E-Mail Invoice/Cr. Memo” flag must be set and “Invoice Customer E-Mail List” must be updated.  

To email the invoice, go to the following menu:

Departments/Labour Hire/Invoice Processing/Tasks/E-Mail Invoice List
 
### “Edit – E-Mail Invoice List” window

INSERT TABLE

## Generating Manual Invoices

Invoices can be generated manually either from the Customer Card or directly from the Job Planning lines, however the automated generation invoice process is recommended as it will contain relevant job information which may be overlooked if information is manually entered.

### Customer Card

You can create a manual invoice directly from the Customer card.  First go to the Customer Card by accessing the following menu:

Departments/Labour Hire/Candidate Processing/Customers

   -   Select the Customer record from the Customer List by searching and clicking on the record.
   
   -   Once you have selected your customer record, click on the “Sales Invoice” button to create a blank invoice and click “Enter” to          create a new invoice.   When you click “Enter” the information on the “General” Tab will populate with various information from          the Customer Card.  The Posting and Document Date will default from today’s date.
 
   -   In the “Lines” Tab complete the following information at a minimum.
   
   INSERT TABLE
 
   -   Continue to enter in lines using the abovementioned steps, otherwise click on the ‘Post” or “Post and Print” button to print the        invoice. 
   
### Job Card
You can create a manual invoice directly from the Job card.  First go to the Job Card by accessing the following menu:

Departments/Labour Hire/Candidate Processing/Jobs

   -   Select the Job record from the Job List by searching and clicking on the record.
   
   -   Once you have selected your job record, click on the Home ribbon, and  “Create Job Sales Invoice” button to create an invoice for        the Job.  
 
    -   In the “Edit – Job Create Sales Invoice” window complete the following information.
 
INSERT TABLE


   -   When completed, click “OK”.  If there are no invoice lines to generate then a message will appear “There is nothing to invoice”,        otherwise you will receive a message “1 invoice is created”.
   
   -   To review the Job created invoice, go to the following menu:  Departments/Labour Hire/Invoice Processing/Lists/Sales Invoice
   
   -   To finalise and post the invoice refer to 2.4 - Posting the Invoice
   
# SALES CR/ADJ NOTES PROCESSING OVERVIEW

This section will discuss two (2) methods in which Sales CR/Adj Notes can be generated:

   -   Generate Invoice
   
   -   Manually generating CR/Adj notes

## 	Generate Invoice
This function generates both Invoices and CR/Adj Notes.  To generate invoices and CR/Adj notes, go to the following menu:

Departments/Labour Hire/Invoice Processing/Generate Invoice/ Generate Invoice
 
###	“Invoice/Credit Generate” window

INSERT TABLE

 

###	““Edit – Sales Invoice/Credit Note Generation Customer FastTab” window

 There are a number of filters which you can enter to further filter information:
 
 INSERT TABLE 
 

##Generated Sales CR/Adj Notes

To view generated Sales CR/Adj Notes, go to the following menu:

Departments/Labour Hire/Invoice Processing/Lists/Sales CR/Adj Notes

A list of all the sales CR/Adj notes generated will appear from which you can select to view each CR/Adj note individually. 

To check CR/Adj notes, double-click on a Sales CR/Adj and the “Edit – Sales Invoice” window will appear.

 
### “Edit – Sales CR/Adj Note” window
The “Sales CR/Adj Note” contains the following tabs and information:

INSERT TABLE



## Printing a Test Report

You can print a test report to preview CR/Adj Note information prior to posting the CR/Adj Note. 

To print a Test Report from the Sales CR/Adj Note, click on the “Actions Button>Posting>Test Report”.
 
If the report indicates any errors or lack of information, you can correct the problem and then reprint the test report again before posting the CR/Adj Note.

##	Posting the CR/Adj Note 

The CR/Adj Note lines have been generated from the information that is processed from the Timesheets.  If there are any adjustments to be made, then adjusting timesheet entries should be made rather than making adjustment to the CR/Adj Note lines.  The system will however permit adjustment to entries directly on an CR/Adj Note line prior to posting.

If the posting routine finds any errors while posting, the process will be interrupted by an error message and can be restarted once the error has been rectified.

To post the CR/Adj Note from within the Sales CR/Adj Note, Click on “Post”  or “Post and Print” buttons.
 
###	Post Button
Click on the “Post” button to post the CR/Adj Notes.

Once you select this option, a response window will appear “Do you want to post the CR/Adj Note?”.  Select “Yes” to post the CR/Adj Note.
 
###	Post and Print Button
Click on the “Post and Print” button if you want to post the invoices individually.

Once you select this option, a response window will appear “Do you want to post and print the CR/Adj Note?”.  Select “Yes” to post and print the CR/Adj note.

Upon completion, the “Sales CR/Adj Note” will print.

 
##	Reviewing Posted CR/Adj Notes

Once CR/Adj notes are posted they can be accessed from within the following areas:

   -   Using the Navigation function from within the Customer Ledger Entries on the Customer Card
   
   -   From the Posted CR/Adj Notes Menu
   
### Using the Navigation Function from Customer Ledger Entries
You can preview posted invoices from within the Customer Ledger Entries area of the Customer card.

First go to the Customer Card by accessing the following menu:

Departments/Labour Hire/Candidate Processing/Customers

   -   Select the Customer record from the Customer List by searching and clicking on the record.
 
   -   Once you have selected your customer record, click on the “Navigate ribbon” and select “Ledger Entries” and select the CR/Adj            note you wish to preview.
 
   -   Click on the “Navigate” Button and select “Posted Sales CR/Adj Note”
 
   -   If you wish to Preview the record click on “Show”, otherwise click on “Print”. 
 
###	Posted CR/Adj Notes
You can preview posted CR/Adj notes from within the Posted CR/Adj Notes area.  You can access the Posted CR/Adj Notes from:

Departments/Labour Hire/Invoice Processing/Lists/Posted CR/Adj Notes

   -   Select the CR/Adj No. by searching and clicking on the record.
   -   Click on “Print”. 
   
## Generating Manual CR/Adj Notes  

There are a number of ways to create a CR/Adj note within Dynamics NAV.  This section will discuss manually creating CR/Adj notes from the Sales CR/Adj areas using the Copy Document function.  

###	Sales CR/Adj Notes
You can create a manual CR/Adj note from the Sales CR/Adj Notes menu.

Departments/Labour Hire/Invoice Processing/Lists/Sales CR/Adj Notes

   -   Click on the “New” button and click “Enter” to create a new CR/Adj note.   When you click “Enter” the information on the                “General” Tab will populate the Posting and Document Date with today’s date.
   -   Click on the ArrowDown button in the “Sell-to Customer No.” field and select the Customer No. you wish to create a CR/Adj note          for and then click “Enter”.  When you click “Enter” the information on the “General” Tab will populate with various information          from the Customer Card. 
   -   If you are crediting an invoice which has been posted to the Customer Ledger entry, you can use the “Copy Document” function to          retrieve the previously posted lines.  To do this, click on the “Copy Document” button.  
 
   -   The “Edit – Copy Sales Document” window will open.  It should be updated as follows: 
   
INSERT TABLE   
   
 
   -   The CR/Adj note and lines will be populated with various information from the sales invoice or document you selected in the Copy        Document process.  The following information will have been generated from a Contractor invoice.  
   
   
INSERT TABLE    
   

   -   To finalise and post the CR/Adj note refer to 3.4 - Posting the CR/Adj Note




