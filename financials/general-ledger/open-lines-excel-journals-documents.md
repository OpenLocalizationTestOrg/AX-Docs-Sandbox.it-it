---
title: Publish journal lines and documents from Excel
description: This topic explains how to enter and publish lines for general journals from Microsoft Excel. It includes information about the various templates that you can use, depending on the type of transactions that you&quot;re entering.
author: twheeloc
manager: AnnBe
ms.date: 2016-03-08 17 - 50 - 05
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: LedgerJournalTable
audience: Application User
ms.search.scope: AX 7.0.0, Operations
ms.custom: 62213
ms.assetid: 791c90c6-faf1-4c63-9a4c-614a284e332a
ms.search.region: Global
ms.author: kweekley
ms.dyn365.intro: Feb-16
ms.dyn365.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 2b7f7f6979ca245a01ac65958d07084879fea5c4
ms.openlocfilehash: 1107989007b3ef8b5e15e92443e9fdff996e1ab3


---

# <a name="publish-journal-lines-and-documents-from-excel"></a>Publish journal lines and documents from Excel

This topic explains how to enter and publish lines for general journals from Microsoft Excel. It includes information about the various templates that you can use, depending on the type of transactions that you're entering.

Users can enter and publish lines for financial journals from Microsoft Excel. After a user creates a journal, the **Open lines in Excel** button displays the templates that are available. Templates are designed to support specific scenarios, however not every combination of account type is supported in the journal. The following table shows the templates that are available and the account types which they support.
|                          |                                                                                                                         |                                                                                         |
|--------------------------|-------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------|
| **Template**             | **Supported account types**                                                                                             | **How to access the template**                                                          |
| Ledger journal lines     | Account: Ledger, Customer, Vendor, Bank Offset account: Ledger, Customer, Vendor, Bank Intercompany is supported.       | General journal                                                                         |
| Invoice register         | Account: Vendor Offset account: Ledger Intercompany isn't supported.                                                    | AP invoice register                                                                     |
| Invoice journal          | Accounts: Vendor Offset account: Ledger Intercompany is supported.                                                      | AP invoice journal                                                                      |
| Vendor invoice           |                                                                                                                         | Vendor invoice                                                                          |
| Customer invoice journal | Account: Customer Offset account: Ledger Intercompany is supported.                                                     | General journal                                                                         |
| Free text invoice        |                                                                                                                         | On the **Free text invoice** page, click **Open in Excel** (the Microsoft Office icon). |
| Fixed assets journal     | Asset to ledger, bank, customer, or vendor. Intercompany isn't supported.                                               | Fixed asset journal                                                                     |
| Vendor payment journal   | Account: Vendor Offset account: Ledger, Bank Intercompany is supported.                                                 | Vendor payment journal                                                                  |
| Customer payment journal | Account: Customer Offset account: Ledger, Bank Intercompany is supported.                                               | Customer payment journal                                                                |
| Project expense journal  | Account: Project, Ledger, Customer, Vendor Offset account: Project, Ledger, Customer, Vendor Intercompany is supported. | General journal Expense (under Project management and accounting)                       |

When the lines are published, they are validated to make sure that they comply with the rules that are set up in the financial journals. After the lines are published, users can edit or post the vouchers from Microsoft Dynamics 365 for Operations. To add financial dimensions to a template, additional changes are required. For additional information, see [Add dimensions to the Microsoft Excel template](dimensions-overview.md). After dimensions are added to the entity, they are available in the Excel designer and can be added to the template.

<a name="see-also"></a>See also
--------

[Dimensions in Excel](dimensions-overview.md)




<!--HONumber=Feb17_HO3-->


