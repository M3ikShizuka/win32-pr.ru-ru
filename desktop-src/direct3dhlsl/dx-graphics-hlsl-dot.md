---
title: DOT
description: Возвращает скалярное произведение двух векторов.
ms.assetid: ad24c06c-0b40-4dc5-a2b9-1d5438635ed8
keywords:
- точка HLSL
topic_type:
- apiref
api_name:
- dot
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: d6d05abf0d67628d1d77b362b028107e07b83457
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126888261"
---
# <a name="dot"></a>DOT

Возвращает скалярное произведение двух векторов.



| *RET* -точка (*x*, *y*) |
|---------------------|



 

## <a name="parameters"></a>Параметры



| Элемент                                                   | Описание                          |
|--------------------------------------------------------|--------------------------------------|
| <span id="x"></span><span id="X"></span>*x*<br/> | \[в \] первом векторе.<br/>  |
| <span id="y"></span><span id="Y"></span>*&*<br/> | \[во \] втором векторе.<br/> |



 

## <a name="return-value"></a>Возвращаемое значение

Скалярное произведение параметра *x* и параметра *y* .

## <a name="type-description"></a>Описание типа



| Имя  | [**Тип шаблона**](dx-graphics-hlsl-intrinsic-functions.md)                       | [**Тип компонента**](dx-graphics-hlsl-intrinsic-functions.md)                 | Размер                            |
|-------|-------------------------------------------------------------------------------------|--------------------------------------------------------------------------------|---------------------------------|
| *x*   | [**уязвимо**](dx-graphics-hlsl-intrinsic-functions.md) | [**float**](/windows/desktop/WinProg/windows-data-types), [ **int**](/windows/desktop/WinProg/windows-data-types) | any                             |
| *y*   | [**уязвимо**](dx-graphics-hlsl-intrinsic-functions.md) | [**float**](/windows/desktop/WinProg/windows-data-types), [ **int**](/windows/desktop/WinProg/windows-data-types) | те же размеры, что и входные *x* |
| *обратно* | [**функцией**](dx-graphics-hlsl-intrinsic-functions.md) | [**float**](/windows/desktop/WinProg/windows-data-types), [ **int**](/windows/desktop/WinProg/windows-data-types) | 1                               |



 

## <a name="minimum-shader-model"></a>Минимальная модель шейдера

Эта функция поддерживается в следующих моделях шейдеров.



| Модель шейдера                                                                       | Поддерживается |
|------------------------------------------------------------------------------------|-----------|
| [Модели шейдеров 2 (DirectX HLSL)](dx-graphics-hlsl-sm2.md) и более поздние модели шейдеров | yes       |
| [Модель шейдера 1 (DirectX HLSL)](dx-graphics-hlsl-sm1.md)                          | yes       |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Встроенные функции (DirectX HLSL)**](dx-graphics-hlsl-intrinsic-functions.md)
</dt> </dl>

 

