---
title: "IRowsetNotifyCP::Fire_OnFieldChange"
ms.custom: na
ms.date: "10/14/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: na
ms.suite: na
ms.technology: 
  - "devlang-cpp"
ms.tgt_pltfrm: na
ms.topic: "article"
f1_keywords: 
  - "Fire_OnFieldChange"
  - "ATL::IRowsetNotifyCP::Fire_OnFieldChange"
  - "ATL.IRowsetNotifyCP.Fire_OnFieldChange"
  - "IRowsetNotifyCP.Fire_OnFieldChange"
  - "IRowsetNotifyCP::Fire_OnFieldChange"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "Fire_OnFieldChange method"
ms.assetid: 03dad058-8d4f-4113-aea4-ef7764eab9ec
caps.latest.revision: 8
ms.author: "mblome"
manager: "ghogen"
translation.priority.ht: 
  - "cs-cz"
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "pl-pl"
  - "pt-br"
  - "ru-ru"
  - "tr-tr"
  - "zh-cn"
  - "zh-tw"
---
# IRowsetNotifyCP::Fire_OnFieldChange
Broadcasts an [OnFieldChange](https://msdn.microsoft.com/en-us/library/ms715961.aspx) event to notify consumers of a change to the value of a column.  
  
## Syntax  
  
```  
  
      HRESULT Fire_OnFieldChange(  
   IRowset* pRowset,  
   HROW hRow,  
   DBORDINAL cColumns,  
   DBORDINAL* rgColumns,  
   DBREASON eReason,  
   DBEVENTPHASE ePhase,  
   BOOL fCantDeny   
);  
```  
  
#### Parameters  
 See [IRowsetNotify::OnFieldChange](https://msdn.microsoft.com/en-us/library/ms715961.aspx) in the *OLE DB Programmer's Reference*.  
  
## Requirements  
 **Header:** atldb.h  
  
## See Also  
 [IRowsetNotifyCP Class](../data/irowsetnotifycp-class.md)