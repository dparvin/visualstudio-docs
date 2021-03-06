---
title: "BP_COND_STYLE | Microsoft Docs"
ms.custom: ""
ms.date: 11/15/2016
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "BP_COND_STYLE"
helpviewer_keywords: 
  - "BP_COND_STYLE enumeration"
ms.assetid: a93b1412-f447-48a1-af9d-38f3dbb3092f
caps.latest.revision: 11
ms.author: "gregvanl"
manager: "ghogen"
---
# BP_COND_STYLE
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

Specifies the breakpoint condition style for pending and bound breakpoints.  
  
## Syntax  
  
```cpp#  
enum enum_BP_COND_STYLE {   
   BP_COND_NONE         = 0x0000,  
   BP_COND_WHEN_TRUE    = 0x0001,  
   BP_COND_WHEN_CHANGED = 0x0002  
};  
typedef DWORD BP_COND_STYLE;  
```  
  
```csharp  
public enum enum_BP_COND_STYLE {   
   BP_COND_NONE         = 0x0000,  
   BP_COND_WHEN_TRUE    = 0x0001,  
   BP_COND_WHEN_CHANGED = 0x0002  
};  
```  
  
## Members  
 BP_COND_NONE  
 Fires the breakpoint when the breakpoint's position is reached. No breakpoint condition specified.  
  
 BP_COND_WHEN_TRUE  
 Fires the breakpoint only when the conditional expression associated with the breakpoint evaluates to `true`.  
  
 BP_COND_WHEN_CHANGED  
 Fires the breakpoint only when the value of the conditional expression associated with the breakpoint has changed from its previous evaluation.  
  
## Remarks  
 Used for the `styleCondition` member of the [BP_CONDITION](../../../extensibility/debugger/reference/bp-condition.md) structure.  
  
## Requirements  
 Header: msdbg.h  
  
 Namespace: Microsoft.VisualStudio.Debugger.Interop  
  
 Assembly: Microsoft.VisualStudio.Debugger.Interop.dll  
  
## See Also  
 [Enumerations](../../../extensibility/debugger/reference/enumerations-visual-studio-debugging.md)   
 [BP_CONDITION](../../../extensibility/debugger/reference/bp-condition.md)

