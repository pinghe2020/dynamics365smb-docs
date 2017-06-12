---
title: "Design Details: Handling Reordering Policies"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "reordering policies"
ms.assetid: ae57c683-824b-4e78-9941-1f4c18a5ccb8
caps.latest.revision: 6
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
# Design Details: Handling Reordering Policies
For an item to participate in supply planning, a reorder policy must be defined. The following four reordering policies exist:  
  
-   Fixed Reorder Qty.  
  
-   Maximum Qty.  
  
-   Order  
  
-   Lot\-for\-Lot  
  
 Fixed Reorder Qty. and Maximum Qty. policies relate to inventory planning. Although inventory planning is technically simpler than the balancing procedure, these policies must coexist with the step\-by\-step balancing of supply and order tracking. To control the integration between the two, and to provide visibility into the involved planning logic, strict principles govern how reordering policies are handled.  
  
## In This Section  
 [Design Details: The Role of the Reorder Point](../ApplicationDesign/design-details-the-role-of-the-reorder-point.md)  
  
 [Design Details: Monitoring the Projected Inventory Level and the Reorder Point](../ApplicationDesign/design-details-monitoring-the-projected-inventory-level-and-the-reorder-point.md)  
  
 [Design Details: The Role of the Time Bucket](../ApplicationDesign/design-details-the-role-of-the-time-bucket.md)  
  
 [Design Details: Staying under the Overflow Level](../ApplicationDesign/design-details-staying-under-the-overflow-level.md)  
  
 [Design Details: Handling Projected Negative Inventory](../ApplicationDesign/design-details-handling-projected-negative-inventory.md)  
  
 [Design Details: Reordering Policies](../ApplicationDesign/design-details-reordering-policies.md)  
  
## See Also  
 [Design Details: Planning Parameters](../ApplicationDesign/design-details-planning-parameters.md)   
 [Design Details: Planning Assignment Table](../ApplicationDesign/design-details-planning-assignment-table.md)   
 [Design Details: Central Concepts of the Planning System](../ApplicationDesign/design-details-central-concepts-of-the-planning-system.md)   
 [Design Details: Balancing Demand and Supply](../ApplicationDesign/design-details-balancing-demand-and-supply.md)   
 [Design Details: Supply Planning](../ApplicationDesign/design-details-supply-planning.md)