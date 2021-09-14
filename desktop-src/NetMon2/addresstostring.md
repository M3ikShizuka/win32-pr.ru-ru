---
description: Функция Аддресстостринг преобразует адрес в строку.
ms.assetid: 999a6142-1423-4006-a489-63895dd19ce3
title: Функция Аддресстостринг (Netmon. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- AddressToString
api_type:
- DllExport
api_location:
- Nmapi.dll
ms.openlocfilehash: 0c7c659a05167055b18c36e5c6c36465538af483
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127067632"
---
# <a name="addresstostring-function"></a>Функция Аддресстостринг

Функция **аддресстостринг** преобразует адрес в строку.

## <a name="syntax"></a>Синтаксис


```C++
LPSTR WINAPI AddressToString(
  _Out_ LPSTR string,
  _In_  BYTE  *lpAddress
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*строка* \[ заполняет\]
</dt> <dd>

Строка, в которую преобразуется адрес.

</dd> <dt>

*лпаддресс* \[ окне\]
</dt> <dd>

Выводимый адрес.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение является указателем на преобразованную строку.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                            |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl>   |
| Библиотека<br/>                  | <dl> <dt>Parser. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Nmapi.dll</dt> </dl>  |



 

 




