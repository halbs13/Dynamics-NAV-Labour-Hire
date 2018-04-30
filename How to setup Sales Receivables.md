# How to setup Sales & Receivables

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











 

This document will discuss the following Sales &
Receivables Setup areas required to operate the Dynamics NAV Labour Hire
module.

 


 Sales & Receivables
     Setup
 Customer Posting Group
 Payment Terms
 Payment
     Method


 


 

.

 

2     
SALES & RECEIVABLES SETUP

2.1      
Sales & Receivables Setup

You use
the Sales & Receivables Setup to set up certain basic rules to be used in
the Sales & Receivables application area. 


A number
series must be setup for the records, regardless of whether the number will be
manually entered into Dynamics NAV or transferred via the interface.

To access the Sales & Receivables Setup, go
to the following menu:

Departments/Financial Management/Receivables/Setup/Sales
& Receivables Setup

2.1.1    
“Edit – Sales & Receivables Setup” window

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  GENERAL FASTTAB – you specify options such as
  how you want to calculate and post discounts and what warnings you would like
  to have displayed.
  
 
 
  
  Discount Posting
  
  
  The options you have available are “No
  Discounts, Invoice Discounts, Line Discounts and All Discounts”
  This field only needs to be configured if the
  customer is using Discounts.
  
 
 
  
  Credit Warnings
  
  
  You can choose not to have warnings telling you
  that the customer’s credit limit has been exceeded.
  The options available are “Both Warnings,
  Credit Limit, Overdue Balance, No Warning”
  This field only needs to be configured if the
  customer chooses Credit Warnings.
  
 
 
  
  Logo Position on Documents
  
  
  Determine the position of the logo by clicking
  the AssistButton to the right of the field and selecting one of the four
  options: No Logo, Left, Centre, Right.
  
 
 
  
  Default Posting Date
  
  
  This field will define how to use the Posting
  Date field on Sales documents.  
  If you select Work Date, the Posting Date field
  will hold the work date by default in case your transactions may wrongfully
  hold the work date if you forget to change the posting date.
  If you select No Date, the Posting Date field
  will be empty by default and you must manually enter a posting date before
  posting.
  
 
 
  
  NUMBERING FASTTAB – you specify the number
  series that will be used for customers, sales documents, reminders, etc.  
  
 
 
  
  Customer Nos
  
  
  Enter in the code for the Number series that
  will be used to assign numbers to customers. 
  
  **Note – Where there is integration with AXiOM,
  the Customer number will be generated from within AXiOM and transfer across
  to NAV.
  
 
 
  
  Quote Nos
  
  
  Enter in the code for the Number series that
  will be used to assign numbers to sales quotes.  
  
 
 
  
  Invoice Nos
  
  
  Enter in the code for the Number series that
  will be used to assign numbers to sales invoices.
  
 
 
  
  Posted Invoice Nos
  
  
  Enter in the code for the Number series that
  will be used to assign numbers to sales posted invoices.
  
 
 
  
  CR/Adj Notes Nos
  
  
  Enter in the code for the Number series that
  will be used to assign numbers to sales CR/Adj notes.
  
 
 
  
  Posted CR/Adj Note Nos
  
  
  Enter in the code for the Number series that
  will be used to assign numbers to posted sales CR/Adj notes.
  
 
 
  
  Click “OK” after
  you have completed your selection.
  
 


 

2.2      
Customer Posting Groups

The Customer Posting Groups window is used to
setup one or more customer posting groups. 
For each posting group you setup, you must create links to the relevant
G/L accounts.  You can use the same G/L account
numbers or different account number for each posting group. 

After you have set up the posting groups, you assign them to the
relevant customer accounts.  When you
post to a customer account, the program will post to the G/L account that is
specified by the customer posting group that is linked to the customer
account.  

To access the Customer Posting Groups, go to the
following menu:

Departments/Administration/Application
Setup/Financial Management/Posting Groups/Customer Posting Groups

