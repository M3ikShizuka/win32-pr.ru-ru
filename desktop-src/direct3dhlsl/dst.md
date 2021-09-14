---
title: функция DST
description: Вычисляет вектор расстояний. | функция DST
ms.assetid: 24d22743-5867-49db-8d0a-55cc3625c947
keywords:
- функция DST HLSL
topic_type:
- apiref
api_name:
- dst
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 58ce243cf9a9f3e6118763368445e5bcf26ba4cc
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127264192"
---
# <a name="dst-function"></a>функция DST

Вычисляет вектор расстояний.

## <a name="syntax"></a>Синтаксис

``` syntax
fVector dst(
  in fVector src0,
  in fVector src1
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*src0* \[ окне\]
</dt> <dd>

Тип: **[фвектор](dx-graphics-hlsl-vector.md)**

Первый вектор.

</dd> <dt>

*src1* \[ окне\]
</dt> <dd>

Тип: **[фвектор](dx-graphics-hlsl-vector.md)**

Второй вектор.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[фвектор](dx-graphics-hlsl-vector.md)**

Вычисленный вектор расстояний.

## <a name="remarks"></a>Remarks

Эта встроенная функция предоставляет те же функциональные возможности, что и время [летнего времени](dst---vs.md)для инструкции шейдера вершин.

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Встроенные функции](dx-graphics-hlsl-intrinsic-functions.md)
</dt> </dl>

 

 




