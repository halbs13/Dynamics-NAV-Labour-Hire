# How to: setup Resources & Jobs

The Dynamics NAV Labour Hire module comprises and requires various areas within Dynamics NAV
to be configured in order for it to operate. 

These areas include:

- [General Ledger](au-labour-setup-general-ledger.md)
- [Sales & Receivables](au-labour-setup-sales-receivables.md)
- [Resources & Jobs](au-labour-setup-resources-jobs.md)
- [Human Resources](au-labour-setup-human-resources.md)
- [Payroll](au-labour-setup-payroll.md)
- [Labour Hire](au-labour-setup-labour-hire.md)

This section will discuss the following setup areas within Resources & Jobs;

- [Resources Setup](#to-setup-resources)
- [Jobs Setup](#to-setup-jobs)
- [Job Posting Groups](#to-job-posting-groups)

## To setup Resources
YA number series must be setup for Resource records, regardless of whether the number will be manually entered into Dynamics NAV or transferred via the interface.

1. In the **Search** box, enter **Resources Setup**, and then choose the related link.  
2. Fill the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Resources No.**|Select the Resources No. series from the **ArrowDown**. If there is integration with AXiOM, the Employee Numbers will be generated from within AXiOM and transfer into NAV, however this field should still be configured. **Note: The No. Series should be setup first.  You will need to create a new No. series if one does not exist.|  
    |**Time Sheet No.s**|This feature relates specifically to standard time sheets using Resources and Machines and **should not** be confused with Time Sheet Entry used in the Labour Hire module or TimeKeeper.|  
    |**Time Sheet First Week Day**|This feature relates specifically to standard time sheets using Resources and Machines and **should not** be confused with Time Sheet Entry used in the Labour Hire module or TimeKeeper.|  
    |**Time Sheet by Job Approval**|This feature relates specifically to standard time sheets using Resources and Machines and **should not** be confused with Time Sheet Entry used in the Labour Hire module or TimeKeeper.| 
        

## To setup Jobs
A number series must be setup for Job records, regardless of whether the number will be manually entered into Dynamics NAV or transferred via the interface.

1. In the **Search** box, enter **Jobs Setup**, and then choose the related link.  
2. On the **Numbering** FastTab, fill the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Job No.s**|Select the Job No. series from the **ArrowDow**.  If there is integration with AXiOM, the Job Numbers will be generated from within AXiOM and transfer into NAV, however this field should still be configured. **Note: The No. Series should be setup first.  You will need to create a new No. series if one does not exist.|  
       

## To setup Job Posting Groups
Job Posting Groups are used through the Labour Hire module to set defaults such as **Dimensions**, **Payroll Branch and Division** and **Product Posting Groups**.  Where there is integration into the AXiOM product, the Job Posting Group it is transferred across as the **Cost Centre** code which can be later selected on the Order.

1. In the **Search** box, enter **Job Posting Groups**, and then choose the related link.  
2. Complete the fields as described in the following table;

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Code**|Enter in a Code that uniquely identifies the Job Posting Group.  The Code field allows for up to 10 characters but if you are using AXiOM then you must enter in 4 characters.|  
    |**Description**|Enter in a Description which accurately describes the Job Posting Group. ** The description field will be transferred into Cost Centre field within AXiOM.|  
    |**Payroll No.**|Select the **Payroll No.** from the **ArrowDown** which this Job Posting Group transaction belongs to.  The Payroll No. is restricted to 6 characters. |  
    |**Payroll Group**|The Payroll Group field is used to group the Cost Centre codes for selection in AXiOM by transferring to the “Ledger Code”.    Enter in a Code with a maximum of 6 characters.| 
    |**Branch Code**|Select the Branch Code from the “ArrowDown” for this Job Posting Group transaction.|
    |**Division Code**|Select the Division Code from the “ArrowDown” for this Job Posting Group transaction.|
    |**Global Dimensions 1**|Select the Dimension Code from the “ArrowDown” for this Job Posting Group transaction.|
    |**Global Dimensions 2**|Select the Dimension Code from the “ArrowDown” for this Job Posting Group transaction.|
    |**General Product Posting Group**|From the AssistButton button, select the Gen. Prod. Posting Group for this Job Posting Group.|
    |**Exclude from Integration**|This field is used to identify transactions which should no longer be included in the transfer of data to AXiOM.|

3. Additional Dimensions can be setup by click on the **Dimensions** icon.    
4. Complete the fields as described in the following table;

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Dimension Code**|Select the additional dimension you wish to add from the “ArrowDown”.|  
    |**Dimension Value Code**|Select the additional dimension value you wish to add from the “ArrowDown”.|  
    |**Value Posting**|This option is not required at this level and is generally setup and maintained on G/L Accounts. |  
   
