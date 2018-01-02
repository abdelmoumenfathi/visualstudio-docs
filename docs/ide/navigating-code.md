---
title: "Navigating Code | Microsoft Docs"
ms.custom: ""
ms.date: "09/26/2017"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-general"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "code editor, navigation"
  - "code editor, go to"
  - "code editor, go to definition"
  - "code editor, go to line"
  - "code editor, peek definition"
  - "code editor, navigation bar"
  - "go to definition"
  - "peek definition"
  - "go to line"
  - "go to"
author: "gewarren"
ms.author: "gewarren"
manager: ghogen
ms.workload: 
  - "multiple"
---
# Navigating Code  
Visual Studio provides numerous ways to navigate code in the editor. This topic summarizes the different ways you can navigate your code, and provides links to topics that go into more detail.  

## Navigate Backward and Navigate Forward commands  
You can use the **Navigate Backward** (**Ctrl + -**) and **Navigate Forward** (**Ctrl + Shift + -**) buttons on the toolbar to move the insertion point to previous locations, or to return to a more recent location from a previous location. These buttons retain the last 20 locations of the insertion point. These commands are also available on the **View** menu, under **Navigate Backward** and **Navigate Forward**.  

![Forward and back navigation buttons](../ide/media/vs2017_nav_buttons.png)  

## Navigation bar
You can use the **navigation bar** (the drop-down boxes at the top of the code window) to navigate to code in a codebase. You can choose a type or member to go directly to it. The navigation bar appears when you edit code in a Visual Basic, C#, or C++ code base. In a partial class, members defined outside the current code file may be disabled (they appear in grey).  

 ![Code navigation bar](../ide/media/vside_navigation_bar.png)

You can navigate around the drop-down boxes as follows:  

-   To navigate to another project that the current file belongs to, choose it in the left drop-down.

-   To navigate to a class or type, choose it in the middle drop-down.  

-   To navigate directly to a procedure or other member of a class, choose it in the right drop-down.  

-   To shift focus from the code window to the navigation bar, press the shortcut key combination **Ctrl + F2**.  

-   To shift focus from box to box on the navigation bar, press the **Tab** key.  

-   To select the navigation bar item that has focus and return to the code window, press the **Enter** key.  

-   To return focus from the navigation bar to the code  without selecting anything, press the **Esc** key.  

To hide the navigation bar, change the **Navigation bar** option in the Text Editor All Languages settings (**Tools**, **Options**, **Text Editor**, **All Languages**), or you can change the settings for individual languages.  

## Find All References  
Finds all the references to the selected element in the solution. You can use this to check possible side-effects of a large refactoring, or to verify "dead" code. Press **F8** to jump between results. For more information, see [Finding references in your code](finding-references.md).  

Input        | Function 
------------ | ---
**Keyboard** | Place your text cursor somewhere inside the type name, and press **Shift + F12**  
**Mouse**    | Select **Find All References** from the context menu  

## Reference highlighting
When you click a symbol in the source code, all instances of that symbol are highlighted in the document. The highlighted symbols may include declarations and references, and many other symbols that **Find All References** would return. These include the names of classes, objects, variables, methods, and properties. In Visual Basic code, keywords for many control structures are also highlighted. To move to the next or the previous highlighted symbol, press **Ctrl + Shift + DOWN ARROW** or **Ctrl + Shift + UP ARROW**. You can change the highlighting color in **Tools**, **Options**, **Environment**, **Fonts and Colors**, **Highlighted Reference.**  

## Go To commands  
Go To has the following commands, which are available in the **Edit** menu under **Go To**:  

- **Go To Line** (**Ctrl + G**): Move to the specified line number in the active document.  

- **Go to All** (**Ctrl + T** or **Ctrl + ,**): Move to the specified line, type, file, member, or symbol.  

- **Go to File** (**Ctrl + 1**, **Ctrl + F**): Move to the specified file in the solution.  

- **Go to Type** (**Ctrl + 1**, **Ctrl + T**): Move to the specified type in the solution.  

- **Go to Member** (**Ctrl + 1**, **Ctrl + M**): Move to the specified member in the solution.  

- **Go to Symbol** (**Ctrl + 1**, **Ctrl + S**): Move to the specifed symbol in the solution.  

See more about these commands in the [Find code using Go To commands](../ide/go-to.md) topic.  

## Go To Definition  
Go To Definition takes you to the definition of the selected element. For more information, see [Go To Defintion and Peek Definition](../ide/go-to-and-peek-definition.md).  

Input        | Function 
------------ | ---
**Keyboard** | Place your text cursor somewhere inside the type name, and press **F12**
**Mouse**    | Right-click on the type name and select **Go To Definition**  OR  press **Ctrl** and click on the type name (new for Visual Studio 2017 version 15.4)  

## Peek Definition  
Peek Definition displays the definition of the selected element in a window without navigating away from your current location in the code editor. For more information, see [How to: View and Edit Code by Using Peek Definition](../ide/how-to-view-and-edit-code-by-using-peek-definition-alt-plus-f12.md) and [Go To Defintion and Peek Definition](../ide/go-to-and-peek-definition.md).  

Input        | Function 
------------ | ---
**Keyboard** | Place your text cursor somewhere inside the type name, and press **Alt + F12**
**Mouse**    | Right-click on the type name and select **Peek Definition** OR press **Ctrl** and click on the type name (if you have the **Open definition in peek view** option checked)  

## Go To Implementation  
Using Go To Implementation, you can navigate from a base class or type to its implementations. If there are multiple implementations, you will see them listed in the **Find Symbol Results** window:  

Input        | Function 
------------ | ---
**Keyboard** | Place your text cursor somewhere inside the type name, and press **Ctrl + F12**
**Mouse**    | Right-click on the type name and select **Go To Implementation**  

## Call Hierarchy  
Call Hierarchy shows you the calls to a method in the Call Hierarchy window:  

Input        | Function 
------------ | ---
**Keyboard** | Place your text cursor somewhere inside the type name, and press **Ctrl + K**, **Ctrl + T**  
**Mouse**    | Right-click on the member name and select **View Call Hierarchy**  

## Next Method and Previous Method commands (Visual Basic)  
In Visual Basic code files, use these commands to move the insertion point to different methods. Choose **Edit**, **Next Method** or **Edit**, **Previous Method**.  

## Structure Visualizer  
The Structure Visualizer feature in the code editor shows *structure guide lines* - vertical dashed lines that indicate matching curly braces in your codebase. This makes it easier to see where logical blocks begin and end.  

![Structure Visualizer](../ide/media/vside_structure_visualizer.png)  

To disable structure guide lines, go to **Tools**, **Options**, **Text Editor**, **General** and clear the **Show structure guide lines** box.  

## Enhanced scroll bar
You can use the enhanced scroll bar in a code window to get a bird's-eye view of your code. In map mode, you can see previews of the code when you move the cursor up and down the scroll bar. For more information, see [How to: Track Your Code by Customizing the Scroll Bar](../ide/how-to-track-your-code-by-customizing-the-scrollbar.md).  

## CodeLens information
You can find info about specific code, like changes and who made those changes, references, bugs, work items, code reviews, and unit test status when you use CodeLens in the code editor. CodeLens works like a heads-up display when you use Visual Studio Enterprise with Team Foundation Server. See [Find code changes and other history](../ide/find-code-changes-and-other-history-with-codelens.md).  

## See Also  
[Writing code in the code and text editor](../ide/writing-code-in-the-code-and-text-editor.md) 