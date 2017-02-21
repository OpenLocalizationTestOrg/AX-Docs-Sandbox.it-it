---
title: Elimination rules
description: This article provides information about elimination rules and the various options for reporting about eliminations.
author: RobinARH
manager: AnnBe
ms.date: 2015-12-01 17 - 00 - 55
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: LedgerEliminationRule
audience: Application User
ms.reviewer: RobinARH
ms.search.scope: AX 7.0.0, Operations
ms.custom: 13131
ms.assetid: 878ace4c-888d-4dc1-b574-a86efe244fed
ms.search.region: Global
ms.author: aolson
ms.dyn365.intro: Feb-16
ms.dyn365.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 2b7f7f6979ca245a01ac65958d07084879fea5c4
ms.openlocfilehash: ea470298d8649e9dde0c0bfaf444bb9ac81d6c23


---

# <a name="elimination-rules"></a>Elimination rules

This article provides information about elimination rules and the various options for reporting about eliminations.

Elimination transactions are required when a parent legal entity does business with one or more subsidiary legal entities and uses consolidated financial reporting. Consolidated financial statements must include only transactions that occur between the consolidated organization and other entities outside that organizations. Therefore, transactions between legal entities that are part of the same organization must be removed, or eliminated, from the general ledger, so that they don't appear on financial reports. There are multiple ways to report about eliminations:

-   An elimination rule can be created and processed in a consolidation or elimination company.
-   Financial reporting can be used to show the eliminations accounts and dimensions on a specific row or column.
-   A separate legal entity can be used to post manual transaction entries to track eliminations.

This topic focuses on elimination rules that are processed in a consolidation or elimination company. You can set up elimination rules to create elimination transactions in a legal entity that is specified as the destination legal entity for eliminations. This destination legal entity is known as the elimination legal entity. Elimination journals can be generated either during the consolidation process or by using an elimination journal proposal. Before you set up elimination rules, you should become familiar with the following terms:

-   **Source legal entity** – The legal entity where the amounts that are being eliminated were posted.
-   **Destination legal entity** – The legal entity where elimination rules are posted.
-   **Elimination legal entity** – The legal entity that is specified as the destination legal entity for eliminations.
-   **Consolidated legal entity** – The legal entity that is created to report financial results for a group of legal entities. The financial data from the legal entities is consolidated into this legal entity, and then a financial report is created by using the combined data.

The following table shows the types of transactions that might have to be eliminated.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Transaction type</th>
<th>Example</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Sales order entry and invoicing (centralized processing)</td>
<td>You sell a product to a customer on behalf of another legal entity in your organization.</td>
</tr>
<tr class="even">
<td>Sales order entry (intercompany/intracompany) and invoicing</td>
<td>You sell products between legal entities in your organization.</td>
</tr>
<tr class="odd">
<td>Purchase orders (centralized processing)</td>
<td>You purchase inventory, supplies, services, fixed assets, and other products from a vendor on behalf of another legal entity in your organization.</td>
</tr>
<tr class="even">
<td>Inventory management (intercompany/intracompany)</td>
<td><ul>
<li>You transfer one legal entity’s inventory to the fixed assets of another legal entity in your organization.</li>
<li>You transfer one legal entity’s inventory to the inventory of another legal entity in your organization.</li>
</ul></td>
</tr>
<tr class="odd">
<td>In-transit inventory tracking</td>
<td>You transfer items between warehouses in the same legal entity, but across different geographical sites.</td>
</tr>
<tr class="even">
<td>Accounts payable centralized invoice processing</td>
<td>You record an invoice on behalf of another legal entity in your organization.</td>
</tr>
<tr class="odd">
<td>Accounts payable centralized payment processing</td>
<td>You pay an invoice on behalf of another legal entity in your organization.</td>
</tr>
<tr class="even">
<td>Cash management and treasury (centralized processing)</td>
<td><ul>
<li>You process tax payments, tax refunds, interest charges, loans, advances, dividend payments, and prepaid royalties or commissions.</li>
<li>You pay an expense on behalf of another legal entity in your organization. The invoice is entered in the destination legal entity’s books, and you must cross-settle between legal entities. For example, one legal entity pays the expense report of an employee in another legal entity. In this case, the employee’s expense report has expenses that are related to another legal entity.</li>
<li>You transfer cash from one legal entity to another in your organization.</li>
</ul></td>
</tr>
<tr class="odd">
<td>Accounts receivable (centralized processing)</td>
<td>You receive cash for another legal entity’s customer invoice, and you deposit the check into that legal entity’s bank account.</td>
</tr>
<tr class="even">
<td>Payroll (centralized processing, intercompany/intracompany)</td>
<td><ul>
<li>You pay another legal entity’s payroll. For example, a legal entity pays its own payroll for its employees but charges back work that an employee did for another legal entity during that pay run. Or, an employee worked half-time for legal entity A and half-time for legal entity B, and the benefits are across all pay. In these cases, the employee’s pay includes pay from both legal entities. Not only are the salaries posted, but taxes, benefits, deductions, and accruals for salaries are also posted.</li>
<li>You transfer labor from one department or division to another.</li>
</ul></td>
</tr>
<tr class="odd">
<td>Fixed assets (intercompany/intracompany)</td>
<td>You transfer fixed assets to another legal entity’s fixed assets or inventory.</td>
</tr>
<tr class="even">
<td>Allocations (intercompany/intracompany)</td>
<td>You process corporate allocations. Allocations are activities to any account that is allocated, regardless of the originating module.</td>
</tr>
</tbody>
</table>

## <a name="example"></a>Example
Your legal entity, legal entity A, sells widgets to another legal entity in your organization, legal entity B. The following example shows how transactions that occur between the two legal entities might have to be eliminated:

-   Legal entity A sells a widget that costs 10.00 to legal entity B for 10.00.
-   Legal entity A sells a widget that costs 10.00 to legal entity B for 10.00, plus 2.00 in actual shipping costs.
-   Legal entity A sells a widget that costs 10.00 to legal entity B for 15.00 and recognizes a margin on the sale.
-   Legal entity A sells a widget that costs 10.00 to legal entity B for 15.00 and recognizes half the margin on the sale. Legal entity B recognizes the other half of the margin on the sale. Therefore, the revenue is split. Split revenue provides an incentive to order from another legal entity in the organization instead of an external organization.

All these transactions create intercompany transactions that are posted to due-to and due-from accounts. In addition, these transactions might include markup and markdown amounts when the amount of the intercompany sale doesn't equal the cost of the goods that were sold.




<!--HONumber=Feb17_HO3-->


