---
title: Order holds
description: This topic describes holds on orders using Retail and commerce in Dynamics AX.
author: josaw1
manager: AnnBe
ms.date: 2016-04-07 19 - 46 - 08
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations
ms.custom: 79132
ms.assetid: 15f04a69-f7ee-4820-bade-f3b11d7a90e4
ms.search.region: global
ms.search.industry: Retail
ms.author: josaw
ms.dyn365.ops.intro: Feb-16
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 163dd8dd3f119eef45b9bc6d5313f48ef0adc222
ms.openlocfilehash: c1d2b2a96ef852e6f08ccc052411236a6cd82595


---

# <a name="order-holds"></a>Order holds

This topic describes holds on orders using Retail and commerce in Dynamics AX.

An order can be put on hold for various reasons. For example, you might put an order on hold until the customer address or payment method can be verified, or until a manager can review the customer’s credit limit. During the sales process, there are times when sales orders must be put on hold. For example, a sales order might be put on hold because of issues with a customer payment, because of suspected fraud, or because a manager must review the order. When a sales order is put on hold, an order hold code is assigned to the sales order to indicate the reason for the hold. Sales order hold codes are configured at **Sales and marketing** &gt; **Setup** &gt; **Sales orders** &gt; **Order holds codes**. A sales order can be put on hold manually at the time of order creation or later. Additionally, an order can be put on hold automatically, based on fraud rules. While a sales order is on hold, you might have to update it with more information. Alternatively, you might want to check out the sales order as you continue to work on it. You can check out a sales order, check it back in, and even override the checkout of another user by using the order hold workbench (**Retail and commerce** &gt; **Customers** &gt; **Order holds**). When an order is ready to be completed, you must remove the hold before you can complete the order process.




<!--HONumber=Feb17_HO3-->


