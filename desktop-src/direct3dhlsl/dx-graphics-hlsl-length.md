---
title: length
description: Возвращает длину указанного вектора с плавающей точкой.
ms.assetid: eb06c87c-d536-448e-becb-762783cc2a77
keywords:
- Длина HLSL
topic_type:
- apiref
api_name:
- length
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: a7a93b0a7d225a25273a2ab4f8bf1d24656b6ee1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127573066"
---
# <a name="length"></a>length

Возвращает длину указанного вектора с плавающей точкой.



| Длина *RET* (*x*) |
|-------------------|



 

## <a name="parameters"></a>Параметры



| Элемент                                                   | Описание:                                     |
|--------------------------------------------------------|-------------------------------------------------|
| <span id="x"></span><span id="X"></span>*x*<br/> | Указанный вектор с плавающей точкой.<br/> |



 

## <a name="return-value"></a>Возвращаемое значение

Скалярная точка с плавающей запятой, представляющая длину параметра *x* .

## <a name="type-description"></a>Описание типа



| Имя  | [**Тип шаблона**](dx-graphics-hlsl-intrinsic-functions.md)                       | [**Тип компонента**](dx-graphics-hlsl-intrinsic-functions.md) | Размер |
|-------|-------------------------------------------------------------------------------------|----------------------------------------------------------------|------|
| *x*   | [**уязвимо**](dx-graphics-hlsl-intrinsic-functions.md) | [**сделать**](/windows/desktop/WinProg/windows-data-types)                        | any  |
| *обратно* | [**функцией**](dx-graphics-hlsl-intrinsic-functions.md) | [**FLOAT**](/windows/desktop/WinProg/windows-data-types)                        | 1    |



 

## <a name="minimum-shader-model"></a>Минимальная модель шейдера

Эта функция поддерживается в следующих моделях шейдеров.



| Модель шейдера                                                                       | Поддерживается           |
|------------------------------------------------------------------------------------|---------------------|
| [Модели шейдеров 2 (DirectX HLSL)](dx-graphics-hlsl-sm2.md) и более поздние модели шейдеров | Да                 |
| [Модель шейдера 1 (DirectX HLSL)](dx-graphics-hlsl-sm1.md)                          | Да ( \_ только VS 1 1 \_ ) |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Встроенные функции (DirectX HLSL)**](dx-graphics-hlsl-intrinsic-functions.md)
</dt> </dl>

 

