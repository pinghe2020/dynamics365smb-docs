---
title: "How to: Print and Reprint G-L Books and VAT Registers"
ms.custom: na
ms.date: "06-05-2016"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "registers, VAT"
  - "registers, printing"
  - "VAT register, print"
  - "registers, general ledger"
  - "general ledger book report, printing"
ms.assetid: c94e157f-cae4-44e5-93d6-bc4a95260169
caps.latest.revision: 9
ms.author: "edupont"
manager: "terryaus"
translation.priority.ht: 
  - "it-it"
---
# How to: Print and Reprint G-L Books and VAT Registers
The tax authorities require that you submit two fiscal reports that list all of the posted ledger entries, the **G\/L Book \- Print** report and the **VAT Register \- Print** report. Each printed page must have its own progressive number, and therefore, you must update [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)] with the last printed page number before you run these reports again.  
  
 The following procedure describes how to print or reprint the **G\/L Book \- Print** report, but the same steps apply to printing or reprinting the **VAT Register \- Print** report.  
  
### To print the general ledger book report  
  
1.  In the **Search** box, enter **G\/L Book \- Print**, and then choose the related link.  
  
2.  Fill in the fields as described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**Report Type**|Select the type of report to create.<br /><br /> If you select **Reprint**, the **From Progressive No.** field becomes enabled.|  
    |**Starting Date**|Enter the first date in the period from which posted entries will be shown.|  
    |**Ending Date**|Enter the last date in the period from which posted entries will be shown.|  
    |**From Progressive No.**|Specifies the progressive number for the report.|  
    |**Print Company Information**|Select to print company information on the report.<br /><br /> The remaining fields are populated based on the **Company Information** window.|  
  
     When you print the report, you will be reminded to update the **General Ledger Setup** window with the page number on the last page.  
  
    > [!IMPORTANT]  
    >  [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)] does not save the page number automatically when you run the reports. After you run the **G\/L Book \- Print** report or the **VAT Register \- Print** report, you must update [!INCLUDE[navnow](../../ApplicationDesign/includes/navnow_md.md)] with the last printed page number.  
  
3.  In the **Search** box, enter **General Ledger Setup**, and then choose the related link.  
  
     To set the last printed page number for the VAT register report, search for **VAT Register**, and choose the link for the window under **VAT Posting Group**.  
  
4.  In the **Fiscal Reporting** FastTab, in the **Last Printed G\/L Book Page** field, specify the page number that is on the last page of the **G\/L Book \- Print** report that you just printed.  
  
 Both official reports can be reprinted. When you reprint a report, the first page of the report must have the same page number as it did when the report was printed the first time. If you want to reprint one of the reports, and the page number is incorrect, you can change the reprinting information for the report  
  
 The following procedure describes how to view or change the page numbering for previously printed versions of the **G\/L Book \- Print** report, but the same steps apply to the **VAT Register \- Print** report.  
  
### To view or change page numbering for reprinting the general ledger book report  
  
1.  In the **Search** box, enter **General Ledger Setup**, and then choose the related link.  
  
2.  On the **Actions** FastTab, in the **Functions** group, choose **Change G\/L Book Reprint Info.**. In the **G\/L Book Reprint Info** window, the **First Page Number** field specifies the first page number of the previously printed reports.  
  
 When you update the **General Ledger Setup** window or the **VAT Registers** window with the page number of the last page of the printed report, make sure that you specify the correct page number. If the reprinted report starts with the wrong page number, the report will not be accepted by the tax authorities. The **G\/L Book Reprint Info** window and the **VAT Register Reprint Info** can help you identify the correct page number.  
  
## See Also  
 [G\-L Book \- Print](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Italy/-$-r_12121-g-l-book-print-$-.md)   
 [VAT Register \- Print](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Italy/-$-r_12120-vat-register-print-$-.md)   
 [G\-L Book Reprint Info](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Italy/-$-n_12149-g-l-book-reprint-info-$-.md)   
 [VAT Register Reprint Info](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Italy/-$-n_12150-vat-register-reprint-info-$-.md)