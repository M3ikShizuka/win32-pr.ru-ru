---
title: Функция Abort (Корекрт \_ Terminate. h)
description: Отправляет сообщение об ошибке в информационную очередь и завершает текущий выполняемый вызов Draw или Dispatch.
ms.assetid: b8ce153b-0d1c-4294-b88e-b7e50e708ab9
keywords:
- Функция Abort HLSL
topic_type:
- apiref
api_name:
- abort
api_location:
- corecrt_terminate.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9428a03b422aed9ff6fae097459a53369d3a30e1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127264427"
---
# <a name="abort-function"></a>Функция abort

Отправляет сообщение об ошибке в информационную очередь и завершает текущий выполняемый вызов Draw или Dispatch.

## <a name="syntax"></a>Синтаксис

``` syntax
void abort(
    
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

 
</dt> <dd>

None

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Эта функция не возвращает значение.

## <a name="remarks"></a>Remarks

Эта операция не выполняет никаких действий на средствах прорисовки, не поддерживающих эту операцию.

### <a name="minimum-shader-model"></a>Минимальная модель шейдера

Эта функция поддерживается в следующих моделях шейдеров.



| Модель шейдера                                                        | Поддерживается |
|---------------------------------------------------------------------|-----------|
| [Shader Model 4 (DirectX HLSL) или более поздней версии.](dx-graphics-hlsl-sm3.md) | Да       |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|---------------------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Корекрт \_ Terminate. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Встроенные функции](dx-graphics-hlsl-intrinsic-functions.md)
</dt> </dl>

 

 





