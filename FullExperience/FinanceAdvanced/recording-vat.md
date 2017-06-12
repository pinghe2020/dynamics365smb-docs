---
title: "Recording VAT"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "VAT, recording"
ms.assetid: 2523e6a0-b946-4305-9d50-392e0e6b8b25
caps.latest.revision: 3
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
# Recording VAT
In EU countries\/regions, every sales and purchase transaction is subject to VAT calculations.  
  
## Calculating and Displaying VAT Amounts in Sales and Purchase Documents  
 You can calculate and display VAT amounts in sales and purchase documents differently depending on the type of customer or vendor that you are dealing with. You can also override the VAT amount calculated by the program to match the VAT amount calculated by your vendor on a given transaction.  
  
### VAT correction  
 It is possible to make corrections to posted VAT entries. This allows you to change the total sales or purchase VAT amounts without changing the VAT base. The feature may be used, for example, if you receive an invoice from a vendor who has calculated VAT incorrectly. For more information on making corrections to posted VAT entries, see [How to: Correct VAT](../Finance/how-to-correct-vat.md).  
  
### Unit Price and Line Amount Including\/Excluding VAT  
 When you select an item in the **No.** field in a sales document, the program also fills in the **Unit Price** field. The unit price is calculated and transferred from either the **Item** card or from the item prices allowed for the item and customer. The program only calculates the **Line Amount** when you enter a quantity for the line.  
  
 In cases where you are selling to retail consumers, you may want your sales document prices to be displayed including VAT both on screen and when printed. To do this, you can select the **Prices Including VAT** check box in the document header.  
  
### Checked and unchecked fields  
 If the **Prices Including VAT** field is selected, the **Unit Price** and **Line Amount** field will be updated to include VAT and the field names will also reflect this.  
  
 If the field is not selected, the program will fill in the **Unit Price** and **Line Amount** field excluding VAT and the field names will reflect this.  
  
### Prices Including VAT Defaults on Customer and Item Cards  
 You can set up the default setting of the **Prices Including VAT** for all sales documents for a customer in the **Prices Including VAT** field on the **Customer** card.  
  
 You can also set up item prices to include or exclude VAT. Normally, item prices contained in the Item Card will be the price excluding VAT. The program uses the information from the **Price Includes VAT** field on the **Item** card to determine the unit price amount for sales documents.  
  
 The following table provides an overview of how the program calculates the unit price amounts for a sales document when you have not set up prices in the **Sales Prices** window:  
  
|**Price Includes VAT field on Item Card**|**Prices Including VAT field in Sales Header**|**Action Performed**|  
|-----------------------------------------------|----------------------------------------------------|--------------------------|  
|No check mark|No check mark|The **Unit Price** on the Item Card is copied to **Unit Price Excl. VAT** field on the sales lines.|  
|No check mark|Check mark|The program calculates the VAT amount per unit and adds to the **Unit Price** on the Item Card. This total Unit Price is then entered in the **Unit Price Incl. VAT field** on the sales lines.|  
|Check mark|No check mark|The program calculates the VAT amount included in the **Unit Price** on the Item Card using the VAT% related to the VAT Bus. Posting Gr. \(Price\) and the VAT Prod. Posting Group combination. The **Unit Price** on the Item Card, reduced by the VAT amount, is then entered in the **Unit Price Excl. VAT** field in the sales lines.|  
|Check mark|Check mark|The **Unit Price** on the Item Card is copied to **Unit Price Incl. VAT** field on the sales lines.|  
  
## See Also  
 [How to: Record VAT](../Finance/how-to-record-vat.md)   
 [Import VAT](../Finance/import-vat.md)   
 [VAT Reporting and Settlement](../Finance/vat-reporting-and-settlement.md)   
 [How to: Enter VAT\-liable Amounts Without VAT in General Journals](../Finance/how-to-enter-vat-liable-amounts-without-vat-in-general-journals.md)   
 [How to: Set Up and Record Intrastat](../Finance/how-to-set-up-and-record-intrastat.md)   
 [How to: Create a VAT Combination Setup](../Finance/how-to-create-a-vat-combination-setup.md)   
 [How to: View VAT Entries](../Finance/how-to-view-vat-entries.md)