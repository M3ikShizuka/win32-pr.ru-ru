---
title: переставить
description: Переставит указанную входную матрицу.
ms.assetid: 2a2ff2fb-73f0-4bb8-af83-38fe0567d122
keywords:
- переставить HLSL
topic_type:
- apiref
api_name:
- transpose
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 44f129a87edaff260de87136954be7598ee3acb6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127573778"
---
# <a name="transpose"></a>переставить

Переставит указанную входную матрицу.



| RET-транспонировать (*x*) |
|--------------------|



 

## <a name="parameters"></a>Параметры



| Элемент                                                   | Описание                             |
|--------------------------------------------------------|-----------------------------------------|
| <span id="x"></span><span id="X"></span>*x*<br/> | \[в \] указанной матрице.<br/> |



 

## <a name="return-value"></a>Возвращаемое значение

Переданное значение параметра *x* .

## <a name="remarks"></a>Комментарии

Если измерения исходной матрицы являются *столбцами* *строк* , то результирующая матрица будет *строкой* *столбцов* .

## <a name="type-description"></a>Описание типа



| Имя | [**Тип шаблона**](dx-graphics-hlsl-intrinsic-functions.md)                       | [**Тип компонента**](dx-graphics-hlsl-intrinsic-functions.md)                                                         | Размер                                                                                   |
|------|-------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------|
| *x*  | [**таблицу**](dx-graphics-hlsl-intrinsic-functions.md) | [**float**](/windows/desktop/WinProg/windows-data-types), [**int**](/windows/desktop/WinProg/windows-data-types), [**bool**](/windows/desktop/WinProg/windows-data-types) | any                                                                                    |
| обратно  | [**таблицу**](dx-graphics-hlsl-intrinsic-functions.md) | [**float**](/windows/desktop/WinProg/windows-data-types), [**int**](/windows/desktop/WinProg/windows-data-types), [**bool**](/windows/desktop/WinProg/windows-data-types) | строки — одинаковое число столбцов в качестве входных данных *x*, Columns = одинаковое число строк в качестве входных данных *x* |



 

## <a name="minimum-shader-model"></a>Минимальная модель шейдера

Эта функция поддерживается в следующих моделях шейдеров.



| Модель шейдера                                                                       | Поддерживается |
|------------------------------------------------------------------------------------|-----------|
| [Модель шейдера 1 (DirectX HLSL)](dx-graphics-hlsl-sm1.md) и более высокие модели шейдеров | yes       |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Встроенные функции (DirectX HLSL)**](dx-graphics-hlsl-intrinsic-functions.md)
</dt> </dl>

 

