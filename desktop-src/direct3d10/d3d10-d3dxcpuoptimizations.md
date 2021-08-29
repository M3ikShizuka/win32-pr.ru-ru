---
description: Включает или отключает оптимизацию ЦП.
ms.assetid: 6f73df12-f2fc-4651-b0f7-f7a55e534d3d
title: Функция D3DXCpuOptimizations (D3DX10Math. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXCpuOptimizations
api_type:
- LibDef
api_location:
- D3DX10.lib
- D3DX10.dll
ms.openlocfilehash: de2c24667384ad8f163774c77b4f7fea9332e953425cd5ee520cd310fa0733a7
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119853454"
---
# <a name="d3dxcpuoptimizations-function"></a>Функция D3DXCpuOptimizations

Включает или отключает оптимизацию ЦП.

## <a name="syntax"></a>Синтаксис


```C++
D3DX_CPU_OPTIMIZATION D3DXCpuOptimizations(
  _In_ BOOL Enable
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Включить* \[ окне\]
</dt> <dd>

Тип: **[ **bool** .](../winprog/windows-data-types.md)**

**Значение true** , чтобы включить оптимизацию ЦП; в противном случае — **false**.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **\_ \_ Оптимизация ЦП D3DX**](d3dx-cpu-optimization.md)**

Возвращает тип обнаруженного ЦП, для которого существуют оптимизации (см. раздел [**\_ \_ Оптимизация ЦП D3DX**](d3dx-cpu-optimization.md)).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX10Math. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3DX10. lib</dt> </dl>   |



## <a name="see-also"></a>См. также

<dl> <dt>

[Математические функции](d3d10-graphics-reference-d3dx10-functions-math.md)
</dt> </dl>

 

 
