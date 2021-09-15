---
title: Функция еррорф
description: Отправляет сообщение об ошибке в информационную очередь.
ms.assetid: bf4dc6dc-b36e-4b71-ad61-b7a5ba332879
keywords:
- Функция еррорф HLSL
topic_type:
- apiref
api_name:
- errorf
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 76c8fbcd9b6cb15dbbb735296a3aada8f5e568cb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462415"
---
# <a name="errorf-function"></a>Функция еррорф

Отправляет сообщение об ошибке в информационную очередь.

## <a name="syntax"></a>Синтаксис

``` syntax
void errorf(
   string format,
    argument ...
);
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*format* 
</dt> <dd>

Строка формата.

</dd> <dt>

*аргумент...* 
</dt> <dd>

Необязательные аргументы.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Эта функция не возвращает значение.

## <a name="remarks"></a>Remarks

Эта операция не выполняет никаких действий на устройствах, которые ее не поддерживают.

### <a name="minimum-shader-model"></a>Минимальная модель шейдера

Эта функция поддерживается в следующих моделях шейдеров.



| Модель шейдера                                                        | Поддерживается |
|---------------------------------------------------------------------|-----------|
| [Shader Model 4 (DirectX HLSL) или более поздней версии.](dx-graphics-hlsl-sm3.md) | Да       |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Встроенные функции](dx-graphics-hlsl-intrinsic-functions.md)
</dt> </dl>

 

 




