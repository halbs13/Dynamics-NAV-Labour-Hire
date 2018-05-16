# INVOICE PROCESSING OVERVIEW

Dynamics NAV Labour Hire’s  Sales Invoice and Sales CR/Adj Note generation function has been designed to automatically generate invoice  for customers using data transferred from the Time Sheet Line table.  The data entered and processed from the Time Sheet Line table will update the Job Planning Lines ready for customer invoices and credit notes to be generated.  

The Invoice and CR/Adj Note Generation function has been designed to cater for the following requirements:

- Generation Selection: Ability to select which customers to generate invoices for.
- Invoice Frequency: Generate invoices at different intervals depending on customer choice.
- Invoice Consolidation: Different levels of consolidation can be selected for customers.  Examples of consolidation are one invoice for each sell to customer or one invoice for just the bill to customer, which represents a parent or umbrella type company.
These features allow users to set up all of the required parameters at a customer level.  

When it comes time to generate invoices, they will simply have to select an option and filter on some choices if required and the invoices and credit notes will automatically be generated correctly for each customer.

The section specifically discusses the process for generating invoices manually from the job planning lines and using the “Generate Sales Invoice” Option.  


## Invoice Processing

This section discusses two (2) methods in which invoices can be generated:

- [Generate Invoice](#generate-invoice) 
- [Manually generating Invoices from the Customer and Job Cards](#generated-invoices)

## Generate Invoice

This function generates both Invoices and CR/Adj Notes.
  
1.  To generate invoices and CR/Adj notes, go to the following menu: *Departments/Labour Hire/Invoice Processing/Generate Invoice/ Generate Invoice*
 
2.  On the **Invoice/Credit Generate** window, fill the fields as described in the table below.

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Posting Date**|Fill in the **Posting Date** field with the posting date. This date will be used as the **Posting Date** on all generated Invoices and Credit Notes and sales records will be posted to the relevant ledger using this date.|
|**Generate**|From the **Generate** field, select your option. Each customer will have set up with an Invoice Frequency, so this should be selected depending on which batch of invoices you are generating.  All customers with a matching frequency will have invoices generated if they have trainings waiting to be invoiced.  The Adhoc option allows you to generate invoices for all customers regardless of frequency.|

3.  Click on the **Generate** button after you have completed your selection.

4.  On the **Customer** FastTab on the **Sales Invvoice/Credit Note Generation** window, you can enter filters as described in the following table.
 
|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Customer No.**|	Select a  **Customer No.** or leave blank for all customers with the same frequency.|

5.  Click the **OK** button.

[GoToTop](#invoice-processing-overview)

## Generated Invoices

1.  To view generated Invoices, go to the following menu: *Departments/Labour Hire/Invoice Processing/Lists/Sales Invoice*

A list of all the sales invoices generated will appear from which you can select to view each invoice individually.  Alternatively you can post the batch of invoices by selecting the **Post Batch** or post individually by nominating the **Post** button.

To check invoices individually, double-click on a Sales Invoice and the “Edit – Sales Invoice” window will appear.
 
2.  The **General** FastTab of the **Sales Invoice** contains the following tabs and information:

|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**Posting Date**|This is the Posting Date entered used to generate the invoice|
|**Document Date**|This is the date the invoice is generated and is used to determine the “Due Date” on the invoice|
|**External Document No.**|This will be left blank but can be used as a reference number for the customer|
|**Invoice/Cr. Memo Format Code**|This is the Sales Invoice Format code sourced from the Customer Card|

3.  The **Lines** FastTab of the **Sales Invoice** contains the following information.

|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**Type**|This will default to “Resource”|
|**No.**|This is the “Resource No.”|
|**Description**|This field will populate from the Pay Transaction Type code as a description|
|**Quantity**|This field will contain the quantity or number of hours|
|**Unit of Measure Code**|This field contains the Unit of Measure Code |
|**Unit Price Excl. GST**|This field contains the “Charge Rate” |
|**Line Amount Excl. GST**|This field contains the Line Amount (Quantity * “Unit Price Excl. GST)|

4.  The **Invoicing** FastTab of the **Sales Invoice** contains the following information.


|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**Invoice Type**|This option will default to “Times”|
|**Payment Terms Code**|The Payment Terms code will be sourced from the Customer Card|
|**Due Date**|This field is populated calculated from the “Document Date” |
|**Payment Method Code**|The Payment Method code will be sourced from the Customer Card|
|**GST Bus. Posting Group**|The GST Bus. Posting Group will be sourced from the Customer Card|


## Printing a Test Report 

You can print a test report to preview invoice information prior to posting the invoice. 

To print a Test Report from the Sales Invoice, click on the **“Actions ribbon> Posting> Test Report”**.

If the report indicates any errors or lack of information, you can correct the problem and then reprint the test report again before posting the invoice.

[GoToTop](#invoice-processing-overview)

## Posting the Invoice 

The Invoice lines have been generated from the information that is processed from the Timesheets.  If there are any adjustments to be made, then adjusting timesheet entries should be made rather than making adjustment to the invoice lines.  The system will however permit adjustment to entries directly on an invoice line prior to posting.

Invoices can be checked via the Test Report and should be posted once checking is complete.  

If the posting routine finds any errors while posting, the process will be interrupted by an error message and can be restarted once the error has been rectified.

To post the invoice from within the Sales Invoice, Click on **Post**  or **Post and Print** buttons.


### Post Button

1.  Click on the **Post** button if you want to post the invoices individually without printing the Sales Invoice.

2.  Once you select this option, a response window will appear **Do you want to post the Invoice?**.  Select **Yes** to post the invoice.

3.  Upon completion, the **Posted Invoice List** will print.
 
### Post and Print Button

1.  Click on the **Post and Print** button if you want to post the invoices individually.

2.  Once you select this option, a response window will appear **Do you want to post and print the Invoice?**.  Select **Yes** to post and print the invoice.

3.  Upon completion, the “Sales Invoice” and **Posted Invoice List** will print.
 
### Post Batch

1.  Click on the **Post Batch** button if you want to post a batch of invoices.
 
2.  On the **Options** FastTab of the **Batch Post Sales Invoices** window, the following fields are available for review.

|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**Posting Date**|Enter in a Posting Date if you wish to override the Posting Date used to generate the invoice, otherwise leave this blank.|
|**Replace Posting Date**|Tick this field if you wish to replace the Posting Date on the invoices generated. |
|**Replace Document Date**|Tick this field if you wish to replace the Document Date on the invoices generated.|

3.  On the **Sales Invoice** FastTab, the following fields are available for review.

|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**No.**|Enter in the Invoice No. range you wish to post. Note – you may have to make note of this prior to selection|

4.  Click **OK** once you have completed your selection.

5.  Upon completion, the **Posted Invoice List** window will appear where you can print, preview or cancel the report. 

[GoToTop](#invoice-processing-overview)
 
## Reviewing Posted Invoices
 
Once invoices are posted they can be accessed from within the following areas:

- Using the Navigation function from within the Customer Ledger Entries on the Customer Card
- From the Posted Invoices Menu


### Using the Navigation Function from Customer Ledger Entries

You can preview posted invoices from within the Customer Ledger Entries area of the Customer card.

1.  Go to the Customer Card by accessing the following menu: *Departments/Labour Hire/Candidate Processing/Customers*

2.	Select the Customer record from the Customer List by searching and clicking on the record.
 
3.	Once you have selected your customer record, click on the “Navigate ribbon/Ledger Entries” and select the invoice you wish to preview.
 
4.	Click on the “Navigate” Button and select “Posted Sales Invoice”
 
5.	If you wish to Preview the record click on “Show Posted Document”. 
 

### Posted Invoices

You can preview posted invoices from within the Posted Invoices area.  You can access the Posted Invoices from: *Departments/Labour Hire/Invoice Processing/Lists/Posted Invoices*

1.	Select the Invoice No. by searching and clicking on the record.
2.	Click on “Print”. 

[GoToTop](#invoice-processing-overview)

## Emailing Invoices

Within Dynamics NAV you have the ability to email invoices to customers.  The “E-Mail Invoice/Cr. Memo” flag must be set and “Invoice Customer E-Mail List” must be updated.  

1.  To email the invoice, go to the following menu: *Departments/Labour Hire/Invoice Processing/Tasks/E-Mail Invoice List*

2.  On the **Options** FastTab of the **E-Mail Invoice List** window, the following fields are available for review.

|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**Message**|You can enter in a message to print out on the invoice.  **Note: you must have a “Message” section on your invoice for this information to print.**|

3.  On the **Sales Invoice Header** FastTab of the **E-Mail Invoice List** window, the following fields are available for review.

|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**Sell-to Customer No.**|From the **ArrowDown**, select or enter in the Customer No. you wish to email to|
|**No.**|From the **ArrowDown**, select or enter in the Invoice No. you wish to.|

4.  You can also enter in other filters as necessary, otherwise click on the **OK** after you have completed your selection.

[GoToTop](#invoice-processing-overview)

## Generating Manual Invoices  

Invoices can be generated manually either from the Customer Card or directly from the Job Planning lines, however the automated generation invoice process is recommended as it will contain relevant job information which may be overlooked if information is manually entered.

### Customer Card

You can create a manual invoice directly from the Customer card.  

1.  Go to the Customer Card by accessing the following menu: *Departments/Labour Hire/Candidate Processing/Customers*

2.	Select the Customer record from the Customer List by searching and clicking on the record.

3.	Once you have selected your customer record, click on the “Sales Invoice” button to create a blank invoice and click “Enter” to create a new invoice.   When you click “Enter” the information on the “General” Tab will populate with various information from the Customer Card.  The Posting and Document Date will default from today’s date.
 
4.	On the **Lines** FastTab of the **Sales Invoice**, fill the fields as described in the following table. 
 
|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**Type**|If you are producing a manual invoice for a contractor, select from the options “Resource”|
|**No.**|If you have selected “Resource” as the Type, in this field you will be able to select the appropriate Contractor Number from the Lookup button.|
|**Description**|Enter in the Description which will appear in the Invoice Description.  This will default to the Resources Name but can be overwritten|
|**Quantity**|Enter in the number of units/hours|
|**Unit of Measure Code**|This information will default from the Resource Card|
|**GST Prod Posting Group**|This information will default from the Resource Card|
|**Unit Price Excl. GST**|Enter in the Charge Rate|


5.	Continue to enter in lines using the abovementioned steps, otherwise click on the **Post** or **Post and Print** button to print the invoice. 

### Job Card

You can create a manual invoice directly from the Job card.  

1.  Go to the Job Card by accessing the following menu: *Departments/Labour Hire/Candidate Processing/Jobs*

2.	Select the Job record from the Job List by searching and clicking on the record.

3.	Once you have selected your job record, click on the Home ribbon, and  “Create Job Sales Invoice” button to create an invoice for the Job.  

4.	On the **Options** FastTab of the **Job Create Sales Invoice** window complete the following information.
 
|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**Posting Date**|The date will default to today’s date but can be changed where applicable.|
|**Create Invoice Per**|You can nominate to create the invoice by Job or Job Task.|

5.  On the **Job Task** FastTab of the **Job Create Sales Invoice** window complete the following information.

|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**Job No.**|If you wish to create an invoice by Job No., enter or select the Job No. from the ArrowDown button.|
|**Job Task No.**|If you wish to create an invoice for a particular Job Task No. of a Job, enter in the Job Task No. by clicking on the **ArrowDown**. **You can also enter in other filters as necessary**|

5.	When completed, click “OK”.  If there are no invoice lines to generate then a message will appear “There is nothing to invoice”, otherwise you will receive a message “1 invoice is created”.

6.	To review the Job created invoice, go to the following menu:  *Departments/Labour Hire/Invoice Processing/Lists/Sales Invoice*

7.	To finalise and post the invoice refer to **Posting the Invoice**

#	SALES CR/ADJ NOTES PROCESSING OVERVIEW


This section will discuss two (2) methods in which Sales CR/Adj Notes can be generated:

1.	[Generate Invoice](#generate-invoices) 
2.	[Manually generating CR/Adj notes](#generated-sales-cr-adj-notes) 

[GoToTop](#invoice-processing-overview)

## Generate Invoices

This function generates both Invoices and CR/Adj Notes.  

1.  To generate invoices and CR/Adj notes, go to the following menu: *Departments/Labour Hire/Invoice Processing/Generate Invoice/ Generate Invoice*

2.  Fill the fields as described in the following table.
 
|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**Posting Date**|Fill in the “Posting Date” field with the posting date. This date will be used as the “Posting Date on all generated Invoices and Credit Notes and sales records will be posted to the relevant ledger using this date.|
|**Generate**|From the “Generate” field, select your option. Each customer will have set up with an Invoice Frequency, so this should be selected depending on which batch of invoices you are generating.  All customers with a matching frequency will have invoices generated if they have trainings waiting to be invoiced. The Adhoc option allows you to generate invoices for all customers regardless of frequency.|

3.  Click on the **Generate** button after you have completed your selection.

4.  On the **Customer** FastTab of the **Sales Invoice/Credit Note Generation** fill the fields as described in the following table.  

|Field Name|Description|
|------------------|---------------------------------------------------------|
|**Customer No.**|Select a  “Customer No.” or leave blank for all customers with the same frequency.|

5.  Click the **OK** button.

## Generated Sales CR Adj Notes

1.  To view generated Sales CR/Adj Notes, go to the following menu: *Departments/Labour Hire/Invoice Processing/Lists/Sales CR/Adj Notes*

A list of all the sales CR/Adj notes generated will appear from which you can select to view each CR/Adj note individually.  

2.  To review the CR/Adj notes, double-click on a **Sales CR/Adj**.  

3.  On the **General** FastTab of the **Sales CR/Adj** card the following fields are avaialble for review.
 

|Field Name|Description|
|------------|---------------------------------------------------------|
|**Posting Date**|This is the Posting Date entered used to generate the invoice|
|**Document Date**|This is the date the invoice is generated and is used to determine the “Due Date” on the invoice|
|**External Document No.**|This will be left blank but can be used as a reference number for the customer|
|**Invoice/Cr. Memo Format Code**|This is the Sales CR/Adj Note Format code sourced from the Customer Card|

4.  On the **Lines** FastTab of the **Sales CR/Adj** card the following fields are avaialble for review.

|Field Name|Description|
|------------|---------------------------------------------------------|
|**Type**|This will default to “Resource”|
|**No.**|This is the “Resource No.”|
|**Description**|This field will populate from the Pay Transaction Type code as a description|
|**Quantity**|This field will contain the quantity or number of hours|
|**Unit of Measure Code**|This field contains the Unit of Measure Code |
|**Unit Price Excl. GST**|This field contains the “Charge Rate” |
|**Line Amount Excl. GST**|This field contains the Line Amount (Quantity * “Unit Price Excl. GST)|

5.  On the **Invoicing** FastTab of the **Sales CR/Adj** card the following fields are avaialble for review.

|Field Name|Description|
|------------|---------------------------------------------------------|
|**Invoice Type**|This option will default to “Times”|
|**Payment Terms Code**|The Payment Terms code will be sourced from the Customer Card|
|**Due Date**|This field is populated calculated from the “Document Date” |
|**Payment Method Code**|The Payment Method code will be sourced from the Customer Card|
|**GST Bus. Posting Group**|The GST Bus. Posting Group will be sourced from the Customer Card|

6.  On the **Application** FastTab of the **Sales CR/Adj** card the following fields are avaialble for review.

|Field Name|Description|
|------------|---------------------------------------------------------|
|**Applies to Doc. Type**|This option will default to “Invoice” if it has been applied the time of entering the adjustment via Timesheet Entry|

7.  On the **Adjustment** FastTab of the **Sales CR/Adj** card the following fields are available for review.

|Field Name|Description|
|------------|---------------------------------------------------------|
|**Adjustment**|This field will be automatically flagged to highlight the CR/Adj Note will be applied as an adjustment|
|**BAS Adjustment**|This field will automatically be flagged to highlight the CR/Adj Note will be applied as a BAS adjustment|
|**Adjustment Applies-to**|This field will contain the sales invoice no. the CR/Adj Note will be applied to if entered via Timesheet Entry|
|**Reason Code**|This field will only be completed if a “Reason Code” has been filled in the Labour Hire Setup.  If this field is blank, click on the **ArrowDown** and select the reason why the CR/Adj Note is being generated|

[GoToTop](#invoice-processing-overview)

## Printing a Test Report
 
1.  You can print a test report to preview CR/Adj Note information prior to posting the CR/Adj Note. 

2.  To print a Test Report from the Sales CR/Adj Note, click on the **“Actions Button>Posting>Test Report”**.
 
3.  If the report indicates any errors or lack of information, you can correct the problem and then reprint the test report again before posting the CR/Adj Note.


## Posting the CR/Adj Note 

The CR/Adj Note lines have been generated from the information that is processed from the Timesheets.  If there are any adjustments to be made, then adjusting timesheet entries should be made rather than making adjustment to the CR/Adj Note lines.  The system will however permit adjustment to entries directly on an CR/Adj Note line prior to posting.

If the posting routine finds any errors while posting, the process will be interrupted by an error message and can be restarted once the error has been rectified.

To post the CR/Adj Note from within the Sales CR/Adj Note, Click on **Post**  or **Post and Print** buttons.
 

### Post Button

1.  Click on the **Post** button to post the CR/Adj Notes.

2.  Once you select this option, a response window will appear **Do you want to post the CR/Adj Note?**.  Select **Yes** to post the CR/Adj Note.
 

### Post and Print Button

1.  Click on the **Post and Print** button if you want to post the invoices individually.

2.  Once you select this option, a response window will appear **Do you want to post and print the CR/Adj Note?**.  Select **Yes** to post and print the CR/Adj note.

3.  Upon completion, the **Sales CR/Adj Note** will print.

 [GoToTop](#invoice-processing-overview)
 
## Reviewing Posted CR/Adj Notes

Once CR/Adj notes are posted they can be accessed from within the following areas:

- Using the Navigation function from within the Customer Ledger Entries on the Customer Card
- From the Posted CR/Adj Notes Menu


### Using the Navigation Function from Customer Ledger Entries

You can preview posted invoices from within the Customer Ledger Entries area of the Customer card.

1. Go to the Customer Card by accessing the following menu: *Departments/Labour Hire/Candidate Processing/Customers*

2.	Select the Customer record from the Customer List by searching and clicking on the record.
 
3.	Once you have selected your customer record, click on the “Navigate ribbon” and select “Ledger Entries” and select the CR/Adj note you wish to preview.
 
4.	Click on the “Navigate” Button and select “Posted Sales CR/Adj Note”
 
5.	If you wish to Preview the record click on “Show”, otherwise click on “Print”. 
 
### Posted CR/Adj Notes

You can preview posted CR/Adj notes from within the Posted CR/Adj Notes area.  

1.  You can access the Posted CR/Adj Notes from: *Departments/Labour Hire/Invoice Processing/Lists/Posted CR/Adj Notes*

2.	Select the CR/Adj No. by searching and clicking on the record.

3.	Click on **Print**. 

[GoToTop](#invoice-processing-overview)

## Generating Manual CR/Adj Notes  

There are a number of ways to create a CR/Adj note within Dynamics NAV.  This section will discuss manually creating CR/Adj notes from the Sales CR/Adj areas using the Copy Document function.  


### Sales CR/Adj Notes

You can create a manual CR/Adj note from the Sales CR/Adj Notes menu. *Departments/Labour Hire/Invoice Processing/Lists/Sales CR/Adj Notes*

1.	Click on the “New” button and click “Enter” to create a new CR/Adj note.   When you click “Enter” the information on the “General” Tab will populate the Posting and Document Date with today’s date.

2.	Click on the ArrowDown button in the “Sell-to Customer No.” field and select the Customer No. you wish to create a CR/Adj note for and then click “Enter” .  When you click “Enter” the information on the “General” Tab will populate with various information from the Customer Card. 

3.	If you are crediting an invoice which has been posted to the Customer Ledger entry, you can use the “Copy Document” function to retrieve the previously posted lines.  To do this, click on the “Copy Document” button.  

4.  On the **Options** FastTab of the **Copy Sales Document** update the fields as described in the following table.   

|Field Name|Description|
|----------------------|-------------------------------------------------------------------------------------------------------|
|**Document Type**|You can select the information to be copied from an invoice which has not yet been posted or from the posted invoice.  From the **ArrowDown**, click on **“Invoice” or “Posted Invoice”**.|
|**Document No.**|From the **ArrowDown**, you can nominate which Invoice or Posted Invoice you wish to copy the information from.  Once you have made your selection, click on **OK**.|
|**Sell-to Customer No.**|This is a non-editable field and will default from the record information you have selected.|
|**Sell-to Customer Name**|This is a non-editable field and will default from the record information you have selected.|
|**Include Header**|This will be automatically ticked and will include the header information from the record you have selected.|
|**Recalculate Lines**|If you wish to have the lines recalculated then you can tick this field, otherwise leave it blank.|
|**Posting Date**|If the CR/Adj note is to have a new Posting Date, then enter in the new posting date into this field.|
|**Replace Posting Date**|If you enter in a new Posting Date, this field will automatically be ticked.|
|**Replace Document Date**|If you enter in a new Posting Date, this field will automatically be ticked.|

5.  Click the **OK** button.

6.  If you changed the Posting Date as part of your selection, you will receive the following message: **“You have changed Posting Date on the sales header, but it has not been changed on the existing sales lines.  The change may affect the exchange rate used in the price calculation of the sales lines.”**

7.  Click **OK** to continue.

8.	The CR/Adj note and lines will be populated with various information from the sales invoice or document you selected in the Copy Document process.  The following information will have been generated from a Contractor invoice.  

9.  On the **General** FastTab, review the fields as described in the following table.

|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**Posting Date**|This is the Posting Date entered used to generate the CR/Adj note from the Copy Document process|
|**Document Date**|This is the Document Date entered used to generate the CR/Adj note from the Copy Document process|
|**External Document No.**|This will be left blank but can be used as a reference number for the customer|
|**Invoice/Cr. Memo Format Code**|This is the Sales CR/Adj Note Format code sourced from the Customer Card|

10.  On the **Lines** FastTab, review the fields as described in the following table.

|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**Type**|This will default to “Resource”|
|**No.**|This is the “Resource No.”|
|**Description**|This field will populate from the Pay Transaction Type code as a description|
|**Quantity**|This field will contain the quantity or number of hours|
|**Unit of Measure Code**|This field contains the Unit of Measure Code |
|**Unit Price Excl. GST**|This field contains the “Charge Rate” |
|**Line Amount Excl. GST**|This field contains the Line Amount (Quantity * “Unit Price Excl. GST)|

11.  On the **Invoicing** FastTab, review the fields as described in the following table.

|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**Invoice Type**|This option will default to “Times”|
|**Payment Terms Code**|The Payment Terms code will be sourced from the Customer Card|
|**Due Date**|This field is populated calculated from the “Document Date” |
|**Payment Method Code**|The Payment Method code will be sourced from the Customer Card|
|**GST Bus. Posting Group**|The GST Bus. Posting Group will be sourced from the Customer Card|

12.  On the **Application** FastTab, review the fields as described in the following table.

|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**Applies to Doc. Type**|This option will default to “Invoice” |
|**Applies-to Doc. No.**|This will default from the Invoice No. selected from the Copy Document Process|

13.  On the **Adjustment Details** FastTab, review the fields as described in the following table.

|Field Name|Description|
|-----------------------------|---------------------------------------------------------|
|**Adjustment**|This field will be automatically flagged to highlight the CR/Adj Note will be applied as an adjustment|
|**Adjustment Applies-to**|This field will contain the sales invoice no. the CR/Adj Note will be applied to selected from the Copy Document Process|
|**Reason Code**|Select the reason from the “ArrowDown” why the CR/Adj Note is being generated|


14.	To finalise and post the CR/Adj note refer to Posting the CR/Adj Note.


[GoToTop](#invoice-processing-overview)
