---
title: "Import VAT"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "VAT, import"
ms.assetid: d695878e-fe07-43d5-94fc-b994e34df532
caps.latest.revision: 2
ms.author: "sgroespe"
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
# Import VAT
Import VAT recording presents a situation where you may need to post a document where the entire amount must be treated as VAT. For example, this is necessary, if you receive a VAT invoice from the tax authorities for imported goods.  
  
## Example  
 For example, a company imports goods and posts a purchase invoice \(without VAT\) for LCY 100,000.00. This purchase invoice is posted in the normal way, and the relevant line in the VAT posting setup specifies a VAT% of 0. Later, the company receives a VAT invoice from the tax authorities. The VAT invoice shows a calculated import VAT amount of 25% of the invoice amount \= LCY 25,000.00. When the company pays this VAT invoice, it must be possible to create a VAT ledger entry where the VAT base is 0 and the VAT amount is LCY 25,000.00.  
  
### Setting up the G\/L VAT Account and VAT Posting Setup  
 To record the import VAT, you must set up a new G\/L VAT account, a VAT Product Posting Group, and a corresponding line in the VAT Posting Setup for this purpose. For more information on setting up codes for Import VAT, see [How to: Set Up Codes for Import VAT](../Finance/how-to-set-up-codes-for-import-vat.md).  
  
### Posting the Import VAT using Journals and Invoices  
 To post the Import VAT invoice in the example, you can use a journal or a purchase invoice.  
  
 For more information on posting the Import VAT invoice, see [How to: Post Import VAT](../Finance/how-to-post-import-vat.md) and [How to: Post Import VAT with Purchase Invoices](../Finance/how-to-post-import-vat-with-purchase-invoices.md).  
  
## See Also  
 [Recording VAT](../Finance/recording-vat.md)   
 [How to: Record VAT](../Finance/how-to-record-vat.md)   
 [VAT Reporting and Settlement](../Finance/vat-reporting-and-settlement.md)   
 [How to: Enter VAT\-liable Amounts Without VAT in General Journals](../Finance/how-to-enter-vat-liable-amounts-without-vat-in-general-journals.md)   
 [How to: Set Up and Record Intrastat](../Finance/how-to-set-up-and-record-intrastat.md)   
 [How to: Create a VAT Combination Setup](../Finance/how-to-create-a-vat-combination-setup.md)   
 [How to: View VAT Entries](../Finance/how-to-view-vat-entries.md)