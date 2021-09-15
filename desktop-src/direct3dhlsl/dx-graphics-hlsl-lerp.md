---
title: лерп
description: Выполняет линейную интерполяцию.
ms.assetid: e369f182-b5bd-4b7f-aa77-9cfe11033bc4
keywords:
- лерп HLSL
topic_type:
- apiref
api_name:
- lerp
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 7c7a5251aaf410d7224b87b9ee9a8f0e8a0c947e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127573063"
---
# <a name="lerp"></a>лерп

Выполняет линейную интерполяцию.



| *RET* лерп (*x*, *y*, *s*) |
|---------------------------|



 

## <a name="parameters"></a>Параметры



| Элемент                                                   | Описание                                                                                           |
|--------------------------------------------------------|-------------------------------------------------------------------------------------------------------|
| <span id="x"></span><span id="X"></span>*x*<br/> | \[в \] значении первого значения с плавающей точкой.<br/>                                                     |
| <span id="y"></span><span id="Y"></span>*&*<br/> | \[во \] втором значении с плавающей запятой.<br/>                                                    |
| <span id="s"></span><span id="S"></span>*#d0*<br/> | \[в \] значении с линейной интерполяцией между параметром *x* и параметром *y* .<br/> |



 

## <a name="return-value"></a>Возвращаемое значение

Результат линейной интерполяции.

## <a name="type-description"></a>Описание типа



| Имя  | [**Тип шаблона**](dx-graphics-hlsl-intrinsic-functions.md)                                                  | [**Тип компонента**](dx-graphics-hlsl-intrinsic-functions.md) | Размер                           |
|-------|----------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------|--------------------------------|
| *x*   | [**Скалярная**](dx-graphics-hlsl-intrinsic-functions.md), **векторная** или **Матрица** | [**сделать**](/windows/desktop/WinProg/windows-data-types)                        | any                            |
| *y*   | то же, что входные данные *x*                                                                                              | [**сделать**](/windows/desktop/WinProg/windows-data-types)                        | те же измерения, что и входные *x* |
| *s*   | то же, что входные данные *x*                                                                                              | [**сделать**](/windows/desktop/WinProg/windows-data-types)                        | те же измерения, что и входные *x* |
| *обратно* | то же, что входные данные *x*                                                                                              | [**сделать**](/windows/desktop/WinProg/windows-data-types)                        | те же измерения, что и входные *x* |



 

## <a name="remarks"></a>Комментарии

Линейная интерполяция основана на следующей формуле: x \* (1-s) + y \* , что может быть эквивалентно записано в виде x + s (y-x).

## <a name="minimum-shader-model"></a>Минимальная модель шейдера

Эта функция поддерживается в следующих моделях шейдеров.



| Модель шейдера                                                                       | Поддерживается                   |
|------------------------------------------------------------------------------------|-----------------------------|
| [Модели шейдеров 2 (DirectX HLSL)](dx-graphics-hlsl-sm2.md) и более поздние модели шейдеров | yes                         |
| [Модель шейдера 1 (DirectX HLSL)](dx-graphics-hlsl-sm1.md)                          | Да (VS 1 1 \_ \_ и PS \_ 1 \_ 1) |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Встроенные функции (DirectX HLSL)**](dx-graphics-hlsl-intrinsic-functions.md)
</dt> </dl>

 

