---
title: Master planning for site coverage, warehouse not mandatory
description: This topic describes how an item that has the site dimension set for coverage is planned.
author: YuyuScheller
manager: AnnBe
ms.date: 2015-09-10 08 - 46 - 21
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: EcoResStorageDimensionGroup, ReqItemTable
audience: Application User
ms.reviewer: YuyuScheller
ms.search.scope: AX 7.0.0, Operations
ms.custom: 2474
ms.assetid: b5987165-4227-4487-8c90-b271d8f39d8e
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: roxanad
ms.dyn365.ops.intro: Feb-16
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 163dd8dd3f119eef45b9bc6d5313f48ef0adc222
ms.openlocfilehash: 2fff3fecc3e2109dbc88751285e786d1fa94141d


---

# <a name="master-planning-for-site-coverage-warehouse-not-mandatory"></a>Master planning for site coverage, warehouse not mandatory

This topic describes how an item that has the site dimension set for coverage is planned.

This master planning scenario involves the following conditions:

-   The site dimension is set to mandatory and must be entered on the demand transaction.
-   The warehouse dimension is not set to mandatory. The warehouse may be known, but it is not used in the master planning calculation.
-   The site dimension is set for coverage planning.
-   The warehouse dimension is not set for coverage planning. Therefore, supply and demand are aggregated by site and, perhaps, other coverage-planned dimensions also.

The following graphic illustrates how master planning proceeds. The parameters that are referred to in the graphic, and their locations, are as follows:
-   Item coverage is defined for the item. Click **Product information management &gt; Products&gt; Released products**. Select the item, and then click **Plan &gt; Item coverage**.
-   Refill relations are defined for the warehouse. Click **Inventory management &gt; Setup &gt; Inventory breakdown &gt; Warehouses**. On the **Master planning** tab, see the **Main warehouse** field group.
-   The default order type is set to Production, Purchase order or Kanban. Click **Product information management &gt; Products&gt; Released products**. Select the item, and then click **Plan &gt; Default order settings**. In the **Default order settings** form, see the **Default order type** field.

![Demand for site coverage warehouse not mandatory](./media/multisitedemandexplosionscenarioforsitecoveragewarehousenotmandatory.jpg)



<a name="see-also"></a>See also
--------

[Master planning and multisite functionality](master-plan-multisite-functionality.md)

[Master planning - site coverage, warehouse mandatory](master-plan-site-coverage-warehouse-mandatory.md)

[Master planning - site and warehouse coverage, warehouse not mandatory](master-plan-site-warehouse-coverage-warehouse-not-mandatory.md)

[Master planning - site and warehouse coverage, warehouse mandatory](master-plan-site-warehouse-coverage-warehouse-mandatory.md)

[Master planning - how the BOM version is determined](master-plan-bom-version-determined.md)




<!--HONumber=Feb17_HO3-->


