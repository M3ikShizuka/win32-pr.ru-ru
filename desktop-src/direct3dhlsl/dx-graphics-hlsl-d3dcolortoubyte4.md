---
title: D3DCOLORtoUBYTE4
description: Преобразует вектор 4D с плавающей запятой, заданный D3DCOLOR, в UBYTE4.
ms.assetid: 20a7be00-1e36-41c3-bc98-933b3faa8f35
keywords:
- D3DCOLORtoUBYTE4 HLSL
topic_type:
- apiref
api_name:
- D3DCOLORtoUBYTE4
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: c60f0934d6700ec7fbd9e6d9e6443cb6409ab15f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126888325"
---
# <a name="d3dcolortoubyte4"></a>D3DCOLORtoUBYTE4

Преобразует вектор 4D с плавающей запятой, заданный D3DCOLOR, в UBYTE4.



| *RET* D3DCOLORtoUBYTE4 (*x*) |
|-----------------------------|



 

Эта функция свиззлес и масштабирует компоненты параметра *x* . Используйте эту функцию, чтобы компенсировать отсутствие поддержки UBYTE4 в определенном оборудовании.

## <a name="parameters"></a>Параметры



| Элемент                                                   | Описание                                              |
|--------------------------------------------------------|----------------------------------------------------------|
| <span id="x"></span><span id="X"></span>*x*<br/> | \[в \] Vector4 с плавающей запятой для преобразования.<br/> |



 

## <a name="return-value"></a>Возвращаемое значение

UBYTE4 представление параметра *x* .

## <a name="type-description"></a>Описание типа



| Имя  | [**Тип шаблона**](dx-graphics-hlsl-intrinsic-functions.md)                       | [**Тип компонента**](dx-graphics-hlsl-intrinsic-functions.md) | Размер |
|-------|-------------------------------------------------------------------------------------|----------------------------------------------------------------|------|
| *x*   | [**уязвимо**](dx-graphics-hlsl-intrinsic-functions.md) | [**float**](/windows/desktop/WinProg/windows-data-types)                        | 4    |
| *обратно* | [**уязвимо**](dx-graphics-hlsl-intrinsic-functions.md) | [**Целое число**](/windows/desktop/WinProg/windows-data-types)                      | 4    |



 

## <a name="minimum-shader-model"></a>Минимальная модель шейдера

Эта функция поддерживается в следующих моделях шейдеров.



| Модель шейдера                                                                       | Поддерживается |
|------------------------------------------------------------------------------------|-----------|
| [Модели шейдеров 2 (DirectX HLSL)](dx-graphics-hlsl-sm2.md) и более поздние модели шейдеров | yes       |
| [Модель шейдера 1 (DirectX HLSL)](dx-graphics-hlsl-sm1.md)                          | VS \_ 1 \_ 1  |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Встроенные функции (DirectX HLSL)**](dx-graphics-hlsl-intrinsic-functions.md)
</dt> </dl>

 

