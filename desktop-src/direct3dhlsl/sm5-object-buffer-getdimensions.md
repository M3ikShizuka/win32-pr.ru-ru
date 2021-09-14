---
title: 'Функция buffer:: Dimension'
description: 'Возвращает длину буфера. | Функция buffer:: Dimension'
ms.assetid: 704890e8-43e4-4e72-b7e2-eeef331bef1c
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
ms.openlocfilehash: c7f1ad1da7600e65d7442c1b2431535e2fdcf38c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127263851"
---
# <a name="buffergetdimensions-function"></a>Функция buffer:: Dimension

Возвращает длину буфера.

## <a name="syntax"></a>Синтаксис

``` syntax
void GetDimensions(
  out uint dim
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*затемнение* \[\]
</dt> <dd>

Тип: **uint**

Длина буфера в байтах.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Эта функция не возвращает значение.

## <a name="remarks"></a>Remarks

Эта функция поддерживается для следующих типов шейдеров:



| Вершина | Поверхности | Домен | Geometry | Пиксель | Вычисления |
|--------|------|--------|----------|-------|---------|
| x      | x    | x      | x        | x     | x       |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Буфер](sm5-object-buffer.md)
</dt> <dt>

[Модель шейдера 5](d3d11-graphics-reference-sm5.md)
</dt> </dl>

 

 




