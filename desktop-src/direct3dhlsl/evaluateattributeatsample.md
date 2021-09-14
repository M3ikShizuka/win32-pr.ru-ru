---
title: Функция Евалуатеаттрибутеатсампле
description: Вычисляется в расположении с индексированным образцом.
ms.assetid: b5886004-5960-461d-a0d2-f4c3b0d09d94
keywords:
- Функция Евалуатеаттрибутеатсампле HLSL
topic_type:
- apiref
api_name:
- EvaluateAttributeAtSample
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: b183f86599d08a6892e33c169b938dc09a2b55de
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127342278"
---
# <a name="evaluateattributeatsample-function"></a>Функция Евалуатеаттрибутеатсампле

Вычисляется в расположении с индексированным образцом.

## <a name="syntax"></a>Синтаксис

``` syntax
numeric EvaluateAttributeAtSample(
  in attrib numeric value,
  in uint sampleindex
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*значение* \[ окне\]
</dt> <dd>

Тип: **attrib numeric**

Входное значение.

</dd> <dt>

*sampleindex* \[ окне\]
</dt> <dd>

Тип: **uint**

Расположение образца.

</dd> </dl>

## <a name="remarks"></a>Remarks

Режим интерполяции может быть **линейным** или **линейным \_ без \_ перспективы** для переменной. Использование **центроид** или **Sample** не учитывается. Также разрешены атрибуты с интерполяцией константы. в этом случае пример индекса игнорируется.

### <a name="minimum-shader-model"></a>Минимальная модель шейдера

Эта функция поддерживается в следующих моделях шейдеров.



| Модель шейдера                                                                | Поддерживается |
|-----------------------------------------------------------------------------|-----------|
| [Модели шейдера 5](d3d11-graphics-reference-sm5.md) и более поздних моделей шейдеров | Да       |



 

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

 

 




