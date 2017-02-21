---
title: Income statement financial report
description: This article describes the default report for income statements. It also describes the building blocks that are associated with this report.
author: twheeloc
manager: AnnBe
ms.date: 2015-11-04 19 - 35 - 20
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.reviewer: annbe
ms.search.scope: AX 7.0.0, Operations
ms.custom: 12294
ms.assetid: 9dd8fcb9-b71a-41e8-b0ea-a0a854604c5a
ms.search.region: Global
ms.author: jcart
ms.dyn365.intro: Feb-16
ms.dyn365.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 2b7f7f6979ca245a01ac65958d07084879fea5c4
ms.openlocfilehash: 480a1aceb6238d878f50f42f7183149c35d8af41


---

# <a name="income-statement-financial-report"></a>Income statement financial report

This article describes the default report for income statements. It also describes the building blocks that are associated with this report. 

<a name="default-income-statement-report"></a>Default income statement report
-------------------------------

| Default report             | What it does                                                                                              |
|----------------------------|-----------------------------------------------------------------------------------------------------------|
| Income Statement – Default | Provides a view of the organization’s profitability for the current period and also for the year to date. |

## <a name="building-blocks"></a>Building blocks
The income statement financial report uses the following building blocks.

| Default report             | Row definition                     | Column definition          |
|----------------------------|------------------------------------|----------------------------|
| Income Statement - Default | Summary Income Statement - Default | Periodic and YTD - Default |

### <a name="row-definition"></a>Row definition

The row definition, Summary Income Statement – Default, contains a section for each part of a traditional income statement. The Main Account Category dimension is used to build this row definition. Therefore, anyone can generate the report without having to make any modifications.

### <a name="column-definition"></a>Column Definition

The column definitions contain different types of columns to provide different levels of detail and financial data.

-   **Periodic and YTD – Default column types:**
    -   **DESC** – The description from the row definition
    -   **FD** – Financial data for the current period
    -   **FD** – Financial data for the year to date

 

<a name="see-also"></a>See also
--------

[Financial reporting](financial-reporting-getting-started.md)

[View financial reports](view-financial-reports.md)

[Dynamics Financial Reportign Blog](http://blogs.msdn.com/b/dynamics_financial_reporting/)




<!--HONumber=Feb17_HO3-->


