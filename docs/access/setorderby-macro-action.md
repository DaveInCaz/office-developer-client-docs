---
title: "SetOrderBy Macro Action"
 
 
manager: soliver
ms.date: 7/29/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- vbaac10.chm98639
  
localization_priority: Normal
ms.assetid: 78f65ce9-b56f-f476-3bd6-f3307bc22a08
description: "You can use the SetOrderBy action to specify how you want to sort records in a form, report, table, or query result."
---

# SetOrderBy Macro Action

You can use the **SetOrderBy** action to specify how you want to sort records in a form, report, table, or query result. 
  
## Setting

The **SetOrderBy** action has the following arguments. 
  
|**Action argument**|**Description**|
|:-----|:-----|
|**Order By** <br/> |A string expression that includes the name of the field or fields on which to sort records and the optional ASC or DESC keywords.  <br/> |
|**Control Name** <br/> |If provided and the active object is a form or report, the name of the control that corresponds to the subform or subreport that will be sorted. If empty and the active object is a form or report, the parent form or report is sorted..  <br/> |
   
## Remarks

When you run this macro action, the sort is applied to the table, form, report or datasheet (query result) that is active and has the focus.
  
The Order By argument is the name of the field or fields on which you want to sort records. When you use more than one field name, separate the names with a comma (,). The **OrderBy** property of the active object is used to save the ordering value and apply it at a later time. OrderBy values are saved with the objects in which they are created. They are automatically loaded when the object is opened, but they aren't automatically applied. 
  
When you set the Order By argument by entering one or more field names and then run the macro, the records are sorted by default in ascending order. 
  
To sort records in descending order, type DESC at the end of the Order By argument expression. For example, to sort customer records in descending order by contact name, set the Order By argument to "ContactName DESC". To sort names by LastName descending, and FirstName ascending, set the Order By argument to "LastName DESC, FirstName ASC".
  
