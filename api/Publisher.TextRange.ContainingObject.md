---
title: TextRange.ContainingObject property (Publisher)
keywords: vbapb10.chm5308465
f1_keywords:
- vbapb10.chm5308465
ms.prod: publisher
api_name:
- Publisher.TextRange.ContainingObject
ms.assetid: f15c81b5-d03f-0d83-323b-6ec6f57b4f26
ms.date: 06/15/2019
ms.localizationpriority: medium
---


# TextRange.ContainingObject property (Publisher)

Returns an **Object** that represents the object that contains the text range. Read-only.


## Syntax

_expression_.**ContainingObject**

_expression_ A variable that represents a **[TextRange](Publisher.TextRange.md)** object.


## Return value

Object


## Example

This example returns the name of the object containing the specified text range.

```vb
Sub NameOfContainingObject() 
 With ActiveDocument.Pages(1).Shapes(1).TextFrame _ 
 .TextRange.ContainingObject 
 MsgBox The name of the object containing the text is " & .Name 
 End With 
End Sub
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]