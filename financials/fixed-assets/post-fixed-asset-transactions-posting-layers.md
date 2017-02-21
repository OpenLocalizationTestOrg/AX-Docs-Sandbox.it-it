---
title: Post fixed asset transactions to posting layers
description: This article gives an overview of posting layer functionality for fixed asset transactions.
author: twheeloc
manager: AnnBe
ms.date: 2015-09-10 20 - 18 - 26
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: AssetBookTable, LedgerJournalTransAsset
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: AX 7.0.0, Operations
ms.custom: 3001
ms.assetid: f626156c-dbbf-4846-9f88-6e3f265cf15e
ms.search.region: Global
ms.author: saraschi
ms.dyn365.intro: Feb-16
ms.dyn365.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 2b7f7f6979ca245a01ac65958d07084879fea5c4
ms.openlocfilehash: 2ec1e8572f88bde31db904ec9112e7b3a4de0b58


---

# <a name="post-fixed-asset-transactions-to-posting-layers"></a>Post fixed asset transactions to posting layers

This article gives an overview of posting layer functionality for fixed asset transactions.

A fixed asset is often depreciated in different ways for different purposes. Depreciation for tax purposes is calculated by current tax rules to achieve the highest possible depreciation before taxes, but depreciation for reporting purposes is calculated according to accounting laws and standards. The various kinds of depreciation are calculated and recorded separately in the posting layers. Each value model that is attached to a fixed asset is set up for a particular posting layer that has an overall depreciation objective. There are three types of posting layers. Current and Operations are used for accounting purposes, and Tax is used for tax depreciation. You can use depreciation books instead of the tax layer, if you prefer. Each journal that you can post depreciations in is defined by its journal name for only one posting layer. The posting layer in the journal cannot be changed, which helps make sure that transactions for each posting layer are kept separate. At least one journal name must be created for each posting layer. You can designate ledger accounts for fixed asset transactions in the Fixed asset posting profiles page. For each posting profile, you must select the relevant transaction type and value model, with the relevant posting layer, and then designate the ledger accounts. If special accounts for tax depreciation are created, they are often put at the end of the chart of accounts and have account numbers that differ from the account numbers for usual business.
| **Note**                                                                                                                                                                                                                                                                                                                                              |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Using derived value models lets you post transactions to different posting layers at the same time. You create the transactions of the primary value model in a journal with the posting layer that corresponds to the value model posting layer. During posting, the derived value model transactions are posted to their respective posting layers. |



<a name="see-also"></a>See also
--------

[Derived value models](https://ax.help.dynamics.com/en/wiki/derived-value-models/)

[Posting with derived value models](https://ax.help.dynamics.com/en/wiki/Posting-with-derived-value-models/)




<!--HONumber=Feb17_HO3-->


