---
title: "Expressions in Makefile Preprocessing"
ms.custom: na
ms.date: "10/14/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: na
ms.suite: na
ms.technology: 
  - "devlang-cpp"
ms.tgt_pltfrm: na
ms.topic: "article"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "preprocessing makefiles"
  - "expressions [C++], makefile preprocessing"
  - "makefiles, preprocessing"
ms.assetid: 37f0f413-97e0-452c-a83f-3c9002c44c92
caps.latest.revision: 6
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
# Expressions in Makefile Preprocessing
The **!IF** or **!ELSE IF** `constantexpression` consists of integer constants (in decimal or C-language notation), string constants, or commands. Use parentheses to group expressions. Expressions use C-style signed long integer arithmetic; numbers are in 32-bit two's-complement form in the range – 2147483648 to 2147483647.  
  
 Expressions can use operators that act on constant values, exit codes from commands, strings, macros, and file-system paths.  
  
## What do you want to know more about?  
 [Makefile preprocessing operators](../build/makefile-preprocessing-operators.md)  
  
 [Executing a program in preprocessing](../build/executing-a-program-in-preprocessing.md)  
  
## See Also  
 [Makefile Preprocessing](../build/makefile-preprocessing.md)