2.2.1    
“Edit – Customer Posting Groups” window


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  To create a new record, click on the “New” button.
  
 
 
  
  Code
  
  
  Enter in a Customer Posting Group code.  You can enter a maximum of 10 characters,
  both numbers and letters.
  
 
 
  
  Receivables Account
  
  
  Enter in the G/L account to which you want the
  program to post receivables for the customers in this posting group.
  
 
 
  
  Service Charge Acc.
  
  
  Enter in the G/L account to which you want the
  program to post service charges for customers in this posting group.  
  
 
 
  
  Payment Disc. Debit Acc.
  
  
  Enter in the G/L account to which you want the
  program to post payment discounts granted to customers in this posting group.
  
 
 
  
  Payment Disc. Credit Acc.
  
  
  Enter in the G/L account to which you want the
  program to post reductions in payment discounted granted to customers in this
  posting group.
  
 
 
  
  Interest Account
  
  
  Enter in the G/L account to which you want the
  program to post interest from reminders and finance charge memos for
  customers in this posting group.
  
 
 
  
  Additional Fee Account
  
  
  Enter in the G/L account to which you want the
  program to post additional fees from reminders and finance charge memo for
  customers in this posting group.
  
 
 
  
  Invoice Rounding Account
  
  
  Enter in the G/L account to which you want the
  program to post amounts resulting from invoice rounding when you post
  transactions involving customers.
  
 
 
  
  Debit Curr. Appln. Rndg. Acc. 
  
  
  Enter in the G/L account to which you want the
  program to post rounding differences that can occur when you apply entries in
  different currencies to one another.
  
 
 
  
  Credit Curr. Appln. Rndg. Acc.
  
  
  Enter in the G/L account to which you want the
  program to post rounding differences that can occur when you apply entries in
  different currencies to one another.
  
 
 
  
  Debit Rounding Account
  
  
  Enter in the G/L account to which you want the
  program to post rounding differences from remaining amount.
  
 
 
  
  Credit Rounding Account
  
  
  Enter in the G/L account to which you want the
  program to post rounding differences from remaining amount.
  
 
 
  
  Payment Tolerance Debit Acc.
  
  
  Enter in the G/L account to which you want the
  program to post payment tolerance when you post payments for sales with this
  particular combination of business group and product group.
  Complete this field only if the “Adjust for
  Payment Disc.” Field in the General Ledger Setup table has not been
  activated.
  
 
 
  
  Payment Tolerance Credit Acc.
  
  
  Enter in the G/L account to which you want the
  program to post payment tolerance when you post payments for sales with this
  particular combination of business group and product group.
  Complete this field only if the “Adjust for
  Payment Disc.” Field in the General Ledger Setup table has not been
  activated.
  
 
 
  
  Click “OK” after
  you have completed your selection.
  
 


 

2.3      
Payment Terms

The Payment Terms window is used to set up codes
for each set of payment terms.

To access the Payment Terms, go to the following
menu:

Departments/Financial
Management/Receivables/Setup/Payment Terms



2.3.1    
“Edit – Payment Terms” window


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  To create a new record, click on the “New” button.
  
 
 
  
  Code
  
  
  Enter in a Payment Terms code.  You can enter a maximum of 10 characters,
  both numbers and letters.
  
 
 
  
  Due Date Calculation
  
  
  Enter in a formula that will tell the program
  how to calculate the due date, e.g. when you create an invoice.
  The due date calculation formula can contain a
  maximum of 20 characters, consisting of numbers and letters, that the program
  recognizes as abbreviations for time specifications.
  
 
 
  
  Discount Date Calculation
  
  
  If the payment terms include a possible payment
  discount, you can enter a date formula for it here.
  If you enter a date formula here, the program
  will automatically calculate a payment discount date when you create an
  invoice.  The date indicates the
  deadline for receiving a payment discount.
  
 
 
  
  Discount %
  
  
  Enter the percentage of the invoice amount
  (amount including GST is the default setting) that will constitute a possible
  payment discount.
  
 
 
  
  Calc. Pmt. Disc. On CR/Adj N. field
  
  
  A checkmark in this field indicates that the
  program will calculate a payment discount on CR/Adj notes with these payment
  terms.
  
 
 
  
  Description
  
  
  Enter an explanation of the payment terms.
  
 
 
  
  Click “OK” after
  you have completed your selection.
  
 


            

2.4      
Payment Method

The Payment Method window is used to set up codes
for each set of payment method you use.

To access the Payment Method, go to the following
menu:

Departments/Financial
Management/Receivables/Setup/Payment Methods



2.4.1    
“Edit – Payment Methods” window


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  To create a new record, click on the “New” button.
  
 
 
  
  Code
  
  
  Enter in a Payment Method code.  You can enter a maximum of 10 characters,
  both numbers and letters.
  
 
 
  
  Description
  
  
  Enter in the text that describes the payment
  method.
  
 
 
  
  Bal. Account Type 
  
  
  Enter the code for the balancing account type
  that will be used in connection with this payment method.
  
 
 
  
  Bal. Account No. 
  
  
  Enter in the number of the balancing account
  that will be used in connection with this payment method.
  
 
 
  
  Payment Processor
  
  
  This field identifies the “Dynamics Online”
  will be used as the payment processor.
  Leave this option blank.
  
 
 
  
  Click “OK” after
  you have completed your selection.
  
 


            

