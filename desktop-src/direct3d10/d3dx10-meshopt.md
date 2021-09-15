---
description: Перечисление D3DX10_MESHOPT — указывает тип выполняемой оптимизации сетки.
ms.assetid: 20d1da8c-8c3d-4045-9a37-d534a8682716
title: Перечисление D3DX10_MESHOPT (D3DX10Mesh. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DX10_MESHOPT
api_type:
- HeaderDef
api_location:
- D3DX10Mesh.h
ms.openlocfilehash: 7b3085cf9970f2c1f6fe3748cc4db8f4fb2b2a78
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127566727"
---
# <a name="d3dx10_meshopt-enumeration"></a>\_Перечисление МЕШОПТ D3DX10

Указывает тип оптимизации сетки для выполнения.

## <a name="syntax"></a>Синтаксис


```C++
typedef enum D3DX10_MESHOPT { 
  D3DX10_MESHOPT_COMPACT             = 0x01000000,
  D3DX10_MESHOPT_ATTR_SORT           = 0x02000000,
  D3DX10_MESHOPT_VERTEX_CACHE        = 0x04000000,
  D3DX10_MESHOPT_STRIP_REORDER       = 0x08000000,
  D3DX10_MESHOPT_IGNORE_VERTS        = 0x10000000,
  D3DX10_MESHOPT_DO_NOT_SPLIT        = 0x20000000,
  D3DX10_MESHOPT_DEVICE_INDEPENDENT  = 0x00400000
} D3DX10_MESHOPT, *LPD3DX10_MESHOPT;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="D3DX10_MESHOPT_COMPACT"></span><span id="d3dx10_meshopt_compact"></span>**D3DX10 \_ мешопт \_ Compact**
</dt> <dd>

Переупорядочивает лица, чтобы удалить неиспользуемые вершины и грани.

</dd> <dt>

<span id="D3DX10_MESHOPT_ATTR_SORT"></span><span id="d3dx10_meshopt_attr_sort"></span>**D3DX10 \_ мешопт \_ attr \_ Sort**
</dt> <dd>

Переупорядочивает лиц, чтобы оптимизировать для уменьшения количества изменений состояния набора атрибутов и повышения производительности Дравсубсет.

</dd> <dt>

<span id="D3DX10_MESHOPT_VERTEX_CACHE"></span><span id="d3dx10_meshopt_vertex_cache"></span>**\_ \_ Кэш вершин D3DX10 \_ мешопт**
</dt> <dd>

Переупорядочивает лиц, чтобы увеличить количество попаданий в кэш вершин.

</dd> <dt>

<span id="D3DX10_MESHOPT_STRIP_REORDER"></span><span id="d3dx10_meshopt_strip_reorder"></span>**\_ \_ Переупорядочение чередующихся мешопт D3DX10 \_**
</dt> <dd>

Переупорядочивает лиц, чтобы максимально увеличить длину смежных треугольников.

</dd> <dt>

<span id="D3DX10_MESHOPT_IGNORE_VERTS"></span><span id="d3dx10_meshopt_ignore_verts"></span>**D3DX10 \_ мешопт \_ игнорировать \_ вертикальные**
</dt> <dd>

Оптимизируйте только грани; не Оптимизируйте вершины.

</dd> <dt>

<span id="D3DX10_MESHOPT_DO_NOT_SPLIT"></span><span id="d3dx10_meshopt_do_not_split"></span>**D3DX10 \_ мешопт \_ \_ не \_ разбиваются**
</dt> <dd>

При сортировке атрибутов не разделите вершины, которые являются общими между группами атрибутов.

</dd> <dt>

<span id="D3DX10_MESHOPT_DEVICE_INDEPENDENT"></span><span id="d3dx10_meshopt_device_independent"></span>**\_ \_ Независимое устройство D3DX10 мешопт \_**
</dt> <dd>

Влияет на размер кэша вершин. С помощью этого флага задается размер кэша вершин по умолчанию, который хорошо работает на устаревшем оборудовании.

</dd> </dl>

## <a name="remarks"></a>Remarks

\_Флаги оптимизации D3DXMESHOPT стрипреордер и D3DXMESHOPT \_ вертекскаче являются взаимоисключающими.

Флаг D3DXMESHOPT \_ шаревб был удален из этого перечисления. \_ \_ Вместо этого используйте общую папку VB D3DXMESH в D3DXMESH.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3DX10Mesh. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Перечисления D3DX](d3d10-graphics-reference-d3dx10-enums.md)
</dt> </dl>

 

 




