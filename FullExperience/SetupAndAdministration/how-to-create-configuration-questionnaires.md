---
title: "How to: Create Configuration Questionnaires"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "RapidStart Services, setup questionnaires"
  - "setup questionnaires, RapidStart Services"
ms.assetid: d3e4a9bf-cbb1-43a9-bd47-6c885c126dfa
caps.latest.revision: 16
ms.author: "edupont"
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
# How to: Create Configuration Questionnaires
You can use a questionnaire to help you determine the scope and needs of configuration. You can create a new questionnaire, or modify an existing questionnaire by adding new questions or question areas.  
  
 You can create questionnaires for setup\-type tables only. For example you can use the tool to provide information to the following windows:  
  
-   Company Information  
  
-   Fixed Asset Setup  
  
-   General Ledger Setup  
  
-   Inventory Setup  
  
-   Manufacturing Setup  
  
-   Purchases and Payables Setup  
  
-   Marketing Setup  
  
-   Service Setup  
  
-   Sales and Receivables Setup  
  
-   Warehouse Setup  
  
> [!NOTE]  
>  To see a complete list of setup tables, in the **Search** box, enter **Setup**, and then choose the related link. To determine the scope of migration of records data, use migration functionality. For more information, see [Migrate Customer Data](../SetupAndAdministration/migrate-customer-data.md).  
  
### To create a custom configuration questionnaire  
  
1.  In the **Search** box, enter **Configuration Questionnaire**, and choose the related link.  
  
2.  On the **Home** tab, choose **New**. The **Config. Questionnaire** window opens.  
  
3.  Provide a code and description.  
  
4.  On the **Home** tab, in the **Process** group, choose **Questions Areas**. The **Question Areas** window opens.  
  
5.  On the **Home** tab, choose **New**. The **Question Area** window opens.  
  
6.  In the **Code** field, enter a code for the question area.  
  
7.  In the **Table ID** field, choose the ID of the table for which you want to collect information. The **Table Name** field is automatically filled in.  
  
8.  Optionally, in the **Description** field, enter a description. In general, the description should describe the type of information that is being collected.  
  
9. On the **Home** tab, choose **Update Questions**. Each field in the table is added to the questionnaire with a question mark following its label. You can rephrase the label to make it clear how the question should be answered. For example, if a field is called "Name," you could edit it to state "What is the name of \<data being collected\>." You can also provide additional information, for example, prescriptive guidance, in the **Reference** field. You can also use this field to provide a url address of a page that provides additional information.  
  
     As needed, you can also delete questions that you do not want to include in the questionnaire.  
  
    > [!NOTE]  
    >  The **Answer Option** field describes the type and format of the answer of the data that is appropriate. The **Answer** field contains user\-supplied information.  
    >   
    >  As needed, you can also define default answers in the **Answer** field. These values are used by default for custom setup. However, the person filling in the questionnaire can modify and update the answer.  
  
10. Choose the **OK** button to close the window.  
  
11. Repeat these steps to add additional question areas.  
  
12. Choose the **Close** button.  
  
## See Also  
 [How to: Complete the Configuration Questionnaire](../SetupAndAdministration/how-to-complete-the-configuration-questionnaire.md)   
 [Config. Questionnaire](../Topic/\($%20N_8610%20Config.%20Questionnaire%20$\).md)