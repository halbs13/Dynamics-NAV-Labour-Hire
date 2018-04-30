# How to setup Human Resources

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











 

This document will discuss the following Human Resources
Setup areas required to operate the Dynamics NAV Labour Hire module.

 


 Human Resources Setup
 Cause of Absence – used
     for Internal Employees
 Cause of Inactivity – used
     for Internal Employees
 Grounds for Termination
 Qualifications – used for
     Internal Employees
 Relatives – used for
     Internal Employees
 Misc. Articles – used for
     Internal Employees


.

 

2     
HUMAN RESOURCES SETUP

2.1      
Human Resources Setup

The Human Resources Setup allows you to define
rules such as Employee No. Series, Base Unit of Measures.

To access the Human Resources Setup, go to the
following menu:

Departments/Payroll/Setup/Human
Resources Setup/Human Resources Setup 

2.1.1    
“Edit - Human Resources Setup” window

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  Employee Nos
  
  
  From the AssistButton button, select the
  Employee No. series.
  If there is integration with AXiOM, the
  Employee Numbers will be generated from within AXiOM and transfer into
  NAV.  This field should be configured
  in case there are Internal Employees being paid within the Labour Hire
  module.  
  **Note:
  The No. Series should be setup first. 
  You will need to create a new No. series if one does not exist.
  
 
 
  
  Base Unit of Measure
  
  
  This field contains the base unit used to
  measure employee absences, work hours, etc. 
  E.g. the unit of measure could be hour or day.
  
 
 
  
  Hours Unit of Measure
   
  
  
  This field contains the base unit used to
  measure time within Employee Time Sheet. E.g. the unit of measure is Hour.
  
 
 
  
  Escalation Time
  
  
  This field is used to determine the duration of
  the initial escalation time used for notifications when using the TimeKeeper
  application.
  
 
 
  
  Second Escalation Time
  
  
  This field is used to determine the duration of
  second escalation time used for notifications when using the TimeKeeper
  application.
  
 
 
  
  Time Sheet Week Ending Day
  
  
  This option is used for Employee Time Sheet to
  determine when the week ending day is.
  
 
 
  
  Job Resource Validation
  
  
  This field forms part of the TimeKeeper
  interface and is used when timesheets are being validated after import from
  TimeKeeper.
  The options available for selection are: 
  ·        
  Job Planning
  Line – select this option if the Resource can only enter time where they are
  on a Planning Line for the Job(s)
  ·        
  None – select
  this option if the Resource can put time against any Job.
  
 
 
  
  Click “OK” after
  you have completed your selection.
  
 


2.2      
Causes of Absence

The Causes
of Absence table is used to set up cause of absence codes for your
employees.  These codes can be used to
indicate various reasons for employee absences: sickness, personal days,
personal emergencies, etc.  After they
have been setup, they are then mapped through to the Pay Transaction Types
within the Payroll module and transactional data transfers across to the
Absence Registration table so that further analysis can be conducted.  

To access the Causes of Absence, go to the
following menu:

Departments/Payroll/Setup/Human Resources Setup/Causes
of Absence



2.2.1    
“Edit – Causes of Absence” window

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  To create a new record, click on the “New” button.
  
 
 
  
  Code
  
  
  Enter in the cause of absence code.  You can enter in a maximum of 10 characters,
  both numbers and letters.
  
 
 
  
  Description
  
  
  Enter in a description for the cause of
  absence.
  
 
 
  
  Total Absence (Base)
  
  
  This field displays the total number of
  absences (calculated in days or hours) for all employees as regards the cause
  of absence for this line.
  The program automatically calculates and
  updates the contents of the field using the entries in the Quantity field in
  the Employee Absence table.
  It is important that you use one “unit of
  measure” consistently when registering employee absences in order to obtain
  meaningful totals and statistics on employee absences.
  
 
 
  
  Unit of Measure Code
  
  
  You can select the Unit of Measure to be used
  for calculating absences.
  
 
 
  
  Click “OK” after
  you have completed your selection.
  
 


2.3      
Causes of Inactivity

The Causes
of Inactivity table is used to set up cause of inactivity codes for your
employees.  These codes can be used to
indicate various reasons causing employee inactiveness: maternity leave,
long-term illness, sabbatical, etc.  When
you have setup the cause of inactivity codes, you can assign them to the
individual employees on the employee card. 
You can also specify a starting date for the period of inactiveness for
the employee on the employee card.  

To access the Cause of Inactivity, go to the
following menu:

Departments/Payroll/Setup/Human Resources Setup/Causes
of Inactivity



