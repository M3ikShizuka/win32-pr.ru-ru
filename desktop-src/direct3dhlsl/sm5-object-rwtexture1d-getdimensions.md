---
title: 'Функция RWTexture1D:: Dimension'
description: 'Возвращает размеры ресурса. | Функция RWTexture1D:: Dimension'
ms.assetid: 1bbd53ed-9396-4e8e-b2f3-3bd85f6e1a90
keywords:
- Функция Dimension HLSL
topic_type:
- apiref
api_name:
- GetDimensions
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: b65f0113ecf2c91786e45c35f5e8e832744bc952
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127342899"
---
# <a name="rwtexture1dgetdimensions-function"></a>Функция RWTexture1D:: Dimension

Возвращает размеры ресурса.

## <a name="syntax"></a>Синтаксис

``` syntax
void GetDimensions(
  out UINT Width
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*Ширина* \[ заполняет\]
</dt> <dd>

Тип: **[ **uint**](/windows/desktop/WinProg/windows-data-types)**

Ширина ресурса в пикселей текстуры.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Ничего

## <a name="remarks"></a>Remarks

Это список перегруженных версий этого метода.


```
void GetDimensions (out UINT Width);

void GetDimensions(out float Width);
```



Эта функция поддерживается для следующих типов шейдеров:



| Вершина | Поверхности | Домен | Geometry | Пиксель | Вычисления |
|--------|------|--------|----------|-------|---------|
|        |      |        |          | x     | x       |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[RWTexture1D](sm5-object-rwtexture1d.md)
</dt> <dt>

[Модель шейдера 5](d3d11-graphics-reference-sm5.md)
</dt> </dl>

 

 
