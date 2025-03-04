---
description: "Learn more about: MEDIAN"
title: "MEDIAN function (DAX) | Microsoft Docs"
ms.service: powerbi 
ms.subservice: dax 
ms.date: 07/08/2020
ms.reviewer: owend
ms.topic: reference
author: minewiskan
ms.author: owend 
recommendations: false
---
# MEDIAN
  
Returns the median of numbers in a column.  
  
To return the median of an expresssion evaluated for each row in a table, use [MEDIANX function](medianx-function-dax.md).  
  
## Syntax  
  
```dax
MEDIAN(<column>)  
```
  
### Parameters  
  
|Term|Definition|  
|--------|--------------|  
|column|The column that contains the numbers for which the median is to be computed.|  
  
## Return value

A decimal number.  
  
## Remarks

- Only the numbers in the column are counted. Blanks, logical values, and text are ignored.  
  
- MEDIAN( Table[Column] ) is equivalent to MEDIANX( Table, Table[Column] ).  

- [!INCLUDE [function-not-supported-in-directquery-mode](includes/function-not-supported-in-directquery-mode.md)]

## Example

The following computes the median of a column named Age in a table named Customers:  
  
```dax
= MEDIAN( Customers[Age] )  
```
  
## See also

[MEDIANX function](medianx-function-dax.md)  
