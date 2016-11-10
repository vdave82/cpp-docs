---
title: "&#39;System.Runtime.InteropServices.DllImportAttribute&#39; cannot be applied to interface methods"
ms.custom: na
ms.date: "10/13/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: na
ms.suite: na
ms.technology: 
  - "devlang-csharp"
ms.tgt_pltfrm: na
ms.topic: "article"
f1_keywords: 
  - "bc31530"
  - "vbc31530"
helpviewer_keywords: 
  - "BC31530"
ms.assetid: e63f1f7d-b7df-4637-a0f4-2783479ca1af
caps.latest.revision: 6
ms.author: "billchi"
manager: "douge"
translation.priority.ht: 
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "ru-ru"
  - "zh-cn"
  - "zh-tw"
translation.priority.mt: 
  - "cs-cz"
  - "pl-pl"
  - "pt-br"
  - "tr-tr"
---
# &#39;System.Runtime.InteropServices.DllImportAttribute&#39; cannot be applied to interface methods
A procedure is defined inside an interface, but the procedure definition applies the \<xref:System.Runtime.InteropServices.DllImportAttribute>.  
  
 The common language runtime (CLR) recognizes this attribute and its \<xref:System.Runtime.InteropServices._Assembly.EntryPoint*> property as designating a replacement procedure defined in an unmanaged dynamic-link library (DLL) outside the .NET Framework. When code calls the procedure to which the \<xref:System.Runtime.InteropServices.DllImportAttribute> is applied, the common language runtime calls the designated unmanaged procedure instead.  
  
 Because the definition of a procedure inside an interface does not include any implementation, it cannot interoperate with unmanaged platforms outside the .NET Framework.  
  
 **Error ID:** BC31530  
  
### To correct this error  
  
-   Remove the \<xref:System.Runtime.InteropServices.DllImportAttribute> from the definition of this procedure.  
  
## See Also  
 \<xref:System.Runtime.InteropServices.DllImportAttribute>   
 [Interface Statement](../Topic/Interface%20Statement%20\(Visual%20Basic\).md)