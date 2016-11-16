---
title: "Use command line option &#39;&lt;option&gt;&#39; or appropriate project settings instead of &#39;&lt;parameter&gt;&#39; | Microsoft Docs"
ms.custom: ""
ms.date: "2015-07-20"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "bc41008"
  - "vbc41008"
helpviewer_keywords: 
  - "BC41008"
ms.assetid: 1c5d6d7a-b767-4dae-aa61-d7fa81d5aad1
caps.latest.revision: 4
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
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
# Use command line option &#39;&lt;option&gt;&#39; or appropriate project settings instead of &#39;&lt;parameter&gt;&#39;
The preferred way to specify a file that contains a public key for an assembly, a public-key container for an assembly, or a partial-signed assembly is to use the [!INCLUDE[vbprvb](../dotnet/includes/vbprvb_md.md)] compiler options. We do not recommend use of the <xref:System.Reflection.AssemblyKeyFileAttribute>, <xref:System.Reflection.AssemblyKeyNameAttribute>, or <xref:System.Reflection.AssemblyDelaySignAttribute> attributes in your code.  
  
 **Error ID:** BC41008  
  
### To correct this error  
  
1.  Use the [/keyfile](/dotnet/visual-basic/reference/command-line-compiler/keyfile), [/keycontainer](/dotnet/visual-basic/reference/command-line-compiler/keycontainer), or [/delaysign](/dotnet/visual-basic/reference/command-line-compiler/delaysign)[!INCLUDE[vbprvb](../dotnet/includes/vbprvb_md.md)] compiler options instead of the <xref:System.Reflection.AssemblyKeyFileAttribute>, <xref:System.Reflection.AssemblyKeyNameAttribute>, or <xref:System.Reflection.AssemblyDelaySignAttribute> attributes in your code.  
  
## See Also  
 [How to: Create Signed Friend Assemblies](../Topic/How%20to:%20Create%20Signed%20Friend%20Assemblies%20\(C%23%20and%20Visual%20Basic\).md)   
 [Visual Basic Command-Line Compiler](/dotnet/visual-basic/reference/command-line-compiler/index)   
 [/keyfile](/dotnet/visual-basic/reference/command-line-compiler/keyfile)   
 [/keycontainer](/dotnet/visual-basic/reference/command-line-compiler/keycontainer)   
 [/delaysign](/dotnet/visual-basic/reference/command-line-compiler/delaysign)