---
title: Директива pragma pack_matrix
description: Директива pragma, задающая выравнивание упаковки для матриц.
ms.assetid: e77dc007-d915-4d78-9fff-d44d4999e4da
keywords:
- pack_matrix директивы pragma HLSL
topic_type:
- apiref
api_name:
- pack_matrix pragma Directive
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 87658a9ffcf2d8715e2caa581c7127301784980c
ms.sourcegitcommit: c276a8912787b2cda74dcf54eb96df961bb1188b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2021
ms.locfileid: "122625760"
---
# <a name="pack_matrix-pragma-directive"></a>\_директива pragma матрицы Pack

Директива pragma, задающая выравнивание упаковки для матриц.



| \#\_Матрица pragma pack ( *Выравнивание* ) |
|--------------------------------------|



 

## <a name="parameters"></a>Параметры



<table>
<colgroup>
<col  />
<col  />
</colgroup>
<thead>
<tr class="header">
<th>Элемент</th>
<th>Описание:</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span id="alignment"></span><span id="ALIGNMENT"></span><em>Выравнивание</em><br/></td>
<td>Выравнивание, устанавливаемое для матриц. Этот параметр может принимать одно из значений, перечисленных в следующей таблице. <br/> 
<table>
<thead>
<tr class="header">
<th>Значение</th>
<th>Описание:</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>column_major</td>
<td>По умолчанию. Задает для выравнивания упаковки матрицы значение столбца Major.</td>
</tr>
<tr class="even">
<td>row_major</td>
<td>Задает выравнивание упаковки матрицы по строке основной.</td>
</tr>
</tbody>
</table>

<p> </p></td>
</tr>
</tbody>
</table>



 

## <a name="examples"></a>Примеры

В следующем примере устанавливается выравнивание упаковки матрицы в строку Major.


```
#pragma pack_matrix( row_major )
```



## <a name="see-also"></a>См. также

<dl> <dt>

[Директивы препроцессора (DirectX HLSL)](dx-graphics-hlsl-appendix-preprocessor.md)
</dt> <dt>

[\#Директива pragma (DirectX HLSL)](dx-graphics-hlsl-appendix-pre-pragma.md)
</dt> </dl>

 

 





