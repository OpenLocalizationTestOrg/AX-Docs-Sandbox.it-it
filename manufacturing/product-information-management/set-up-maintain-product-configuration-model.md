---
title: Set up a product configuration model
description: This article describes the steps for setting up and creating a product configuration model.
author: YuyuScheller
manager: AnnBe
ms.date: 2015-09-11 14 - 38 - 59
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: PCProductConfigurationModelListPage
audience: Application User
ms.reviewer: YuyuScheller
ms.search.scope: AX 7.0.0, Operations
ms.custom: 4051
ms.assetid: a58d3ef5-65c5-4b7c-9e19-ca7ce1e83e38
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: yuyus
ms.dyn365.ops.intro: Feb-16
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 163dd8dd3f119eef45b9bc6d5313f48ef0adc222
ms.openlocfilehash: 5d0259962a92521831df217d25aa4ce28f52c66f


---

# <a name="set-up-a-product-configuration-model"></a>Set up a product configuration model

This article describes the steps for setting up and creating a product configuration model.

| Task                                                        | Description                                                                                                                                                                                                                                                                                                                                                                                        |
|-------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Create a product master.                                    | Create a product master from the **Product master** list. Release the product master to all relevant companies. For a product master that is used as a version for a product configuration model or as a subcomponent, **Constraint-based configuration** must be selected as the configuration technology, and the configuration dimension must be selected only for the product dimension group. |
| Create components.                                          | Create components on the **Components** page. Components are the building blocks of a product configuration model and can be reused in multiple product configuration models.                                                                                                                                                                                                                      |
| Create attribute types.                                     | Create attribute types on the **Attribute types** page. Attribute types specify the set of data types for all attributes that are used in product configuration models. Attributes of the **Boolean**, **Text** with a fixed list, and **Integer** with a range types list the set of values that are available when you configure a product variant based on a product configuration model.       |
| Create a product configuration model.                       | Create a product configuration model on the **New product configuration model** page.                                                                                                                                                                                                                                                                                                              |
| Add attributes to a product configuration model.            | Create an attribute on the **Attributes** FastTab on the **Constraint-based product configuration model details** page. Attributes describe the features of the product configuration model.                                                                                                                                                                                                       |
| Add constraints to a product configuration model.           | Create constraints on the **Constraints** FastTab on the **Constraint-based product configuration model details** page. Constraints are limitations that a product configuration must satisfy. Constraints are either expression constraints or table constraints.                                                                                                                                 |
| Add subcomponents to a product configuration model.         | Create subcomponents on the **Subcomponents** FastTab on the **Constraint-based product configuration model details** page. Subcomponents are related to components and are linked to items that represent the subcomponent.                                                                                                                                                                       |
| Add user requirements to a product configuration model.     | User requirements are similar to subcomponents, but they don't reference an item. You can think about user requirements as a phantom BOM. Any BOM lines or route operations that are placed directly under the user requirement will be collapsed into the parent component.                                                                                                                       |
| Add BOM lines to a product configuration model.             | Create BOM lines on the **BOM lines** FastTab on the **Constraint-based product configuration model details** page. BOM lines represent a part that is required to build a variant of the product.                                                                                                                                                                                                 |
| Add route operations to a product configuration model.      | Create route operations on the **Route operations** FastTab on the **Constraint-based product configuration model details** page. Route operations represent a step in a sequence of steps that are performed to make a variant of the product.                                                                                                                                                    |
| Create an active version for a product configuration model. | Create an active version of the product configuration model on the **Versions** page. A version is the relationship between a product configuration model and a product master. A product configuration model that has an active version can be configured from a sales order, sales quotation, purchase order, or production order.                                                               |
| Test a product configuration model.                         | Test the product configuration model from either the **Constraint-based product configuration model details** page or the **Product configuration models list** page. Testing the product configuration models simulates the product model configuration process that occurs during order handling.                                                                                                |
| Create product configuration model template.                | Create a product configuration model template on the **Configuration templates** page. A configuration template includes values for attributes in the product configuration model. Select the attribute values on the **Configure line** page. You can select to load a product model configuration template during product model configuration.                                                   |
| Configure an item.                                          | Product configuration models can be configured from a sales order, sales quotation, purchase order, or production order.                                                                                                                                                                                                                                                                           |






<!--HONumber=Feb17_HO3-->


