---
title: "-Fo (Object File Name)"
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
  - "/Fo"
  - "VC.Project.VCCLCompilerTool.ObjectFile"
  - "VC.Project.VCCLWCECompilerTool.ObjectFile"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "Fo compiler option [C++]"
  - "object files, naming"
  - "/Fo compiler option [C++]"
  - "-Fo compiler option [C++]"
ms.assetid: 0e6d593e-4e7f-4990-9e6e-92e1dcbcf6e6
caps.latest.revision: 11
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
# /Fo (Object File Name)
Specifies an object (.obj) file name or directory to be used instead of the default.  
  
## Syntax  
  
```  
/Fopathname  
```  
  
## Remarks  
 If you do not use this option, the object file uses the base name of the source file and the .obj extension. You can use any name and extension you want, but the recommended convention is to use .obj.  
  
### To set this compiler option in the Visual Studio development environment  
  
1.  Open the project's **Property Pages** dialog box. For details, see [How to: Open Project Property Pages](../notintoc/how-to--open-project-property-pages.md).  
  
2.  Click the **C/C++** folder.  
  
3.  Click the **Output Files** property page.  
  
4.  Modify the **Object File Name** property.  In the development environment, the object file must have an extension of .obj.  
  
### To set this compiler option programmatically  
  
-   See \<xref:Microsoft.VisualStudio.VCProjectEngine.VCCLCompilerTool.ObjectFile*>.  
  
## Example  
 The following command line creates an object file named THIS.obj in an existing directory, \OBJECT, on drive B.  
  
```  
CL /FoB:\OBJECT\ THIS.C  
```  
  
## See Also  
 [Output-File (/F) Options](../buildref/output-file---f--options.md)   
 [Compiler Options](../buildref/compiler-options.md)   
 [Setting Compiler Options](../buildref/setting-compiler-options.md)   
 [Specifying the Pathname](../buildref/specifying-the-pathname.md)