---
title: 'Функция Texture1DArray:: operator'
description: 'Возвращает переменную ресурса, доступную только для чтения. | Функция Texture1DArray:: operator'
ms.assetid: 05ec9652-b5dd-41cf-8bef-730c507c5ba4
keywords:
- Оператор Function HLSL
topic_type:
- apiref
api_name:
- Operator
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 578d778cd1e0e064c435c19fb094feb66f651e05
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126884088"
---
# <a name="texture1darrayoperator--function"></a>Функция Texture1DArray:: operator

Возвращает переменную ресурса, доступную только для чтения.

## <a name="syntax"></a>Синтаксис

``` syntax
R Operator[](
  in uint2 pos
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*POS-терминал* \[ окне\]
</dt> <dd>

Тип: **uint2**

Позиция индекса. Первый компонент содержит координату x. Второй компонент указывает нужный срез массива.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **R**

Переменная ресурса, доступная только для чтения.

## <a name="remarks"></a>Комментарии

Этот метод всегда обращается к первому MIP уровню. Чтобы указать другие уровни MIP, используйте вместо него метод [**MIP \[ \] \[ \] . operator**](sm5-object-texture1darray-mipsoperatorindex.md) .

Эта функция поддерживается для следующих типов шейдеров:



| Вершина | Поверхности | Домен | Geometry | Пиксель | Вычисления |
|--------|------|--------|----------|-------|---------|
| x      | x    | x      | x        | x     | x       |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Texture1DArray](sm5-object-texture1darray.md)
</dt> <dt>

[Модель шейдера 5](d3d11-graphics-reference-sm5.md)
</dt> </dl>

 

 




