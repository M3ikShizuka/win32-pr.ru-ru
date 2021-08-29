---
title: sign
description: Возвращает знак x.
ms.assetid: 3e2e04e8-0ffc-4721-a5d8-1ccfa6ca2a1a
keywords:
- подписать HLSL
topic_type:
- apiref
api_name:
- sign
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 80bd3395d2841a3a47e2218b7d8a5e06e8403f3e9d1d4c94ea5a85e6b39939b6
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119120068"
---
# <a name="sign"></a>sign

Возвращает знак *x*.



| знак *возврата* (*x*) |
|-----------------|



 

## <a name="parameters"></a>Параметры



| Элемент                                                   | Описание                        |
|--------------------------------------------------------|------------------------------------|
| <span id="x"></span><span id="X"></span>*x*<br/> | \[во \] входном значении.<br/> |



 

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение-1, если *x* меньше нуля; 0, если *x* равен нулю; и 1, если *x* больше нуля.

## <a name="type-description"></a>Описание типа



| Имя  | [**Тип шаблона**](dx-graphics-hlsl-intrinsic-functions.md)                                                  | [**Тип компонента**](dx-graphics-hlsl-intrinsic-functions.md)                 | Размер                           |
|-------|----------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------|--------------------------------|
| *x*   | [**Скалярная**](dx-graphics-hlsl-intrinsic-functions.md), **векторная** или **Матрица** | [**float**](/windows/desktop/WinProg/windows-data-types), [ **int**](/windows/desktop/WinProg/windows-data-types) | any                            |
| *обратно* | то же, что входные данные *x*                                                                                              | [**INT**](/windows/desktop/WinProg/windows-data-types)                                          | те же измерения, что и входные *x* |



 

## <a name="minimum-shader-model"></a>Минимальная модель шейдера

Эта функция поддерживается в следующих моделях шейдеров.



| Модель шейдера                                                                       | Поддерживается                   |
|------------------------------------------------------------------------------------|-----------------------------|
| [Модели шейдеров 2 (DirectX HLSL)](dx-graphics-hlsl-sm2.md) и более поздние модели шейдеров | Да                         |
| [Модель шейдера 1 (DirectX HLSL)](dx-graphics-hlsl-sm1.md)                          | Да (VS \_ 1 \_ 1 и PS \_ 1 \_ 4) |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Встроенные функции (DirectX HLSL)**](dx-graphics-hlsl-intrinsic-functions.md)
</dt> </dl>

 

