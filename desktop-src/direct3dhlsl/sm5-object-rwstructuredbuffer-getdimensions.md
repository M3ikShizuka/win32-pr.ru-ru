---
title: 'Функция Рвструктуредбуффер:: Dimension'
description: 'Возвращает размеры ресурсов. | Функция Рвструктуредбуффер:: Dimension'
ms.assetid: 842b3d21-2e2b-4906-93ee-0252b2e8cf85
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
ms.openlocfilehash: 0e3868f33e372472999c29bffdd8e12bc8ef09b7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127174711"
---
# <a name="rwstructuredbuffergetdimensions-function"></a>Функция Рвструктуредбуффер:: Dimension

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

Ничего

## <a name="remarks"></a>Remarks

Эта функция поддерживается для следующих типов шейдеров:



| Вершина | Поверхности | Домен | Geometry | Пиксель | Вычисления |
|--------|------|--------|----------|-------|---------|
|        |      |        |          | x     | x       |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[рвструктуредбуффер](sm5-object-rwstructuredbuffer.md)
</dt> <dt>

[Модель шейдера 5](d3d11-graphics-reference-sm5.md)
</dt> </dl>

 

 