2.3.1    
“Edit – Cause of Inactivity” window

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  To create a new record, click on the “New” button.
  
 
 
  
  Code
  
  
  Enter in the cause of inactivity code.  You can enter in a maximum of 10
  characters, both numbers and letters.
  
 
 
  
  Description
  
  
  Enter in a description for the cause of
  inactivity.
  
 
 
  
  Click “OK” after
  you have completed your selection.
  
 


2.4      
Grounds for Termination

The
Grounds for Termination table is used to set up grounds for termination codes
for your employees.  These codes can be
used to indicate various reasons for employee termination: dismissal,
retirement, resignation, etc.  When you
have setup the grounds for termination codes, you can assign them to the
individual employees on the employee card. 
You can also specify a date on which the employee was terminated.  

To access the Grounds for Termination, go to the
following menu:

Departments/Payroll/Setup/Human Resources
Setup/Grounds for Termination



2.4.1    
“Edit – Grounds for Termination” window

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  To create a new record, click on the “New” button.
  
 
 
  
  Code
  
  
  Enter in the grounds for termination code.  You can enter in a maximum of 10
  characters, both numbers and letters.
  
 
 
  
  Description
  
  
  Enter in a description for the grounds for
  termination.
  
 
 
  
  Term. Lump Sum A Type
  
  
  For each of the
  Termination codes, you will need to specify the Term. Lump Sum A type
  accordingly as these will print on the INB Payment Summary.  
  The options available
  are:
  ·        
  R –
  where payment for a genuine redundancy, invalidity or under an approved early
  retirement scheme
  ·        
  T – where payment was not a payment for a genuine redundancy,
  invalidity or under an approved early retirement scheme
  
 
 
  
  ETP Applicable
  
  
  The ETP field is used to identify how the
  termination payment will be treated.  
  If the employee is terminated with a code and this field has been
  selected, the Termination payment is then taxed and treated differently.
  
 
 
  
  Click “OK” after
  you have completed your selection.
  
 


2.5      
Qualifications

The
Qualifications table is used to set up qualification codes for your
employees.  These codes can be used for
various employee qualifications: job titles, employee computer skills,
education, course, etc.   The table
enables you to effectively register and update your employees’ qualifications
in other parts of the program.  

To access the Qualifications, go to the following
menu:

Departments/Payroll/Setup/Human Resources
Setup/Qualifications

 

2.5.1    
“Edit – Qualifications” window

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  To create a new record, click on the “New” button.
  
 
 
  
  Code
  
  
  Enter in the qualifications code.  You can enter in a maximum of 10
  characters, both numbers and letters.
  
 
 
  
  Description
  
  
  Enter in a description for the qualification.
  
 
 
  
  Qualified Employees
  
  
  This field shows whether there are any employees
  with the qualification specified on the line. A yes indicates that the
  company has employees with this qualification.
  To see the employees that have this qualification,
  click the AssistButton to the right of the field
  
 
 
  
  Click “OK” after
  you have completed your selection.
  
 


2.6      
Relatives

The
Relatives table is used to set up relative codes for your employees’
relatives.   You can also use this table
to set up codes for close contacts to the employee if the employee does not
have any family.    

To access the Relatives, go to the following
menu:

Departments/Payroll/Setup/Human Resources
Setup/Relatives



 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

2.6.1    
“Edit – Relatives” window

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  To create a new record, click on the “New” button.
  
 
 
  
  Code
  
  
  Enter in the relatives code.  You can enter in a maximum of 10
  characters, both numbers and letters.
  
 
 
  
  Description
  
  
  Enter in a description for the relative.
  
 
 
  
  Click “OK” after
  you have completed your selection.
  
 





2.7      
Misc. Articles

The Misc.
Articles table is used to set up codes for the benefits that you employees
receive any other articles that are in your employees’ possession (keys,
computers, company cars, etc.) The table enables you to effectively register
and update your company’s articles in other parts of the program.  

To access the Misc. Articles, go to the following
menu:

Departments/Payroll/Setup/Human Resources Setup/Misc.
Articles



 

 

 

 

 

2.7.1    
“Edit – Misc. Articles” window

 


 
  
   
   Field Name
   
   
   Description
   
  
 
 
  
  To create a new record, click on the “New” button.
  
 
 
  
  Code
  
  
  Enter in the misc. articles code.  You can enter in a maximum of 10
  characters, both numbers and letters.
  
 
 
  
  Description
  
  
  Enter in a description for the misc. article.
  
 
 
  
  Click “OK” after
  you have completed your selection.
  
 


 

