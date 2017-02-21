---
title: Production order cost estimation
description: This article provides information about production cost estimation. Production cost estimation provides the projected material and capacity consumption costs of producing an item in the planned production order quantity.
author: YuyuScheller
manager: AnnBe
ms.date: 2016-04-12 16 - 06 - 35
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: BOMCalcTrans, InventCostTrans, ProdCalcTrans, ProdTableJour, ProdTableListPage
audience: Application User
ms.search.scope: AX 7.0.0, Operations
ms.custom: 80633
ms.assetid: fcc154aa-6f50-4911-b4a5-0ff5f2955b03
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: mguada
ms.dyn365.ops.intro: Feb-16
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 163dd8dd3f119eef45b9bc6d5313f48ef0adc222
ms.openlocfilehash: 597ac8b9547f9da4302a740bc96230a7beaf9eb9


---

# <a name="production-order-cost-estimation"></a>Production order cost estimation

This article provides information about production cost estimation. Production cost estimation provides the projected material and capacity consumption costs of producing an item in the planned production order quantity. 

After you create a production order, you must estimate production costs. The purpose is to estimate item and route consumption for the production process, because these estimates are used as the basis for subsequent scheduling and production processes.

## <a name="production-cost-estimation"></a>Production cost estimation
Estimates of production costs are based on the following information:

-   The quantity on the production order
-   The components on the production bills of materials (BOMs)
-   The routing operations in the production route
-   The indirect costs that apply to the components and operations
-   The active cost data as of the calculation date

If there is a phantom line item on the production BOMs, the calculations reflect the phantom’s components and route operations. You can use the estimation task to recalculate estimated costs so that they reflect updated information. For example, the updated information might be changes to the quantity on the production order, the components on the production BOMs, the routing operations in the production route, the indirect costs that apply to these components and operations, or the active cost data as of the recalculation date. The calculations of estimated cost also suggest a sales price for the production item, based on a cost-plus-markup approach. The calculations of estimated cost can optionally apply to reference orders that reflect other production orders that are linked to the production order.

## <a name="view-the-estimated-costs"></a>View the estimated costs
After you run estimation, you can view the results on the **Price calculation** page. The estimation calculates the following values:

-   **Production cost** – The production cost is the top line of the estimate. It shows the complete cost of running the production order and the total sales price for the production. It's the sum of all the cost lines on the estimate.
-   **Route or resource costs** – Route or resource costs are the costs for the production operations. They include the cost of elements such as setup time, run time, and overhead.
-   **Material costs** – Material costs are the costs and prices of the BOM components that are required in order to produce the item. These costs have previously been established and entered into the system.

## <a name="other-uses-of-cost-estimation"></a>Other uses of cost estimation
A cost estimate also provides the following information:

-   Meaningful price quotations
-   Estimates of the profitability of the order
-   Estimates of raw material usage
-   Comparisons of cost information from previous productions
-   Budget and forecasting information
-   Estimates of the production size that is required in order to maintain a particular cost





<!--HONumber=Feb17_HO3-->


