

1      introduction

Information entered into the Payroll module during the Tax
Year is used to create the PAYG Payment Summaries. Eligible Termination
Payments (ETP) Summaries are also generated using ETP data entered against
employees when they are terminated. (E.G. the number of days worked prior to
July 1983).

 

The PAYG Payment Summaries and Eligible Termination
summaries are printed on plain paper with a laser printer using the ATO
approved layout. Income tax legislation states that if plain paper is used to
print employee PAYG Payment Summaries then the PAYG Payment Summary details
must be lodged with the ATO by magnetic media. The PAYG Payment Summary details
are generated into a data file for lodging on magnetic media.

 

After the Payment Summary is generated the employee and
employee pay transactions are flagged as having the “Payment Summary Raised” in
the Payroll Employee card until the next pay run.

 

The values printed on the Payment Summaries are taken from
the YTD Accumulators. If the YTD accumulators on Pay Transaction Types were not
setup correctly you must correct the Pay Transaction Type and then update the
YTD accumulators values using the “Update YTD Accumulation Code” function prior
to printing the Payment Summaries.

 

The Print Payment Summary menu
option is used to run the following functions: 

Print the “Payment Summary Proof List”,Print the Payment SummariesPrint Eligible Termination SummariesProduce the ATO electronic file. 









2     
End of Financial Year Processing

2.1   
Update YTD Accumulation Codes

The Pay Transaction Types used to
pay employees are accumulated to PAYG Payment summary YTD Accumulation codes.
The codes are used to accumulate YTD amounts reported on the employee’s payment
summary. 

 

Only Pay Transaction Type
payments that are reported to the ATO have an YTD Accumulation code.

 

When the Payment Summary YTD
Accumulation code has not been correctly applied to the Pay Transaction Type
you must correct the accumulation code in the Pay transaction and then run the
YTD accumulation Code Update to update the values in the Employee Ledger table.

 

 

To access the YTD Accumulation Code Update, go to the following menu:

 

Departments/Payroll/EOFY Processing/End of Tax
Year/YTD Accumulation Code Update



 

 

 

 

 

 

 

 

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  Tax Year
  
  
  Enter or select the Tax Year you wish to
  update the YTD Accumulator code values and then click the “OK” button. Note: This process does not need to
  run if there have been no changes to the “P.S. YTD Accumulation” codes on the
  Pay Transaction Types.
  
 


 

2.2   
Payment Summary Proof List

The same menu option is used to print the Payment Summary
Proof List, PAYG Payment Summaries, ETP summaries and to create the Electronic
ATO file. 

 

The Proof List can be printed without printing the PAYG
Payment Summaries by leaving the “Print Payment Summaries” field un-ticked on
the option tab. The Proof list can be run unlimited times until you are
satisfied with the amounts to print on the employee payment summaries and in
the corresponding ATO electronic file.

The “Payment Summary Proof List” is designed to assist you
in balancing your Payroll for the Taxation year. You can select parameters
(filters) to assist you in the balancing and checking of the Payment Summaries.
The Proof List prints errors and warnings that must be corrected before the
PAYG Payment Summaries and ATO Electronic file are produced.

 

Note: Depending
on the type of error produced the process will not continue. For example, if
Payroll Company information is missing the process will stop; if employee
information is missing the process continues.

 

PAYG Payment Summaries are not produced for an employee with
an “Incorporated Company” type. These employees are still printed on the
“Payment Summary Proof List” to assist with the End of Year (EOY)
reconciliation process.

 

Note: A “PAYG
Payment Summary Proof List” is always printed, by default, when selecting the
“Print PAYG Payment Summaries” option. This is used to provide proof of the
values printed on the PAYG Payment Summaries and supplied to the ATO.

 

To
print the PAY Payment Summary Proof List, go to the following menu:

 

Departments/Payroll/EOFY Processing/End of Tax
Year/EOTY Payment Summaries

 



 

 

Select End of Tax Year processing
and click “OK”

 



 

 

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  PAYROLL FASTTAB -  Only
  the standard fields are covered. A full list if fields available as filters
  can be used by selecting the first blank line and clicking the “ArrowDown”
  
 
 
  
  No.
  
  
  Select a Payroll(s) to use as a filter to
  limit the employee’s printed. If left blank all Payroll(s) will print
  
 
 
  
  PAYROLL EMPLOYEE FASTTAB -  Only the standard fields are covered. A full
  list if fields available as filters can be used by selecting the first blank
  line and clicking the “ArrowDown”.
  
 
 
  
  Employee No.
  
  
  
  Select an Employee(s) to use as a filter to limit the employee’s. If
  left blank all Employee PAYG Payment Summaries details for the selected
  Payroll(s) will print.
  
  
 
 
  
  OPTIONS FASTTAB
  
  
 
 
  
  Tax Year
  
  
  
  Select the Tax Year you wish to reconcile and report.
  
  
 
 
  
  Print PAYG
  Payment Summaries
  
  
  
  Leave this field blank to print the “Payment Summary Proof List” without
  the PAYG Payment Summaries and file. The proof list can be run, unlimited
  times and is used to confirm the amounts that are printed on the employee’s
  PAYG Payment Summaries.
  If this field is ticked the Employee PAYG Payment Summaries are
  printed and the rest of the fields are displayed. The Employee and their
  transactions are flagged as “PAYG Payment Summaries printed”.
  
  
 
 
  
  Click “OK” once
  you have completed your selection.
  
  
 
 
 
  
  
  
  
 
 


 

