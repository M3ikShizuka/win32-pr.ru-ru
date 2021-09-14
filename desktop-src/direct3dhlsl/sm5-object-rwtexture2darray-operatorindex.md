---
title: 'Функция RWTexture2DArray:: operator'
description: 'Возвращает переменную ресурса. | Функция RWTexture2DArray:: operator'
ms.assetid: ae3d0697-ea0a-450d-bdfe-7bc5d8faf11a
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
ms.openlocfilehash: faf49c48fbf5042ce2765005cd8daea4d1227255
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461182"
---
# <a name="rwtexture2darrayoperator--function"></a>Функция RWTexture2DArray:: operator

Возвращает переменную ресурса.

## <a name="syntax"></a>Синтаксис

``` syntax
R Operator[](
  in uint3 pos
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*POS-терминал* \[ окне\]
</dt> <dd>

Тип: **uint3**

Позиция индекса. Первый и второй компоненты содержат координаты (x, y). Третий компонент указывает нужный срез массива.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **R**

Переменная ресурса.

## <a name="remarks"></a>Remarks

Эта функция поддерживается для следующих типов шейдеров:



| Вершина | Поверхности | Домен | Geometry | Пиксель | Вычисления |
|--------|------|--------|----------|-------|---------|
|        |      |        |          | x     | x       |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[RWTexture2DArray](sm5-object-rwtexture2darray.md)
</dt> <dt>

[Модель шейдера 5](d3d11-graphics-reference-sm5.md)
</dt> </dl>

 

 




