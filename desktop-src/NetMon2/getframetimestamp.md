---
description: Функция Жетфраметиместамп возвращает метку времени данного кадра.
ms.assetid: 4ac50400-6674-40fa-9a69-9c0ccb55b92c
title: Функция Жетфраметиместамп (Netmon. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- GetFrameTimeStamp
api_type:
- DllExport
api_location:
- Nmapi.dll
ms.openlocfilehash: 37a75f946a5fc0ddb2b32d99334368a272fdf2e6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173583"
---
# <a name="getframetimestamp-function"></a>Функция Жетфраметиместамп

Функция **жетфраметиместамп** возвращает метку времени данного кадра.

## <a name="syntax"></a>Синтаксис


```C++
__int64 WINAPI GetFrameTimeStamp(
  _In_ HFRAME hFrame
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*хфраме* \[ окне\]
</dt> <dd>

Обработчик для фрейма.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если функция выполнена успешно, возвращаемое значение — это метка времени кадра в микросекундах.

Если функция завершилась неудачно, возвращаемое значение равно минус единице (-1).

## <a name="remarks"></a>Remarks

Функция **жетфраметиместамп** возвращает метку времени, которая показывает время, прошедшее с начала процесса записи, и запись кадра.

[*Эксперты*](e.md) и [*средства синтаксического анализа*](p.md) могут вызывать функцию **жетфраметиместамп** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl>  |
| Библиотека<br/>                  | <dl> <dt>Нмапи. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Nmapi.dll</dt> </dl> |



 

 




