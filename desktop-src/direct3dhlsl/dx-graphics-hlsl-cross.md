---
title: перекрестные
description: Возвращает перекрестное произведение двух трехмерных векторов с плавающей точкой.
ms.assetid: 5f1832af-6bc5-49a7-956a-fd762f674f5f
keywords:
- перекрестное HLSL
topic_type:
- apiref
api_name:
- cross
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 91959bf415c3e56edf370942de268523bf998743
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126964674"
---
# <a name="cross"></a>перекрестные

Возвращает перекрестное произведение двух трехмерных векторов с плавающей точкой.



| *RET* перекрестие (*x*, *y*) |
|-----------------------|



 

## <a name="parameters"></a>Параметры



| Элемент                                                   | Описание                                             |
|--------------------------------------------------------|---------------------------------------------------------|
| <span id="x"></span><span id="X"></span>*x*<br/> | \[в \] первом трехмерном векторе с плавающей точкой.<br/>  |
| <span id="y"></span><span id="Y"></span>*&*<br/> | \[во \] втором трехмерном векторе с плавающей точкой.<br/> |



 

## <a name="return-value"></a>Возвращаемое значение

Перекрестное произведение параметра *x* и параметра *y* .

## <a name="type-description"></a>Описание типа



| Имя  | [**Тип шаблона**](dx-graphics-hlsl-intrinsic-functions.md)                       | [**Тип компонента**](dx-graphics-hlsl-intrinsic-functions.md) | Размер |
|-------|-------------------------------------------------------------------------------------|----------------------------------------------------------------|------|
| *x*   | [**уязвимо**](dx-graphics-hlsl-intrinsic-functions.md) | [**сделать**](/windows/desktop/WinProg/windows-data-types)                        | 3    |
| *y*   | [**уязвимо**](dx-graphics-hlsl-intrinsic-functions.md) | [**сделать**](/windows/desktop/WinProg/windows-data-types)                        | 3    |
| *обратно* | [**уязвимо**](dx-graphics-hlsl-intrinsic-functions.md) | [**сделать**](/windows/desktop/WinProg/windows-data-types)                        | 3    |



 

## <a name="minimum-shader-model"></a>Минимальная модель шейдера

Эта функция поддерживается в следующих моделях шейдеров.



| Модель шейдера                                                                       | Поддерживается             |
|------------------------------------------------------------------------------------|-----------------------|
| [Модели шейдеров 2 (DirectX HLSL)](dx-graphics-hlsl-sm2.md) и более поздние модели шейдеров | yes                   |
| [Модель шейдера 1 (DirectX HLSL)](dx-graphics-hlsl-sm1.md)                          | VS \_ 1 \_ 1 и PS \_ 1 \_ 4 |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Встроенные функции (DirectX HLSL)**](dx-graphics-hlsl-intrinsic-functions.md)
</dt> </dl>

 

