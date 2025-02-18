---
title: "Non-SQL Server Publishers"
description: "Non-SQL Server Publishers"
author: "MashaMSFT"
ms.author: "mathoma"
ms.date: 09/25/2024
ms.service: sql
ms.subservice: replication
ms.topic: conceptual
ms.custom:
  - updatefrequency5
helpviewer_keywords:
  - "heterogeneous database replication, non-SQL Server Publishers"
  - "non-SQL Server Publishers"
  - "heterogeneous data sources, non-SQL Server Publishers"
  - "Publishers [SQL Server replication], Oracle"
---
# Non-SQL Server Publishers  
[!INCLUDE [SQL Server](../../../includes/applies-to-version/sqlserver.md)]

Publishing data from non- [!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)] sources allows you to consolidate data in [!INCLUDE[msCoName](../../../includes/msconame-md.md)] [!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)]. [!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)] can subscribe to snapshot or transactional data published from an Oracle database. For more information about publishing from Oracle, see [Oracle Publishing Overview](../../../relational-databases/replication/non-sql/oracle-publishing-overview.md).  
  
[!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)] supports the following heterogeneous scenarios for transactional and snapshot replication:  
  
-   Publishing data from [!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)] to non-[!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)] Subscribers.  

-   Publishing data to and from Oracle has the following restrictions:  

  |Replication |2016 or earlier |2017 or later |
  |:-----------|:---------------|:-------------|
  |Replication from Oracle |Only support Oracle 10g or earlier |Only support Oracle 10g or earlier |
  |Replication to Oracle |Up to Oracle 12c |Not supported |


 Heterogeneous replication to non-SQL Server subscribers is deprecated. Oracle Publishing is deprecated. To move data, create solutions using change data capture and [!INCLUDE[ssIS](../../../includes/ssis-md.md)].  
  
  
> [!CAUTION]  
>  [!INCLUDE[ssNoteDepFutureAvoid](../../../includes/ssnotedepfutureavoid-md.md)]  
  
 Publishing from non- [!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)] databases is ideal for the following scenarios:  
  
|Scenario|Description|  
|--------------|-----------------|  
|[!INCLUDE[msCoName](../../../includes/msconame-md.md)] .NET Framework application deployments|Develop with [!INCLUDE[msCoName](../../../includes/msconame-md.md)] Visual Studio and [!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)] while operating on data replicated from a non-[!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)] database.|  
|Data warehousing staging servers|Keep [!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)] staging databases synchronized with a non-[!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)] database.|  
|Migration to [!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)]|Test your application in real time against [!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)] while replicating the source system's changes. Switch to [!INCLUDE[ssNoVersion](../../../includes/ssnoversion-md.md)] when satisfied with the migration.|  
  
## Related content

- [Heterogeneous Database Replication](../../../relational-databases/replication/non-sql/heterogeneous-database-replication.md)
