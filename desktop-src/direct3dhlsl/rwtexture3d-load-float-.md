---
title: 'Функция RWTexture3D:: Load (int)'
description: 'Считывает данные текстуры. | Функция RWTexture3D:: Load (int)'
ms.assetid: 93C4FFFF-8695-4BAF-BAE4-A2704332E6A9
keywords:
- Загрузить функцию HLSL
topic_type:
- apiref
api_name:
- Load
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 70f001cbea05f21a96bfbf1b5bdbf43a1d7da07d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127341967"
---
# <a name="rwtexture3dloadint-function"></a>Функция RWTexture3D:: Load (int)

Считывает данные текстуры.

## <a name="syntax"></a>Синтаксис


``` syntax
 Load(
  in int Location
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Расположение* \[ окне\]
</dt> <dd>

Тип: **int**

Расположение текстуры.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип:

Возвращаемый тип соответствует типу в объявлении для объекта [**RWTexture3D**](sm5-object-rwtexture3d.md) .

## <a name="remarks"></a>Комментарии

Эта функция поддерживается для следующих типов шейдеров:



| Вершина | Поверхности | Домен | Geometry | Пиксель | Вычисления |
|--------|------|--------|----------|-------|---------|
|        |      |        |          | x     | x       |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Методы Load](rwtexture3d-load.md)
</dt> </dl>

 

 




