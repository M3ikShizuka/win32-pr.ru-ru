---
description: Функция Жетфрамемактипе Возвращает тип MAC фрейма.
ms.assetid: 8d3da770-1392-4638-a267-32c2dae289b0
title: Функция Жетфрамемактипе (Netmon. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- GetFrameMacType
api_type:
- DllExport
api_location:
- Nmapi.dll
ms.openlocfilehash: b85accc64a6e29424e3f65d070bafcf29bb3ec0f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173584"
---
# <a name="getframemactype-function"></a>Функция Жетфрамемактипе

Функция **жетфрамемактипе** ВОЗВРАЩАЕТ тип Mac фрейма.

## <a name="syntax"></a>Синтаксис


```C++
DWORD WINAPI GetFrameMacType(
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

Функция возвращает тип MAC фрейма, который может иметь одно из следующих значений.

-   \_неизвестный тип Mac \_
-   \_тип Mac \_ Ethernet
-   \_тип Mac \_ токенринг
-   \_тип Mac \_ FDDI

## <a name="remarks"></a>Remarks

[*Эксперты*](e.md) и [*средства синтаксического анализа*](p.md) могут вызывать функцию **жетфрамемактипе** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl>  |
| Библиотека<br/>                  | <dl> <dt>Нмапи. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Nmapi.dll</dt> </dl> |



 

 




