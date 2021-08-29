---
description: Функция Лоадстрингаддр преобразует строку (например, &\# 0034; 157.54.32.45&\# 0034;) и создает адрес DWORD.
ms.assetid: 305e0072-b597-4cd5-975e-94103a1680aa
title: Функция Лоадстрингаддр (Netmon. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- LoadStringAddr
api_type:
- DllExport
api_location:
- Nmapi.dll
ms.openlocfilehash: 5c706d47c6923de0c01f346430e8050eb94484782cf030186e1ef865f220cc18
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120037144"
---
# <a name="loadstringaddr-function"></a>Функция Лоадстрингаддр

Функция **лоадстрингаддр** преобразует строку (например, "157.54.32.45") и создает адрес **DWORD** .

## <a name="syntax"></a>Синтаксис


```C++
BOOL LoadStringAddr(
         DWORD *pAddress,
   const char  *str
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*паддресс* 
</dt> <dd>

Указатель на **DWORD**.

</dd> <dt>

*str* 
</dt> <dd>

Указатель на строку символов с представлением IP-адреса x. x. x. x (например, 127.0.0.1).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Значение, если функция выполнена успешно (обнаружено имя адреса); Возвращаемое значение равно **true**.

Если функция завершается неудачно, возвращается значение **false**.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl>  |
| Библиотека<br/>                  | <dl> <dt>Нмапи. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Nmapi.dll</dt> </dl> |



 

 




