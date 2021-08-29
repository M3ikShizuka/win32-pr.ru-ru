---
title: 'Функция Структуредбуффер:: Load (int)'
description: 'Считывает данные буфера. | Функция Структуредбуффер:: Load (int)'
ms.assetid: ef08d360-0494-49f7-9481-cb802e14aeee
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
ms.openlocfilehash: 4e68ea973edfbcdf3caa8bae0c5ff92693ac15ffccf5230bbf5dcf30d83a9bae
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120095034"
---
# <a name="structuredbufferloadint-function"></a>Функция Структуредбуффер:: Load (int)

Считывает данные буфера.

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

Расположение буфера.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип:

Возвращаемый тип соответствует типу в объявлении для объекта [**структуредбуффер**](sm5-object-structuredbuffer.md) .

## <a name="remarks"></a>Remarks

Эта функция поддерживается для следующих типов шейдеров:



| Вершина | Поверхности | Домен | Геометрия | Пиксель | Службы вычислений |
|--------|------|--------|----------|-------|---------|
|        |      |        |          | x     | x       |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Методы Load](structuredbuffer-load.md)
</dt> </dl>

 

 




