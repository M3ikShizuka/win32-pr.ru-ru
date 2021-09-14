---
title: 'Функция Структуредбуффер:: Dimension'
description: 'Возвращает размеры ресурсов. | Функция Структуредбуффер:: Dimension'
ms.assetid: 423ea79c-4440-4837-b637-95180a1d5019
keywords:
- Функция Dimension HLSL
topic_type:
- apiref
api_name:
- GetDimensions
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 2b3d7c879c77386ddee80a63053711b8ae34ee8c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126963537"
---
# <a name="structuredbuffergetdimensions-function"></a>Функция Структуредбуффер:: Dimension

Возвращает размеры ресурсов.

## <a name="syntax"></a>Синтаксис

``` syntax
void GetDimensions(
  out uint numStructs,
  out uint stride
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*нумструктс* \[ заполняет\]
</dt> <dd>

Тип: **uint**

Число структур в ресурсе.

</dd> <dt>

*Шаг с шагом* \[ заполняет\]
</dt> <dd>

Тип: **uint**

Шаг в байтах для каждого элемента структуры.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Эта функция не возвращает значение.

## <a name="remarks"></a>Комментарии

Эта функция поддерживается для следующих типов шейдеров:



| Вершина | Поверхности | Домен | Geometry | Пиксель | Вычисления |
|--------|------|--------|----------|-------|---------|
| x      | x    | x      | x        | x     | x       |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[структуредбуффер](sm5-object-structuredbuffer.md)
</dt> <dt>

[Модель шейдера 5](d3d11-graphics-reference-sm5.md)
</dt> </dl>

 

 




