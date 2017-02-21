---
title: Update the bank journal composite entity
description: The following steps are needed in order to add the additional BankTransactionType field to the composite BankJournalEntity.
author: twheeloc
manager: AnnBe
ms.date: 2016-10-31 16 - 22 - 18
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User, Developer
ms.search.scope: Operations
ms.custom: 221654
ms.assetid: 9d49f005-bfe9-4b7d-b265-36ba94704f8f
ms.search.region: Global
ms.author: saraschi
ms.dyn365.intro: Nov-16
ms.dyn365.version: Version 1611
translationtype: Human Translation
ms.sourcegitcommit: 2b7f7f6979ca245a01ac65958d07084879fea5c4
ms.openlocfilehash: 9dd32650e46d9f3008fc5147dcfee3494c438880


---

# <a name="update-the-bank-journal-composite-entity"></a>Update the bank journal composite entity

The following steps are needed in order to add the additional BankTransactionType field to the composite BankJournalEntity.

Use the following steps to add the additional BankTransactionType field to the composite BankJournalEntity.

1.  Compile and synchronize the following bank journal composite entities, entities, and staging tables:
    -   Composite Entity\\BankJournalEntity
    -   Entity\\BankJournalHeaderEntity
    -   Entity\\BankJournalLineEntity
    -   Table\\BankJournalHeaderStaging
    -   Table\\BankJournalLineStaging

2.  Data management\\data projects
    -   Expose the **Bank Transaction** type on **Source Data** layout.
        -   Source data format = XML-Element
        -   Entity name = Bank Journal
        -   Upload data file = new version SampleBankJournalCompositeEntity.xml
        -   Click **Yes** to overwrite the existing file.
        -   Click **Yes** to generate mapping from scratch.
        -   Verify that the Bank Transaction Type is mapped.
            -   Click **View map** on Line entity.
            -   Verify that Bank Transaction type is mapped from Source to Staging.

3.  Import the new statement.





<!--HONumber=Feb17_HO3-->


