# How to setup Human Resources

The Dynamics NAV Labour Hire module comprises and requires various areas within Dynamics NAV
to be configured in order for it to operate. 

These areas include:

- [General Ledger](au-labour-setup-general-ledger.md)
- [Sales & Receivables](au-labour-setup-sales-receivables.md)
- [Resources & Jobs](au-labour-setup-resources-jobs.md)
- [Human Resources](au-labour-setup-human-resources.md)
- [Payroll](au-labour-setup-payroll.md)
- [Labour Hire](au-labour-setup-labour-hire.md)

This section will discuss the following setup areas within Human Resources;

- [Human Resources Setup](#to-setup-human-resources)
- [Cause of Absences](#to-setup-cause-of-absences) - used for Internal Employees
- [Cause of Inactivity](#to-setup-cause-of-inactivity) - used for Internal Employees
- [Grounds for Termination](#to-setup-grounds-for-termination) - used for Internal Employees
- [Qualifications](#to-setup-qualifications) - used for Internal Employees
- [Relatives](#to-setup-relatives) - used for Internal Employees
- [Misc. Articles](#to-setup-misc-articles) - used for Internal Employees

## To setup Human Resources
The Human Resources Setup allows you to define rules such as Employee No. Series, Base Unit of Measures.

1. In the **Search** box, enter **Human Resources Setup**, and then choose the related link.  
2. Fill the fields as described in the following table.  

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Employee Nos**|From the**ArrowDown**, select the Employee No. series. If there is integration with AXiOM, the Employee Numbers will be generated from within AXiOM and transfer into NAV.  This field should be configured in case there are Internal Employees being paid within the Labour Hire module.  **Note: The No. Series should be setup first.  You will need to create a new No. series if one does not exist.**|  
|**Base Uit of Measure**|This field contains the base unit used to measure employee absences, work hours, etc.  E.g. the unit of measure could be hour or day.|  
|**Hours Unit of Measure**|This field contains the base unit used to measure time within Employee Time Sheet. E.g. the unit of measure is Hour.|  
|**Escalation Time**|This field is used to determine the duration of the initial escalation time used for notifications when using the TimeKeeper application.| 
|**Second Escalation Time**|This field is used to determine the duration of second escalation time used for notifications when using the TimeKeeper application.|
|**Time Sheet Week Ending Day**|This option is used for Employee Time Sheet to determine when the week ending day is.|
|**Job Resource Validation**|This field forms part of the TimeKeeper interface and is used when timesheets are being validated after import from TimeKeeper. The options available for selection are: **Job Planning Line** – select this option if the Resource can only enter time where they are on a Planning Line for the Job(s). **None** – select this option if the Resource can put time against any Job.

[GoToTop](#how-to-setup-human-resources)

## To setup Cause of Absences
The Causes of Absence table is used to set up cause of absence codes for your employees.  These codes can be used to indicate various reasons for employee absences: sickness, personal days, personal emergencies, etc.  After they have been setup, they are then mapped through to the Pay Transaction Types within the Payroll module and transactional data transfers across to the Absence Registration table so that further analysis can be conducted. 

1. In the **Search** box, enter **Causes of Absence**, and then choose the related link.  
2. Fill the fields as described in the following table.  

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|    
|**Code**|Enter in the cause of absence code.  You can enter in a maximum of 10 characters, both numbers and letters.|  
|**Description**|Enter in a description for the cause of absence.|  
|**Total Absence (Base)**|This field displays the total number of absences (calculated in days or hours) for all employees as regards the cause of absence for this line. The program automatically calculates and updates the contents of the field using the entries in the Quantity field in the Employee Absence table. It is important that you use one **unit of measure** consistently when registering employee absences in order to obtain meaningful totals and statistics on employee absences.|  
|**Unit of Measure Code**|You can select the Unit of Measure to be used for calculating absences.| 
 
 [GoToTop](#how-to-setup-human-resources)
 
 ## To setup Cause of Inactivity
The Causes of Inactivity table is used to set up cause of inactivity codes for your employees.  These codes can be used to indicate various reasons causing employee inactiveness: maternity leave, long-term illness, sabbatical, etc.  When you have setup the cause of inactivity codes, you can assign them to the individual employees on the employee card.  You can also specify a starting date for the period of inactiveness for the employee on the employee card. 

1. In the **Search** box, enter **Causes of Inactivity**, and then choose the related link.  
2. Fill the fields as described in the following table.  

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Code**|Enter in the cause of inactivity code.  You can enter in a maximum of 10 characters, both numbers and letters.|  
|**Description**|Enter in a description for the cause of inactivity.|  

[GoToTop](#how-to-setup-human-resources)

## To setup Grounds for Termination
The Grounds for Termination table is used to set up grounds for termination codes for your employees.  These codes can be used to indicate various reasons for employee termination: dismissal, retirement, resignation, etc.  When you have setup the grounds for termination codes, you can assign them to the individual employees on the employee card.  You can also specify a date on which the employee was terminated. 

1. In the **Search** box, enter **Grounds for Termination**, and then choose the related link.  
2. Fill the fields as described in the following table.  

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|
|**Code**|Enter in the grounds for termination code.  You can enter in a maximum of 10 characters, both numbers and letters.|  
|**Description**|Enter in a description for the grounds for termination.|  
|**Term. Lump Sum A Type**|For each of the Termination codes, you will need to specify the Term. Lump Sum A type accordingly as these will print on the INB Payment Summary.  The options available are: **R** – where payment for a genuine redundancy, invalidity or under an approved early retirement scheme.  **T** – where payment was not a payment for a genuine redundancy, invalidity or under an approved early retirement scheme.|  
|**ETP Applicable**|The ETP field is used to identify how the termination payment will be treated.  If the employee is terminated with a code and this field has been selected, the Termination payment is then taxed and treated differently.|

[GoToTop](#how-to-setup-human-resources)

## To setup Qualifications
The Qualifications table is used to set up qualification codes for your employees.  These codes can be used for various employee qualifications: job titles, employee computer skills, education, course, etc.   The table enables you to effectively register and update your employees’ qualifications in other parts of the program.  

1. In the **Search** box, enter **Qualifications**, and then choose the related link.  
2. Fill the fields as described in the following table.  

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|    
|**Code**|Enter in the qualifications code.  You can enter in a maximum of 10 characters, both numbers and letters.|  
|**Description**|Enter in a description for the qualification.|  
|**Qualified Employees**|This field shows whether there are any employees with the qualification specified on the line. A yes indicates that the company has employees with this qualification. To see the employees that have this qualification, click the **ArrowDown**.|  
  
[GoToTop](#how-to-setup-human-resources)
  
## To setup Relatives
The Relatives table is used to set up relative codes for your employees’ relatives.   You can also use this table to set up codes for close contacts to the employee if the employee does not have any family.   

1. In the **Search** box, enter **Relatives**, and then choose the related link.  
2. Fill the fields as described in the following table.  

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|    
|**Code**|Enter in the relatives code.  You can enter in a maximum of 10 characters, both numbers and letters.|  
|**Description**|Enter in a description for the relative.|  
 
 [GoToTop](#how-to-setup-human-resources)
 
## To setup Misc Articles
The Misc. Articles table is used to set up codes for the benefits that you employees receive any other articles that are in your employees’ possession (keys, computers, company cars, etc.) The table enables you to effectively register and update your company’s articles in other parts of the program.   

1. In the **Search** box, enter **Misc. Articles**, and then choose the related link.  
2. Fill the fields as described in the following table.  

|Field Name|Description|
|---------------------------------------------|---------------------------------------------------------------------|  
|**Code**|Enter in the misc. articles code.  You can enter in a maximum of 10 characters, both numbers and letters.|  
|**Description**|Enter in a description for the misc. article.|  
    
[GoToTop](#how-to-setup-human-resources)
