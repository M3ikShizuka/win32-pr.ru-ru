---
description: Указывает, что набор инструкций D3DX в настоящее время оптимизирован для.
ms.assetid: 5fc97028-4a9d-4bc7-9c90-236a70e570e1
title: Перечисление D3DX_CPU_OPTIMIZATION (D3DX10Math. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DX_CPU_OPTIMIZATION
api_type:
- HeaderDef
api_location:
- D3DX10Math.h
ms.openlocfilehash: 208422604e79b3ef7a87b548e7d71eceedd9fb78
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126963949"
---
# <a name="d3dx_cpu_optimization-enumeration"></a>\_ \_ Перечисление оптимизации ЦП D3DX

Указывает, что набор инструкций D3DX в настоящее время оптимизирован для.

## <a name="syntax"></a>Синтаксис


```C++
typedef enum _D3DX_CPU_OPTIMIZATION { 
  D3DX_NOT_OPTIMIZED    = 0,
  D3DX_3DNOW_OPTIMIZED  = 1,
  D3DX_SSE2_OPTIMIZED   = 2,
  D3DX_SSE_OPTIMIZED    = 3
} D3DX_CPU_OPTIMIZATION;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="D3DX_NOT_OPTIMIZED"></span><span id="d3dx_not_optimized"></span>**D3DX \_ не \_ оптимизирован**
</dt> <dd>

Не Оптимизируйте.

</dd> <dt>

<span id="D3DX_3DNOW_OPTIMIZED"></span><span id="d3dx_3dnow_optimized"></span>**D3DX \_ 3DNOW \_ оптимизирован**
</dt> <dd>

Оптимизировать для 3DNow! набор инструкций.

</dd> <dt>

<span id="D3DX_SSE2_OPTIMIZED"></span><span id="d3dx_sse2_optimized"></span>**D3DX \_ SSE2 \_ оптимизирован**
</dt> <dd>

Оптимизировать для набора инструкций SSE2.

</dd> <dt>

<span id="D3DX_SSE_OPTIMIZED"></span><span id="d3dx_sse_optimized"></span>**D3DX \_ SSE \_ оптимизирован**
</dt> <dd>

Оптимизируйте для набора инструкций SSE.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3DX10Math. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Перечисления D3DX](d3d10-graphics-reference-d3dx10-enums.md)
</dt> </dl>

 

 




