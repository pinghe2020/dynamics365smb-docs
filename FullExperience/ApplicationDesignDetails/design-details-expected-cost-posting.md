---
title: "Design Details: Expected Cost Posting"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "posting, expected costs"
  - "costs, expected"
ms.assetid: 792412fe-7c40-4408-8fe3-a14f3a9a711b
caps.latest.revision: 8
ms.author: "sgroespe"
manager: "terryaus"
translation.priority.ht: 
  - "da-dk"
  - "de-at"
  - "de-ch"
  - "de-de"
  - "en-au"
  - "en-ca"
  - "en-gb"
  - "en-in"
  - "en-nz"
  - "es-es"
  - "es-mx"
  - "fi-fi"
  - "fr-be"
  - "fr-ca"
  - "fr-ch"
  - "fr-fr"
  - "is-is"
  - "it-ch"
  - "it-it"
  - "nb-no"
  - "nl-be"
  - "nl-nl"
  - "ru-ru"
  - "sv-se"
---
# Design Details: Expected Cost Posting
Expected costs represent the estimation of, for example, a purchased item’s cost that you record before you receive the invoice for the item.  
  
 You can post expected cost to inventory and to the general ledger. When you post a quantity that is only received or shipped but not invoiced, then a value entry is created with the expected cost. This expected cost affects the inventory value, but is not posted to the general ledger unless you set up the system up to do so.  
  
> [!NOTE]  
>  Expected costs are only managed for item transactions. Expected costs are not for immaterial transaction types, such as capacity and item charges.  
  
 If only the quantity part of an inventory increase has been posted, then the inventory value in the general ledger does not change unless you have selected the **Expected Cost Posting to G\/L** check box in the **Inventory Setup** window. In that case, the expected cost is posted to interim accounts at the time of receipt. After the receipt has been fully invoiced, the interim accounts are then balanced and the actual cost is posted to the inventory account.  
  
 To support reconciliation and traceability work, the invoiced value entry shows the expected cost amount that has been posted to balance the interim accounts.  
  
## Example  
 The following example shows expected cost if the **Automatic Cost Posting** check box and the **Expected Cost Posting to G\/L** check box are selected in the **Inventory Setup** window.  
  
 You post a purchase order as received. The expected cost is LCY 95.00.  
  
 **Value Entries**  
  
|Posting Date|Entry Type|Cost Amount \(Expected\)|Expected Cost Posted to G\/L|Expected Cost|Item Ledger Entry No.|Entry No.|  
|------------------|----------------|------------------------------|----------------------------------|-------------------|---------------------------|---------------|  
|01\-01\-20|Direct Cost|95.00|95.00|Yes|1|1|  
  
 **Relation Entries in the G\/L – Item Ledger Relation Table**  
  
|G\/L Entry No.|Value Entry No.|G\/L Register No.|  
|--------------------|---------------------|-----------------------|  
|1|1|1|  
|2|1|1|  
  
 **General Ledger Entries**  
  
|Posting Date|G\/L Account|Account No. \(En\-US Demo\)|Amount|Entry No.|  
|------------------|------------------|---------------------------------|------------|---------------|  
|01\-01\-20|Inventory Accrual Account \(Interim\)|5530|\-95.00|2|  
|01\-01\-20|Inventory Account \(Interim\)|2131|95.00|1|  
  
 At a later date, you post the purchase order as invoiced. The invoiced cost is LCY 100.00.  
  
 **Value Entries**  
  
|Posting Date|Cost Amount \(Actual\)|Cost Amount \(Expected\)|Cost Posted to G\/L|Expected Cost|Item Ledger Entry No.|Entry No.|  
|------------------|----------------------------|------------------------------|-------------------------|-------------------|---------------------------|---------------|  
|01\-15\-20|100.00|\-95.00|100.00|No|1|2|  
  
 **Relation Entries in the G\/L – Item Ledger Relation Table**  
  
|G\/L Entry No.|Value Entry No.|G\/L Register No.|  
|--------------------|---------------------|-----------------------|  
|3|2|2|  
|4|2|2|  
|5|2|2|  
|6|2|2|  
  
 **General Ledger Entries**  
  
|Posting Date|G\/L Account|Account No. \(En\-US Demo\)|Amount|Entry No.|  
|------------------|------------------|---------------------------------|------------|---------------|  
|01\-15\-20|Inventory Accrual Account \(Interim\)|5530|95.00|4|  
|01\-15\-20|Inventory Account \(Interim\)|2131|\-95.00|3|  
|01\-15\-20|Direct Cost Applied Account|7291|\-100|6|  
|01\-15\-20|Inventory Account|2130|100|5|  
  
## See Also  
 [Design Details: Inventory Costing](../ApplicationDesign/design-details-inventory-costing.md)   
 [Design Details: Cost Adjustment](../ApplicationDesign/design-details-cost-adjustment.md)   
 [Design Details: Reconciliation with the General Ledger](../ApplicationDesign/design-details-reconciliation-with-the-general-ledger.md)   
 [Design Details: Inventory Posting](../ApplicationDesign/design-details-inventory-posting.md)   
 [Design Details: Variance](../ApplicationDesign/design-details-variance.md)