---
title: 'Функция RWTexture1D:: operator'
description: 'Возвращает переменную ресурса. | Функция RWTexture1D:: operator'
ms.assetid: 16e62879-8ed3-4b17-9124-9da41c41af4f
keywords:
- Оператор Function HLSL
topic_type:
- apiref
api_name:
- Operator
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: ca44252a99e8b8e373cf109341c8c200636d8cf7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126973262"
---
# <a name="rwtexture1doperator--function"></a>Функция RWTexture1D:: operator

Возвращает переменную ресурса.

## <a name="syntax"></a>Синтаксис

``` syntax
R Operator[](
  in uint pos
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*POS-терминал* \[ окне\]
</dt> <dd>

Тип: **uint**

Позиция индекса. Содержит координату x.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **R**

Переменная ресурса.

## <a name="remarks"></a>Комментарии

Эта функция поддерживается для следующих типов шейдеров:



| Вершина | Поверхности | Домен | Geometry | Пиксель | Вычисления |
|--------|------|--------|----------|-------|---------|
|        |      |        |          | x     | x       |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[RWTexture1D](sm5-object-rwtexture1d.md)
</dt> <dt>

[Модель шейдера 5](d3d11-graphics-reference-sm5.md)
</dt> </dl>

 

 




