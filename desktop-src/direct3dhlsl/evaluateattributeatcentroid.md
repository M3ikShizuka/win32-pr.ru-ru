---
title: Функция Евалуатеаттрибутеатцентроид
description: Вычисляется на центроид пикселей.
ms.assetid: 6735b3f4-765f-4cd9-9f38-326a52709021
keywords:
- Функция Евалуатеаттрибутеатцентроид HLSL
topic_type:
- apiref
api_name:
- EvaluateAttributeAtCentroid
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: ee95c7f2f202dfd0065e5e9c30003cc46fd29281
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126973286"
---
# <a name="evaluateattributeatcentroid-function"></a>Функция Евалуатеаттрибутеатцентроид

Вычисляется на центроид пикселей.

## <a name="syntax"></a>Синтаксис

``` syntax
numeric EvaluateAttributeAtCentroid(
  in attrib numeric value
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*значение* \[ окне\]
</dt> <dd>

Тип: **attrib numeric**

Входное значение.

</dd> </dl>

## <a name="remarks"></a>Комментарии

Режим интерполяции может быть **линейным** или **линейным \_ без \_ перспективы** для переменной. Использование **центроид** или **Sample** не учитывается. Также разрешены атрибуты с интерполяцией константы. в этом случае пример индекса игнорируется.

### <a name="minimum-shader-model"></a>Минимальная модель шейдера

Эта функция поддерживается в следующих моделях шейдеров.



| Модель шейдера                                                                | Поддерживается |
|-----------------------------------------------------------------------------|-----------|
| [Модели шейдера 5](d3d11-graphics-reference-sm5.md) и более поздних моделей шейдеров | да       |



 

Эта функция поддерживается в следующих типах шейдеров:



| Вершина | Поверхности | Домен | Geometry | Пиксель | Вычисления |
|--------|------|--------|----------|-------|---------|
|        |      |        |          | x     |         |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Встроенные функции](dx-graphics-hlsl-intrinsic-functions.md)
</dt> <dt>

[Модель шейдера 5](d3d11-graphics-reference-sm5.md)
</dt> </dl>

 

 




