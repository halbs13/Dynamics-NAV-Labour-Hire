# How to setup Labour Hire

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

- [Labour Hire Setup](#to-setup-labour-hire)
- [Rate Frequency Conversion](#to-setup-rate-frequency-conversion)
- [Fee Types](#to-setup-fee-types) 
- [Placement Types](#to-setup-placement-types) 
- [Interface Options](#to-setup-interface-options) 
- [Interface Defaults](#to-setup-interface-defaults) 

## To setup Labour Hire
You use the Labour Hire Setup to establish certain basic rules to be used in the Labour Hire application area.

1. In the **Search** box, enter **Labour Hire Setup**, and then choose the related link.  
2. On the **General** FastTab, fill the fields as described in the following table. 

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Job Contract Posting Method**|This option defines when invoices can be generated once timesheets are processed.  The options available are; **Payroll** – if this option is selected then sales invoices will be available for generation once Payroll has been processed and posted. **Timesheet** – if this option is selected then sales invoices will be available for generation once Timesheets have processed to payroll.|  
    |**Placement No.s**|The Placement No.s are used to allocate Placement No.s when using the Placement Entry screen. Select the Placement No.s from the **ArrowDown**. This option is not used if there is integration to Axiom.|  
    |**Use Interface**|The **Use Interface** field if selected, can be used to restrict fields being updated in various tables within NAV as defined in the Interface Options table.|  
    |**Escalation Time**|This field is used to determine the duration of the initial escalation time used for notifications when using the TimeKeeper application.| 
   
3. On the **Permanent Placement** FastTab, fill the fields as described in the following table. 

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**No. Days/Weeks To Calculate Invoice Generation Date**|The **No. Days/Weeks To Calculate Invoice Generation Date** field is used to define when Permanent Placement invoices are to be generated.|  
     |**Days/Week**|The **Days/Weeks** field is used to define if Permanent Placement invoices are generated days or weeks after the Permanent Placement.| 
     |**Start/Create Date**|The **Start/Create Date** field is used to define if Permanent Placement invoices are generated from the Start Date or Creation Date of the Permanent Placement.|  
     |**Before/After**|The **Before/After** field is used to define if Permanent Placement invoices are generated Before or After the date of the Permanent Placement.|
     |**Placement Flat Fee Type Code**|The **Placement Flat Fee Type Code** field is used to define the GL account the Placement Flat Fees will be posted to.| 
     |**Plcmt. Salary % Fee Type Code**|The **Plcmt. Salary % Fee Type Code** field is used to define the GL account the Placement Salary % Fee will be posted to.|  
     
4. On the **Timesheet** FastTab, fill the fields as described in the following table. 

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Automatic Timesheet Line**|The **Automatic Timesheet Line** check box is used to define if timesheets are automatically generated when payrolls are posted and pay periods are closed.|  
     |**Timesheet Unit Validation**|The Timesheet Unit Validation feature is used to define the number of hours worked on a daily basis. It is generally used for reporting to clients or for internal reasons that allows your organisation to record the number of hours an employee works on a daily basis. The “Timesheet Unit Validation” check box is used to define if timesheet unit validation is required.| 
     |**Dup. Timesheet Check Frequency**|The **Dup. Timesheet Check Frequency** defines the frequency of when duplicate timesheets are checked. The options available are; Weekly or Daily. Duplicate timesheets are checked based on the following; * Alternate Date or Pay Period End Date * Transaction Type|  
     
5. On the **Invoicing** FastTab, fill the fields as described in the following table. 

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Default Job Invoice Grouping**|The **Default Job Invoice Grouping** field is used to define how invoices will be generated. The options available are; **Blank**,  **Alternate Date** – if you select this option then invoices will be grouped by Alternate Date when generated.  **Job Posting Group** – if you select this option then invoices will be grouped by Job Posting Group when generated. **Job Bill-To Contact** – if you select this option then invoices will be grouped by Job Bill-To Contact when generated. **Job No.** – if you select this option then invoices will be grouped by Job No. when generated. **Job Task No.** – if you select this option then invoices will be grouped by Job Task No. when generated.|  
                                                                              [GoToTop](#how-to-setup-labour-hire)
    
         
## To setup Rate Frequency Conversion
The Rate Frequency Conversion window is used to establish one or more different type of rate frequencies used on Order Rate Sets.

The Rate Frequency Conversion factors are generally used when Placement Entry is being used.

1. In the **Search** box, enter **Rate Frequency Conversion**, and then choose the related link.  
2. Fill the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Frequency**|Select the **Frequency** type from the **ArrowDown**. The options available are; **Hour, **Day, **Week, **Month, **Unit.**|  
    |**Hourly Conversion Rate**|Enter in the value to convert the hourly rate.|  
    |**Maximum**|Enter in the maximum number of units.|  
    |**Unit of Measure Code**|You can select the Unit of Measure code from the **ArrowDown**.| 
 
## To setup Fee Types
The Fee Types window is used to establish the Fee Types that are used within your organisation. An example of how this might be used is where you have Permanent Placement Fee overhead charges such as setup fees which can be mapped through to a relevant General Ledger account.

1. In the **Search** box, enter **Fee Types**, and then choose the related link.  
2. Fill the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Code**|Select the “Fee Type” Code from the “ArrowDown”.|  
    |**Description**|Enter in a Description to describe the Fee Type.| 
    |**Fee Type**|Enter in the Fee Type. The options available are; **Placement**, **Requirement.**|
    |**G/L Account No.**|Enter in the GL account number where the placement fee type value will post to in the General Ledger.|

## To setup Placement Types
The Placement Types window is used to set up codes for each set of Placement Types you process within your organisation.

1. In the **Search** box, enter **Placement Type**, and then choose the related link.  
2. Fill the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Code**|Enter in a Placement Type. You can enter a maximum of 10 characters, both numbers and letters.|  
    |**Description**|Enter in the text that describes the Placement Type.|  
    |**Placement Category**|Enter in the Placement Category which describes the Placement Type. The options available are; **Permanent, **Contractor.**|  
    |**Exclude from Integration**|The **Exclude from Integration** field is used to identify whether this transaction will be excluded from the integration to Axiom.|
    
## To setup Interface Options
The Interface Options window is used to specify the integration behavior between NAV and Axiom and NAV and TimeKeeper.  

1. In the **Search** box, enter **Interface Options**, and then choose the related link.  
2. On the **Integration** FastTab, fill the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Code**|Enter in the qualifications code.  You can enter in a maximum of 10 characters, both numbers and letters.|  
    |**Description**|Enter in a description for the qualification.|  
    |**Qualified Employees**|This field shows whether there are any employees with the qualification specified on the line. A yes indicates that the company has employees with this qualification. To see the employees that have this qualification, click the AssistButton to the right of the field.|  
  
  ## To setup Relatives
The Relatives table is used to set up relative codes for your employees’ relatives.   You can also use this table to set up codes for close contacts to the employee if the employee does not have any family.   

1. In the **Search** box, enter **Relatives**, and then choose the related link.  
2. Fill the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Code**|Enter in the relatives code.  You can enter in a maximum of 10 characters, both numbers and letters.|  
    |**Description**|Enter in a description for the relative.|  
 
 ## To setup Misc. Articles
The Misc. Articles table is used to set up codes for the benefits that you employees receive any other articles that are in your employees’ possession (keys, computers, company cars, etc.) The table enables you to effectively register and update your company’s articles in other parts of the program.   

1. In the **Search** box, enter **Mics. Articles**, and then choose the related link.  
2. Fill the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Code**|Enter in the misc. articles code.  You can enter in a maximum of 10 characters, both numbers and letters.|  
    |**Description**|Enter in a description for the misc. article.|  
  
