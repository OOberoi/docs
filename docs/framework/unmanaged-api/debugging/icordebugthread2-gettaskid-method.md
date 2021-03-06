---
title: "ICorDebugThread2::GetTaskID Method | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-clr"
ms.tgt_pltfrm: ""
ms.topic: "reference"
apiname: 
  - "ICorDebugThread2.GetTaskID"
apilocation: 
  - "mscordbi.dll"
apitype: "COM"
f1_keywords: 
  - "ICorDebugThread2::GetTaskID"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "ICorDebugThread2::GetTaskID method [.NET Framework debugging]"
  - "GetTaskID method [.NET Framework debugging]"
ms.assetid: 6ba3c6ee-4ba1-4c98-bf1e-8531acd3da09
caps.latest.revision: 12
author: "rpetrusha"
ms.author: "ronpet"
manager: "wpickett"
---
# ICorDebugThread2::GetTaskID Method
Gets the identifier of the task running on this thread.  
  
## Syntax  
  
```  
HRESULT GetTaskID (  
    [out] TASKID  *pTaskId  
);  
```  
  
#### Parameters  
 `pTaskId`  
 [out] A pointer to the identifier of the task running on the thread represented by this ICorDebugThread2 object.  
  
## Remarks  
 A task can only be running on the thread if the thread is associated with a connection. `GetTaskID` returns zero in `pTaskId` if the thread is not associated with a connection.  
  
## Requirements  
 **Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).  
  
 **Header:** CorDebug.idl, CorDebug.h  
  
 **Library:** CorGuids.lib  
  
 **.NET Framework Versions:** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]