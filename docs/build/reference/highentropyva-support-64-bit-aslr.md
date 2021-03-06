---
title: "-HIGHENTROPYVA (Support 64-Bit ASLR) | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: ["cpp-tools"]
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: ["C++"]
ms.assetid: fe35f9f7-d28e-4694-9aeb-a79db06168e0
caps.latest.revision: 6
author: "corob-msft"
ms.author: "corob"
manager: "ghogen"
ms.workload: ["cplusplus"]
---
# /HIGHENTROPYVA (Support 64-Bit ASLR)
Specifies that the executable image supports high-entropy 64-bit address space layout randomization (ASLR).  
  
## Syntax  
  
```  
/HIGHENTROPYVA[:NO]  
```  
  
## Remarks  
 By default, /HIGHENTROPYVA is on for 64-bit executable images. It is not applicable to 32-bit executable images. To enable this option, /DYNAMICBASE must also be on.  
  
 /HIGHENTROPYVA modifies the header of a .dll file or .exe file to indicate whether ASLR with 64-bit addresses is supported. When this option is set on an executable and all of the modules that it depends on, an operating system that supports 64-bit ASLR can rebase the segments of the executable image at load time by using randomized addresses in a 64-bit virtual address space. This large address space makes it more difficult for an attacker to guess the location of a particular memory region.  
  
### To set this linker option in Visual Studio  
  
1.  Open the project **Property Pages** dialog box. For more information, see [Working with Project Properties](../../ide/working-with-project-properties.md).  
  
2.  Expand the **Configuration Properties** node.  
  
3.  Expand the **Linker** node.  
  
4.  Select the **Command Line** property page.  
  
5.  In **Additional Options**, enter `/HIGHENTROPYVA` or `/HIGHENTROPYVA:NO`.  
  
## See Also  
 [Setting Linker Options](../../build/reference/setting-linker-options.md)   
 [Linker Options](../../build/reference/linker-options.md)