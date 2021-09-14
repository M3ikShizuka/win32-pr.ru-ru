---
description: Функция Компарефрамедестаддресс сравнивает адрес с адресом назначения кадра.
ms.assetid: 739b3b9f-f989-459d-ac3e-6be7769adc06
title: Функция Компарефрамедестаддресс (Netmon. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CompareFrameDestAddress
api_type:
- DllExport
api_location:
- Nmapi.dll
ms.openlocfilehash: a9ce0ff776588c06b8fddc34240e9c2170ceca69
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127253870"
---
# <a name="compareframedestaddress-function"></a>Функция Компарефрамедестаддресс

Функция **компарефрамедестаддресс** сравнивает адрес с адресом назначения кадра.

## <a name="syntax"></a>Синтаксис


```C++
BOOL WINAPI CompareFrameDestAddress(
  _In_ HFRAME    hFrame,
  _In_ LPADDRESS lpAddress
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*хфраме* \[ окне\]
</dt> <dd>

Обработчик для фрейма.

</dd> <dt>

*лпаддресс* \[ окне\]
</dt> <dd>

Указатель на адрес.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если адреса совпадают, возвращается значение **true**.

Если адреса не совпадают, возвращается значение **false**.

## <a name="remarks"></a>Комментарии

Чтобы функция **компарефрамедестаддресс** успешно возвращалась, тип адреса назначения должен совпадать с типом адреса, указанным в параметре *лпаддресс* .

Сетевой монитор предоставляет две другие функции, [компарефрамесаурцеаддресс](compareframesourceaddress.md) и [компареаддрессес](compareaddresses.md), которые можно использовать для сравнения адресов. Функция **компарефрамесаурцеаддресс** сравнивает заданный адрес с исходным адресом кадра, а функция **компареаддресс** сравнивает два заданных адреса.

[*Эксперты*](e.md) и [*средства синтаксического анализа*](p.md) могут вызывать функцию **компарефрамедестаддресс** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl>  |
| Библиотека<br/>                  | <dl> <dt>Нмапи. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Nmapi.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[компареаддрессес](compareaddresses.md)
</dt> <dt>

[компарефрамесаурцеаддресс](compareframesourceaddress.md)
</dt> </dl>

 

 




