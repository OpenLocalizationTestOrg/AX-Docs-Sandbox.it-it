---
title: Posting definitions
description: This article provides information about posting definitions, and how to define and link them. For supported posting types and documents, you can use posting definitions instead of posting profiles to classify main accounts and financial dimensions on accounting entries.
author: twheeloc
manager: AnnBe
ms.date: 2015-12-03 20 - 43 - 23
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: JournalizingDefinition, JournalizingDefinitionTrans, LedgerParameters
audience: Application User
ms.reviewer: annbe
ms.search.scope: AX 7.0.0, Operations
ms.custom: 15741
ms.assetid: ba95c154-6cbf-45b2-b2f0-7eb254429bc3
ms.search.region: Global
ms.author: peakerbl
ms.dyn365.intro: Feb-16
ms.dyn365.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 2b7f7f6979ca245a01ac65958d07084879fea5c4
ms.openlocfilehash: d2787d269a0ce8ccef106f72b7de5bae65161075


---

# <a name="posting-definitions"></a>Posting definitions

This article provides information about posting definitions, and how to define and link them. For supported posting types and documents, you can use posting definitions instead of posting profiles to classify main accounts and financial dimensions on accounting entries.

For supported posting types and documents, you can use posting definitions instead of posting profiles to classify main accounts and financial dimensions on accounting entries. You can view the supported documents and posting types on the **Transaction posting definitions** page. To start using posting definitions, select the **Use posting definitions** option on the **General ledger parameters** page. Even when you use posting definitions, you must still define posting profiles for the originating entries and non-supported posting types and documents. You must use posting definitions in order to enable encumbrance accounting for purchase orders and pre-encumbrance accounting for purchase requisitions.

## <a name="defining-posting-definitions"></a>Defining posting definitions
Use the **Posting definitions** page to specify the match criteria and define the entries that should be generated when a match occurs. The match criteria are evaluated for the originating entries as accounting distributions. On the **Posting definitions** page, you can also assign priority numbers to entry lines to control the order in which the lines are evaluated. The lines that have the lowest priority number are evaluated first. For example, all lines that have a priority of 1 are evaluated, and then lines that have a priority of 2, and so on. When a match is found, the other match criteria are ignored. Additionally, only the criteria in the group that match the originating transaction create generated entries. You can validate your posting definitions by using the **Test posting definition** wizard. After you define a sample originating entry for a posting definition, you'll see the generated entries. You can use posting definition versions together with effective dates. For example, you can create a future version of a posting definition to post to a different ledger account in a new fiscal year. Use the **Transaction posting definitions** page to assign posting definitions to transaction types.

## <a name="linking-posting-definitions"></a>Linking posting definitions
You can link from one posting definition to another when you create posting definitions. The criteria for the definition that you linked to are then considered in addition to the criteria for the current posting definition. This feature helps save you time, because you don't have to reenter criteria on the **Entries** FastTab on the **Posting definitions** page for the current posting definition if you already entered those lines for another definition. In the diagrams or tables, include any links that you might use. To avoid conflicts with the current posting definition, make sure that the lines in any posting definitions that you link to are unique. The following restrictions apply when you create links in posting definitions:

-   A given posting definition can either link to another posting definition or be linked to from another posting definition, but not both. However, a posting definition can link to multiple posting definitions.
-   You can set up links only among posting definitions that are in the same module.
-   You can assign a posting definition to any transaction type, but the transaction type must be in the same module as the posting definition. Use the **Transaction posting definitions** page to see what module a transaction type is in.


<a name="see-also"></a>See also
--------

[Examples: Posting definitions](https://ax.help.dynamics.com/en/?post_type=incsub_wiki&p=74871)




<!--HONumber=Feb17_HO3-->


