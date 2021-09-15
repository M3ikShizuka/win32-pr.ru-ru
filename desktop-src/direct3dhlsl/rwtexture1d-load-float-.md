---
title: 'Функция RWTexture1D:: Load (int)'
description: 'Считывает данные текстуры. | Функция RWTexture1D:: Load (int)'
ms.assetid: AA5E324E-A2C0-45C5-92A8-E4DBC4EB684C
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
ms.openlocfilehash: e78cd12502ada91e48df1ce88be6a19fb714327f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570838"
---
# <a name="rwtexture1dloadint-function"></a>Функция RWTexture1D:: Load (int)

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

Возвращаемый тип соответствует типу в объявлении для объекта [**RWTexture1D**](sm5-object-rwtexture1d.md) .

## <a name="remarks"></a>Комментарии

Эта функция поддерживается для следующих типов шейдеров:



| Вершина | Поверхности | Домен | Geometry | Пиксель | Вычисления |
|--------|------|--------|----------|-------|---------|
|        |      |        |          | x     | x       |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Методы Load](rwtexture1d-load.md)
</dt> </dl>

 

 




