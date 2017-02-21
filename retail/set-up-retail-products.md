---
title: Set up retail products
description: This article describes how to set up retail products in Microsoft Dynamics 365 for Operations - Retail.
author: josaw1
manager: AnnBe
ms.date: 2015-12-03 22 - 19 - 34
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations
ms.custom: 16181
ms.assetid: c89fee68-6288-479a-9d6b-cb04fa6b1325
ms.search.region: global
ms.search.industry: Retail
ms.author: jeffbl
ms.dyn365.ops.intro: Feb-16
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 163dd8dd3f119eef45b9bc6d5313f48ef0adc222
ms.openlocfilehash: 590fc67bf0abd94cd8a432362f275d03da88be88


---

# <a name="set-up-retail-products"></a>Set up retail products

This article describes how to set up retail products in Microsoft Dynamics 365 for Operations - Retail.

Before you can offer products for resale in your retail channels, you must create and configure the products in Dynamics 365 for Operations AX - Retail. Retail uses the product features in Dynamics 365 for Operations to create organization-wide products in the product master. You can create the products, define the product properties and attributes, and assign the products to retail category hierarchies. To make the products available to your retail channels and add them to an active assortment, you must release the products to the legal entities where they are available. To set up the products that you sell by using retail channels, complete the following tasks.

1.  Define a retail product hierarchy. By using the category hierarchy features in Dynamics 365 for Operations, you can define retail category hierarchies to group and categorize the products that you distribute to your retail channels. User-defined and system attributes can be defined at the category level. Then, all products that are assigned to the category inherit those attributes. Multiple category hierarchies can be defined, and each product can be assigned to multiple hierarchies. However, in a single hierarchy, each product can be assigned to only one category.
2.  Add products and product variants to the product master. Products that are added to the product master represent a global list of products. You can add products manually, one at a time, or you can import product data from your vendors.
3.  Release the products to legal entities. Only products that have been released to legal entities can be made available to your retail channels. When you first define a product, you define it on an organization-wide level. You can then select one or more legal entities to release the product to. The product then becomes available to multiple retail channels across your organization. You can use this functionality to create a product one time, add and update product attributes and properties in one place, and then distribute the product across your organization, to the retail channels where it's available.
4.  Add products to assortments. An assortment represents a collection of products that you offer in your retail channels. You can define one or more assortments, and each product can be assigned to one or more assortments. To assign products to retail channels, you assign the assortments to those retail channels. When you create an assortment, you can add products that haven't yet been released to a legal entity. However, you must release the products to a legal entity before those products can be made available to the retail channels.
5.  Add products to navigation hierarchies. Before products can be browsed online or in point of sale (POS), they must be categorized in a Retail navigation hierarchy.
6.  Add products to catalogs. Although this step is optional for POS, online stores require that products be included in at least one catalog.





<!--HONumber=Feb17_HO3-->


