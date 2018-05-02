# How to setup Incorporated Companies

This document will contain information relating to the setup of Incorporated Companies and contains the
following sections:

- [Incorporated Company Overview](#incorporated-company-overview)
- [Incorporated Company Flag Identification](#incorporated-company-flag-identification)
- [Company Details](#company-details)
- [Workers Compensation Policies](#workers-compensation-policies)
- [Goods & Services Tax (GST) Overview](#goods-&-services-tax-(gst)-overview)
- [GST Transaction Type Setup](#gst-transaction-type-setup)
- [GST Calculation](#gst-calculation)

## Incorporated Company Overview

Contractors that operate through Incorporated
Companies can be processed through the Labour Hire Suite. These contractors are
maintained and paid using the Payroll system and are setup as per PAYG type
contractors with some differences which will be outlined in this document.

[GoToTop](#how-to-setup-incorporated-companies)

## Incorporated Company Flag Identifications

An “Incorporated Company” option is available as an Employment Basis from within the Employee Type. 

During implementation, all Employee Typecodes are setup and mapped to the appropriate employment basis type. 

To access the Employee Types task, go to thefollowing menu:

*Departments/Payroll/Setup/Payroll Setup/General/Employee Types*

When setting up a new contractor that operates through an Incorporated Company, you must select Employee Type “INCORP” or “Incorporated Company”.

[GoToTop](#how-to-setup-incorporated-companies)
     
## Company Details

The Contractor Company Name and A.B.N fields are located on the Declaration Tab of the Payroll Employee card.

To access the Employee Maintenance task go to the following menu: 

*Departments/Payroll/Employee Maintenance/Payroll Employees*

[GoToTop](#how-to-setup-incorporated-companies)

## Workers Compensation Policies

Contractors operating through Incorporated Companies are required to provide details of their workers compensation policy.

The information that needs to be recorded
includes Policy Number, Insurer and Expiration Date.

Access is via the Payroll Employee card under the Work Cover Tab.

To access the Employee Maintenance task go to the following menu:

*Departments/Payroll/Employee Maintenance/Payroll Employees*

The following fields need to be entered:

 |Field Name | Description
 |--------------------------------------------------------------- | --------------------------------------------------------------|
 |**Workers Comp Policy No.** |The “Workers Comp Policy No.” is used to  record a Contractors policy number.|
 |**Workers Comp Insurer** | The “Workers Comp Insurer” is used to record the name of the Contractors Workers Comp Insurer.|
|**Policy Expiration Policy**|The “Policy Expiration Date” is used to record the expiry date of the policy.|
   

[GoToTop](#how-to-setup-incorporated-companies)
    
## Goods & Services Tax ( GST ) Overview

Where contractors are operating through Incorporated Companies they will not have PAYG Tax deducted but will instead
have GST calculated and added to their payment.

On the TaxTab in the Employee Card – the Tax Scale No. should be changed to GST.

To access the Employee Maintenance task go to the following menu: 

*Departments/Payroll/Employee Maintenance/Payroll Employees*

[GoToTop](#how-to-setup-incorporated-companies)

## GST Transaction Type Setup

A Transaction Code must be setup to represent GST. This code will be used in conjunction with the GST Tax scale when
calculating contractor pays.

GST Accumulation Type and Accumulation Summary Type options are used when setting up the GST transaction code to
separate it from PAYG Tax.

To access the Pay Transaction Types task go to the following menu: 

*Departments/Payroll/Setup/Payroll Setup/General/Pay Transaction Types*

The GST Product Posting Group field is used to reconcile the General Ledger Account used for GST. This is the only
transaction type that will be setup with a GST Product Posting Group instead of a transaction posting group.

[GoToTop](#how-to-setup-incorporated-companies)

## GST Calculation

On the Pay Transaction Type setup card on the Parameters Tab, there is a GST applicable box that should be ticked for every code that should have GST applied. For wages type code, GST would apply, whereas for a reimbursement type code, GST may not apply.

To access the Pay Transaction Types task go to the following menu: 

*Departments/Payroll/Setup/Payroll Setup/General/Pay Transaction Types*

GST needs to be setup on the Payroll Control card and mapped to GST Tax Tran Type
 
To access the Payroll Control Setup task go to the following menu: 

*Departments/Payroll/Setup/Payroll Setup/Payroll Controls/Payroll Setup*


 [GoToTop](#how-to-setup-incorporated-companies)


