---
description: Функция Компарефрамесаурцеаддресс сравнивает адрес с исходным адресом кадра.
ms.assetid: 7221c0cc-d6c1-4ec9-bf11-3ba1fefb35da
title: Функция Компарефрамесаурцеаддресс (Netmon. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CompareFrameSourceAddress
api_type:
- DllExport
api_location:
- Nmapi.dll
ms.openlocfilehash: 8738f1322f30baeb5152f5f453cc8d77c74405889caaf667a3d73413d9cdad96
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119891104"
---
# <a name="compareframesourceaddress-function"></a>Функция Компарефрамесаурцеаддресс

Функция **компарефрамесаурцеаддресс** сравнивает адрес с исходным адресом кадра.

## <a name="syntax"></a>Синтаксис


```C++
BOOL WINAPI CompareFrameSourceAddress(
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

## <a name="remarks"></a>Remarks

Чтобы функция **компарефрамесаурцеаддресс** была выполнена, тип адреса источника должен совпадать с типом адреса, указанным в параметре *лпаддресс* .

Сетевой монитор предоставляет две другие функции для сравнения адресов: [компарефрамедестаддресс](compareframedestaddress.md) и [компареаддрессес](compareaddresses.md). Функция **компарефрамедестаддресс** сравнивает заданный адрес с адресом назначения кадра, а функция **компареаддресс** сравнивает два заданных адреса.

[*Эксперты*](e.md) и [*средства синтаксического анализа*](p.md) могут вызывать функцию **компарефрамесаурцеаддресс** .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl>  |
| Библиотека<br/>                  | <dl> <dt>Нмапи. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Nmapi.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[компареаддрессес](compareaddresses.md)
</dt> <dt>

[компарефрамедестаддресс](compareframedestaddress.md)
</dt> </dl>

 

 




