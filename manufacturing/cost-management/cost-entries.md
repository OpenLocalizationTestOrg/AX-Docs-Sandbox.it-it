---
title: Cost entries
description: This article provides information about cost entries and when they are created. A cost entry is a record that registers the quantity and cost of a given event.
author: YuyuScheller
manager: AnnBe
ms.date: 2015-12-07 09 - 09 - 22
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: InventCostOnhandItem
audience: Application User
ms.reviewer: YuyuScheller
ms.search.scope: AX 7.0.0, Operations
ms.custom: 19131
ms.assetid: caf89a9d-71d1-4ff8-9a06-1b1979c9ab6f
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: yuyus
ms.dyn365.ops.intro: Feb-16
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 163dd8dd3f119eef45b9bc6d5313f48ef0adc222
ms.openlocfilehash: 71bfbf4fdcb241fea76b0022d018b4c4cbc07dfb


---

# <a name="cost-entries"></a>Cost entries

This article provides information about cost entries and when they are created. A cost entry is a record that registers the quantity and cost of a given event.

Cost entries are aggregations of inventory transactions that are recorded on active financial inventory dimensions.

## <a name="examples"></a>Examples
### <a name="example-1-no-cost-entries-are-created"></a>Example 1: No cost entries are created

A transfer journal event is registered. The event transfers one piece of item A from location A to location B. The Location inventory dimension isn't considered part of the cost object. Therefore, the event creates two inventory transactions and no cost entries.

### <a name="example-2-cost-entries-are-created"></a>Example 2: Cost entries are created

A transfer journal event is registered. The event transfers one piece of item A from site 1 to site 2. The Site inventory dimension is considered part of the cost object. Therefore, the event creates two inventory transactions and two cost entries.

### <a name="example-3-one-cost-entry-is-created"></a>Example 3: One cost entry is created

A product receipt event is registered for a purchase order. The event registers 100 pieces of item A at a unit cost of 10.00 U.S. dollars (USD). Because item A uses a serial number to track the purpose of inventory management, a unique serial number is created for each item that is received. Therefore, the event creates 100 inventory transactions and one cost entry.

## <a name="cost-entries-page"></a>Cost entries page
The new **Cost entries** page lets you view and control registrations of quantities and costs. This page complements the **Inventory transaction** and **Inventory settlement** pages. Records are registered in chronological order for an event. Therefore, you can quickly find and control the accumulated costs of a specific event or all events that are related to a document. Here is an example:

-   A product receipt event is registered for item A. One hundred pieces are received at a unit cost of 10.00 USD.
-   A few days after the invoice event is registered, the cost increases to 11.00 USD. Therefore, the total amount is 1,100 USD. A second voucher is created to account for the difference of 100 USD.
-   A few days later, a miscellaneous charge of 15.00 USD to cover the transportation cost is registered on the purchase order.

| Voucher | Date       | Reference      | Number | Lot ID  | Reference Lot | Return Lot ID | Quantity | Amount  |
|---------|------------|----------------|--------|---------|---------------|---------------|----------|---------|
| 00001   | 01-01-2015 | Purchase order | 100001 | 0000101 |               |               | 100.00   | 1000.00 |
| 00002   | 20-01-2015 | Purchase order | 100001 | 0000101 |               |               |          | 100.00  |
| 00003   | 31-01-2015 | Adjustment     | 100001 | 0000101 |               |               |          | 15.00   |

The **Cost entries** page enables filtering by document ID and document date. **Note:** Cost entries are available only for [cost objects](cost-object.md) or released products.

<a name="see-also"></a>See also
--------

[Cost objects](cost-object.md)




<!--HONumber=Feb17_HO3-->


