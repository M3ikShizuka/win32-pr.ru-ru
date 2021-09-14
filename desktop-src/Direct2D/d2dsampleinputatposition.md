---
title: Функция D2DSampleInputAtPosition (D2d1effecthelpers. h)
description: Выборка входных данных N в абсолютной позиции сцены, а не относительно позиции для входа. Доступно только для сложных входных данных.
ms.assetid: E839287F-91D1-4591-8DE7-1DFC3001A23D
keywords:
- Функция D2DSampleInputAtPosition Direct2D
topic_type:
- apiref
api_name:
- D2DSampleInputAtPosition
api_location:
- d2d1.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e12bba2b83f3956cf4b654c00b0650a6a0ce9a54
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127163448"
---
# <a name="d2dsampleinputatposition-function"></a>Функция D2DSampleInputAtPosition

Выборка входных данных N в абсолютной позиции сцены, а не относительно позиции для входа. Доступно только для сложных входных данных.

## <a name="syntax"></a>Синтаксис

``` syntax
float4 WINAPI D2DSampleInputAtPosition(
  in uint N,
  in float2 uv
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*N* \[ в\]
</dt> <dd>

Входной номер.

</dd> <dt>

*UV* \[ окне\]
</dt> <dd>

Расположение UV.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Функция возвращает **float4** в формате текскурдн.

## <a name="remarks"></a>Комментарии

В следующем примере показана функция, используемая в циклической оболочке.

``` syntax
  
D2D_PS_ENTRY(CircularWrapPS)  
{  
    // TODO: perform math to calculate a circular wrap
  
    // Find the input scene position.  
    float2 inputScenePosition = float2( TODO: add math parameters );  
  
    return D2DSampleInputAtPosition(0, inputScenePosition);  
}
```

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>D2d1effecthelpers. hlsli</dt> </dl> |
| DLL<br/>    | <dl> <dt>D2d1.dll</dt> </dl>                |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Связывание шейдеров эффектов](effect-shader-linking.md)
</dt> <dt>

[Вспомогательные методы HLSL](hlsl-helpers.md)
</dt> </dl>

 

 