2.3    Printing
PAYG Summaries

This process is used
to Print the PAYG Payment Summaries and Create the Electronic Media File.

 

The same menu option is
used to print the Payment Summary Proof List, PAYG Payment Summaries, ETP’s and
to create the Electronic ATO file. 

 

There are five types of
PAYG Payment Summaries that can be produced.

 


 Individual
     Non-Business
 Labour
     Hire
 Personal
     Services
 Volutary
     Agreement
 Eligible
     Termination Payment


 

The Payment Summary
Proof List function automatically prints the correct Payment Summary Type when
the process is run. Employees receive the type of Summary based on their
“Employment Basis” attached to the “Employee Type Code” on the Employee Payroll
Card – General Tab. PAYG Payment Summaries are not produced for employee’s with
an “Incorporated Company” type. 

 

The payment
summaries cannot be previewed; you must print the PAYG payment summaries. The
PAYG Payment Summaries are printed to your MS Windows default printer. If the
PAYG Payment Summaries must be printed to a different printer other than your
default printer then set the other printer as your default windows printer
before printing the payment summaries.

 

A “Payment Summary
Proof List” is always printed, by default. This is used to provide proof of the
values printed on the Payment Summaries and supplied to the ATO.

The format of the
ATO Electronic file name is defaulted. You must indicate the path where the
file is to be placed by entering the path location or navigating to the
required directory. If no Path is present then the file will be written to the
Navision client directory on your PC.

 

Note: Eligible Termination Payment ( ETP ) summaries are produced
automatically during the PAYG Payment Summary process if you have entered the
employees ETP details using the Eligible Termination Pay task accessed via the
button  from the Payroll
Employee Card.

 

 



 

To print the PAYG Payment
Summary, go to the
following menu:

 

Departments/Payroll/EOFY
Processing/End of Tax Year/EOTY Payment Summaries

 



 

 

Select Either Normal Processing or End of Tax
Year processing and click “OK”

 



 

 


 
  
   
   Field Name
   
   
   
   Description
   
   
  
 
 
  
  PAYROLL FASTTAB -  Only
  the standard fields are covered. A full list if fields available as filters
  can be used by selecting the first blank line and clicking the “ArrowDown”
  
  
 
 
  
  No.
  
  
  
  Select a Payroll(s) to use as a filter to limit the employee’s
  printed. If left blank all Payroll(s) will print
  
  
 
 
  
  PAYROLL EMPLOYEE FASTTAB -  Only
  the standard fields are covered. A full list if fields available as filters
  can be used by selecting the first blank line and clicking the “ArrowDown”
  
  
 
 
  
  Employee No.
  
  
  
  Select an Employee(s) to use as a filter to limit the employee’s. If
  left blank all Employee PAYG Payment Summaries details for the selected
  Payroll(s) will print.
  
  
 
 
  
  OPTIONS FASTTAB
  
  
 
 
  
  Tax Year
  
  
  
  Select the Tax Year you wish to reconcile and report.
  
  
 
 
  
  Print PAYG
  Payment Summaries
  
  
  
  Tick this field to print the Employee Payment summaries. The Employee
  and their transactions are flagged as “PAYG Payment Summaries printed”. If
  left blank only the “Payment Summary Proof List” is printed.
  
  
 
 
  
  Date
  
  
  
  This date prints as the signatory date on the PAYG Payment Summary.
  This date has no effect on the production or selection of the payments
  summaries.
  
  
 
 
  
  Authorised
  Person
  
  
  
  Use this field to enter the Authorised Person’s name registered with
  the ATO. This field is printed on each PAYG Payment Summary. If left blank
  the Individual PAYG Payment Summary must be manually signed by the Authorised
  signatory from your organization.
  
  
 
 
  
  Include Printed
  
  
  
  Tick this flag to print previously printed PAYG Payment Summaries.
  This option is used to reprint PAYG Payment Summaries already printed for
  termination employees or when an employee has misplaced the original. 
  
  
 
 
  
  Employee  No.
  
  
  
  Select an Employee No(s) to use as a filter to limit the employee for
  the selected payroll. If left blank all Employee Payment Summaries details
  for the selected Payroll(s) will print.
  
  
 
 
  
  Do Not Create
  Electronics File
  
  
  
  It is recommended that this field is blank when printing PAYG Payment
  Summaries to ensure your ATO electronic file always reflects the amounts
  printed on the PAYG Payment summaries.
  
   
  
  
 
 
  
  File Name
  
  
  
  This field is used to enter the file path and name. The default value
  in this field is the file name format required by the ATO. You must specify
  the file path where the file is to be created; click the button to locate the file.The default
  file name is :Empdupe.A01”. The ‘01” can be incremented manually when there
  is more than one Payment Summary print cycle.When running the process for
  more than one payroll the process will automatically produce one file for
  each Payroll. The file extension (A01) will be austomatically increment for
  each payroll file produced.
  
  
 
 
  
  Run Type
  
  
  
  This field must be “Production”. Select “Test” only to send a test
  file to the ATO for clarification before creating the production file. Dialog
  has received confirmation for the layout from the ATO therefore Test should
  be used only if required.
  
  
 
 
  
  Supplier File
  Reference
  
  
  
  This field is used by the ATO to further identify the file for
  enquiries from the ATO to you.
  
  
 
 
  
  Click
  “OK” once you have completed your selection.
  
 


