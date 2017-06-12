---
title: "How to: Set Up Bank Reference Files"
ms.custom: na
ms.date: "06-05-2016"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "bank reference files"
ms.assetid: a49775c0-1323-44cb-8b94-f507767f929c
caps.latest.revision: 3
ms.author: "edupont"
translation.priority.ht: 
  - "fi-fi"
---
# How to: Set Up Bank Reference Files
To process electronic payments, you must first set up bank reference files to determine how payment data should be imported or exported.  
  
### To set up a bank reference file  
  
1.  In the **Search** box, enter **Bank Reference File Setup**, and then choose the related link.  
  
2.  On the **General** FastTab, fill in the fields as described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**No.**|Specifies a bank account code.|  
    |**Export Reference Payments**|Enter the full path of the payment file to export.|  
    |**Import Reference Payments**|Enter the full path of the payment file to import.|  
    |**Currency Exchange Rate File**|Enter the full path of the currency exchange rate file.|  
    |**Inform. of Appl. Cr. Memos**|Select to display credits applied to invoices on the payment recipient's account statement.|  
  
3.  On the **Foreign Payments** FastTab, fill in the fields as described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**Export Foreign Payments**|Enter the full path of the payment file to export to foreign banks.|  
    |**Due Date Handling**|Select how due date processing should be applied to foreign payments.<br /><br /> **Batch** – All payments in the file receive the same payment date.<br /><br /> –or–<br /><br /> **Transaction** – Each payment in the file receives a transaction\-specific payment date. Contact your bank to determine whether this setting should be used.|  
    |**Default Service Fee Code**|Select a default service fee code for foreign banks.|  
    |**Default Payment Method**|Select a default payment method for foreign payments.|  
    |**Exchange Rate Contract No.**|Enter the exchange rate contract number.|  
    |**Allow Comb. Foreign Pmts.**|Select to combine all foreign payments made to one recipient in one day from the same bank account.|  
  
4.  On the **SEPA** FastTab, fill in the fields as described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**Bank Party ID**|Enter a SEPA bank party ID. **Note:**  This field is only used for the SEPA pain.001.001.02 standard.|  
    |**File Name**|Enter the full path of the SEPA payment file. **Note:**  This field is only used for the SEPA pain.001.001.02 standard.|  
  
    > [!IMPORTANT]  
    >  To export vendor payments using the SEPA standard, you must fill the **Payment Export Format** field in the **Bank Account Card** window.  
  
5.  Choose the **OK** button.  
  
## See Also  
 [Payment Export Format](assetId:///0bd91b95-8ee0-4c8f-90b6-c78248849896)   
 [Electronic Banking in Finland](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Finland/electronic-banking-in-finland.md)   
 [How to: Generate Payment Files](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Finland/how-to-generate-payment-files.md)   
 [How to: Disregard Payment Discounts](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Finland/how-to-disregard-payment-discounts.md)   
 [Reference File Setup](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Finland/-$-t_32000000-reference-file-setup-$-.md)