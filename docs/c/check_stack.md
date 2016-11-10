---
title: "check_stack"
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
  - "vc-pragma.check_stack"
  - "check_stack_CPP"
dev_langs: 
  - "C++"
  - "C"
helpviewer_keywords: 
  - "check_stack pragma"
  - "pragmas, check_stack"
  - "pragmas, check_stack usage table"
ms.assetid: f18e20cc-9abb-48b7-ad62-8d384875b996
caps.latest.revision: 7
ms.author: "corob"
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
# check_stack
Instructs the compiler to turn off stack probes if **off** (or **–**) is specified, or to turn on stack probes if **on** (or **+**) is specified.  
  
## Syntax  
  
```  
  
      #pragma check_stack([ {on | off}] )  
#pragma check_stack{+ | –}  
```  
  
## Remarks  
 If no argument is given, stack probes are treated according to the default. This pragma takes effect at the first function defined after the pragma is seen. Stack probes are neither a part of macros nor of functions that are generated inline.  
  
 If you don't give an argument for the **check_stack** pragma, stack checking reverts to the behavior specified on the command line. For more information, see [Compiler Reference](../buildref/compiler-options.md). The interaction of the **#pragma check_stack** and the [/Gs](../buildref/-gs--control-stack-checking-calls-.md) option is summarized in the following table.  
  
### Using the check_stack Pragma  
  
|Syntax|Compiled with<br /><br /> /Gs option?|Action|  
|------------|------------------------------------|------------|  
|**#pragma check_stack( )** or<br /><br /> **#pragma check_stack**|Yes|Turns off stack checking for functions that follow|  
|**#pragma check_stack( )** or<br /><br /> **#pragma check_stack**|No|Turns on stack checking for functions that follow|  
|**#pragma check_stack(on)**<br /><br /> or **#pragma check_stack +**|Yes or No|Turns on stack checking for functions that follow|  
|**#pragma check_stack(off)**<br /><br /> or **#pragma check_stack –**|Yes or No|Turns off stack checking for functions that follow|  
  
## See Also  
 [Pragma Directives and the __Pragma Keyword](../c/pragma-directives-and-the-__pragma-keyword.md)