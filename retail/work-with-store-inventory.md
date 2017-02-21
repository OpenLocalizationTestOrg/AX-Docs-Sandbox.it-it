---
title: Manage store inventory
description: This article describes the types of documents that you can use to manage inventory.
author: josaw1
manager: AnnBe
ms.date: 2015-12-09 18 - 39 - 11
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations
ms.custom: 21391
ms.assetid: 1a990296-9f8b-40e5-8c30-def0d7f280e9
ms.search.region: global
ms.search.industry: Retail
ms.author: rubendel
ms.dyn365.ops.intro: Feb-16
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 163dd8dd3f119eef45b9bc6d5313f48ef0adc222
ms.openlocfilehash: c481c67a0172e244f76c17a62f0237e71ec0c985


---

# <a name="manage-store-inventory"></a>Manage store inventory

This article describes the types of documents that you can use to manage inventory.

You can use the following types of documents to manage your organization's inventory.

## <a name="purchase-orders"></a>Purchase orders
Purchase orders are created at the head office. If a retail warehouse is included in the purchase order header, the order can be received at the store by using Modern POS (MPOS) or Cloud POS in Microsoft Dynamics 365 for Operations - Retail. After the quantities that are received at the store are entered, they can be saved locally for additional modification. Alternatively, the quantities can be committed and sent to the head office. At the head office, the quantities that were received at the store are displayed in Dynamics 365 for Operations, in the **Receive now** field on the purchase order.
Transfer orders
---------------

A transfer order can specify that a particular store is a location that items can be shipped from. In this case, the transfer order appears at the store as a picking request in MPOS or Cloud POS. After the quantities that are requested are picked, they are committed and sent to the head office. At the head office, the quantities that were picked at the store are displayed in Dynamics 365 for Operations, in the **Ship now** field on the transfer order. A transfer order may specify that a particular store is a location that items can be shipped to. In this case, the transfer order appears at the store as a receiving request in MPOS or Cloud POS. After the quantities that are received at the store are entered, they can be saved locally for additional modification. Alternatively, the quantities can be committed and sent to the head office. At the head office, the quantities that were received at the store are displayed in Dynamics 365 for Operations, in the **Receive now** field on the transfer order.

## <a name="stock-counts"></a>Stock counts
Stock counts can be either scheduled or unscheduled. Scheduled stock counts are initiated at the head office, which specifies the items that must be counted. The head office creates a counting document that can be received at the store, where the quantities of actual on-hand stock are entered in MPOS or Cloud POS. Unscheduled stock counts are initiated at a store, and the quantities of actual on-hand stock are updated in either MPOS or Cloud POS. Unlike scheduled stock counts, unscheduled stock counts do not have a predefined list of items. When a stock count of either type is completed, it is committed and sent to the head office. At the head office, the count is validated and posted.






<!--HONumber=Feb17_HO3-->


