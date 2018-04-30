# How to: Setup EFT

The Dynamics NAV Labour Hire module comprises and requires various areas within Dynamics NAV
to be configured in order for it to operate. 

These areas include:

- [General Ledger](au-labour-setup-general-ledger.md)
- [Sales & Receivables](au-labour-setup-sales-receivables.md)
- [Resources & Jobs](au-labour-setup-resources-jobs.md)
- [Human Resources](au-labour-setup-human-resources.md)
- [Payroll](au-labour-setup-payroll.md)
- [Labour Hire](au-labour-setup-labour-hire.md)

This section will discuss the setting up EFT to produce the appropriate files.

### To set up EFT   
1. In the **Search** box, enter **Bank Accounts**, and then choose the related link.  
2. On the **General** FastTab, fill the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**No.**|Enter in a No. for the Bank Account.|  
    |**Name**|Enter in a Name for the Bank Account.|  
    |**Address**|If your bank account has an Address, make sure that the **Country/Region Code** field is filled.|  
    |**Address2**|If the Bank Account Address doesn't fit into the first field, then this field can be used to record additonal information.|
    |**Post Code & City**|Completethe Post Code & City.|
    |**State**|Complete the State.|
    |**Country/Region Code**|Complete the Country & Region Code.|
    |**Phone No.**|Complete the Phone No. field, if known.|
    |**Contact**|Complete the Contact field, if known.|
    |**Bank Branch No.**|Complete the Bank Branch No. of where the Bank Account is held.|
    |**Bank Account No.**|Complete the Bank Account No. of the Bank Account.|
    
3. On the **Posting** FastTab, fill the fields as described in the following table.

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Bank Acc. Posting Group**|The **Bank Account Posting Group** field is used to identify where the entries will post to in the General Ledger.  Complete the Bank Acc. Posting Group that relates to this Bank Account.|  
    
 4. On the **Transfer** FastTab, fill the fields as described in the following table.

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**EFT Bank Code**|Complete the Bank Code of your Banking Institution.|
    |**EFT BSB No.**|The value in this field will populate with information entered on the **General** FastTab.|
    |**EFT Security No.**| Complete the EFT Security No.  This information is exported into the EFT file you generated.  It is usually known as the **User ID No.** in the EFT file.|
    |**EFT Bank Code**|Enter in the EFT Bank Code for the file being produced.  **53** is the number that is required on the file to the bank as this indentifies to the Bank that the file is a **Salary & Wages** file and will therefore be released accordingly.|
    |**EFT Balancing Record Required**|Select this field if a Balancing Record is required on the EFT file.  Confirmation from your Banking Institution may be required.|
    
