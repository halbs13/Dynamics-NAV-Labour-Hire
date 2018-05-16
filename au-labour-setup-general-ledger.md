# How to setup General Ledger

The Dynamics NAV Labour Hire module comprises and requires various areas within Dynamics NAV
to be configured in order for it to operate. 

These areas include:

- [General Ledger](au-labour-setup-general-ledger.md)
- [Sales & Receivables](au-labour-setup-sales-receivables.md)
- [Resources & Jobs](au-labour-setup-resources-jobs.md)
- [Human Resources](au-labour-setup-human-resources.md)
- [Payroll](au-labour-setup-payroll.md)
- [Labour Hire](au-labour-setup-labour-hire.md)

This section will discuss the setting up General Ledger areas required to operate the Dynamics NAV Labour Hire module at a summarised level as this setup should be undertaken by a user with the appropriate level of Financial Management knowledge.  Some of the areas discussed in this document are;

- [General Ledger Setup](#to-set-up-general-ledger)
- [Dimensions Setup](#to-set-up-dimensions) 

### To set up General Ledger   
1. In the **Search** box, enter **General Ledger Setup**, and then choose the related link.  
2. On the **General** FastTab, fill the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Allow Posting From**|You can restrict posting to the General Ledger at a global level or at a user level. Dates you enter in here will be used at a global level.|  
    |**Allow Posting To**|You can restrict posting to the General Ledger at a global level or at a user level.  Dates you enter in here will be used at a global level.|  
    |**Local Address Format**|.|  
    |**LCY Code**|Enter in the **LCY Code** for this field.|
    |**Local Currency Symbol**|Enter in the **Local Currency Symbol** for this field.|
    |**GST Rounding**|From the **Options**, select **Nearest**.|
    |**Bank Account No.s**|Click on the **ArrowDown** to select the No. Series used to allocate Bank Account No.s.|
    
[GoToTop](#how-to-setup-general-ledger)

## To set up Dimensions
A dimensions is a data that you can add to an entry as a kind of marker so that the program can group entries with similar characteristics and easily retrieve these groups for analysis purposes.  Dimensions can be used throughout the programs on entries in journals and documents, as well as budgets.

The term dimensions is used to describe how analysis occurs.  A two-dimensional analysis, for example, would be Sales Per Area.  However, by using more than two dimensions when creating an entry, you can carry out a more complex analysis at a later time, for example, sales per sales campaign per customer group per area.

Each dimension can have an unlimited series of dimension values that are sub-units of that dimension.  For example, a dimension called Department can have departments called Sales, Administration and so on as sub-units.  These departments are dimension values.  Dimensions and dimension values are user-defined and unlimited, which means you can create dimensions tailored to your company's needs and business processes.  However, some dimensions such as account number and date, are already defined for you by the program.

1. In the **Search** box, enter **Dimension**, and then choose the related link.
2. Fill the fields as described in the following table.


[GoToTop](#how-to-setup-general-ledger)
