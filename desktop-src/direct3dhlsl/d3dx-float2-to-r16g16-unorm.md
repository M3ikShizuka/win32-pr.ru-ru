---
title: Функция D3DX_FLOAT2_to_R16G16_UNORM
description: Упаковывает заданный XMFLOAT2 обратно в формат DXGI \_ \_ R16G16 \_ UNORM.
ms.assetid: 5a1bd034-262f-4f55-8f38-d2fda42bb13b
keywords:
- Функция D3DX_FLOAT2_to_R16G16_UNORM HLSL
topic_type:
- apiref
api_name:
- D3DX_FLOAT2_to_R16G16_UNORM
api_location:
- D3DX_DXGIFormatConvert.inl
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7a45b63fb60790e3bb657fdc49beff947a0835dbc683158ee7510722fd5a736d
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120024974"
---
# <a name="d3dx_float2_to_r16g16_unorm-function"></a>D3DX \_ FLOAT2 \_ to \_ R16G16 \_ UNORM Function

Упаковывает заданный XMFLOAT2 обратно в формат DXGI \_ \_ R16G16 \_ UNORM.

## <a name="syntax"></a>Синтаксис

``` syntax
UINT D3DX_FLOAT2_to_R16G16_UNORM(
   XMFLOAT2 unpackedInput
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*унпаккединпут* 
</dt> <dd>

Распакованные данные шейдера.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Упакованные данные шейдера.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------|--------------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D3DX \_ дксгиформатконверт. inl</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Функции](format-conversion-functions.md)
</dt> <dt>

[Распаковка и \_ формат упаковки для редактирования образа In-Place](dx-graphics-hlsl-unpacking-packing-dxgi-format.md)
</dt> </dl>

 

 





