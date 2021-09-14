---
title: Функция WaveReadLaneAt
description: Возвращает значение выражения для заданного индекса полосы в заданной волны.
ms.assetid: CA9467D9-8885-4A5D-87F3-5BA40AE78993
keywords:
- Функция Вавереадланеат HLSL
topic_type:
- apiref
api_name:
- WaveReadLaneAt
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 573730053a93a110381637ef8e62dc08a4aa1535
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126970449"
---
# <a name="wavereadlaneat-function"></a>Функция WaveReadLaneAt

Возвращает значение выражения для заданного индекса полосы в заданной волны.

## <a name="syntax"></a>Синтаксис

``` syntax
<type> WaveReadLaneAt(
   <type> expr,
   uint laneIndex
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*expr* 
</dt> <dd>

Выражение для вычисления.

</dd> <dt>

*ланеиндекс* 
</dt> <dd>

Индекс полосы, для которой будет возвращен результат *expr* .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Полученное значение является результатом *выражения expr*. Он будет единообразным, если *ланеиндекс* является однородным.

## <a name="remarks"></a>Комментарии

Эта функция фактически является широковещательной рассылкой значения на *ланеиндекс*"th".

Эта функция поддерживается из модели шейдеров 6,0 на всех стадиях шейдера.

## <a name="see-also"></a>См. также раздел

* [Общие сведения о модели шейдеров 6](hlsl-shader-model-6-0-features-for-direct3d-12.md)
* [Модель шейдеров 6](shader-model-6-0.md)
