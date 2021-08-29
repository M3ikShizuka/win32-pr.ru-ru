---
description: Происходит, когда подсказка пера обращается к поверхности планшета в дигитайзере.
ms.assetid: 7f4a441d-00d2-4120-8a8d-d3496cdc7e58
title: 'Метод Итаблетевентсинк:: Курсордовн'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ITabletEventSink.CursorDown
api_type:
- COM
api_location:
- wisptis.exe
- wisptis.exe.dll
ms.openlocfilehash: 242e9ebdf2999c342e6ae7f4711a9f142b38a23e977e7dc9a44b906e0062bc2a
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119820644"
---
# <a name="itableteventsinkcursordown-method"></a>Метод Итаблетевентсинк:: Курсордовн

Происходит, когда подсказка пера обращается к поверхности планшета в дигитайзере.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT CursorDown(
  [in] TABLET_CONTEXT_ID tcid,
  [in] CURSOR_ID         cid,
  [in] ULONG             nSerialNumber,
  [in] ULONG             cbPkt,
  [in] BYTE              *pbPkt
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*тЦид* \[ окне\]
</dt> <dd>

Идентификатор планшета.

</dd> <dt>

*CID* \[ в\]
</dt> <dd>

Идентификатор пера.

</dd> <dt>

*нсериалнумбер* \[ окне\]
</dt> <dd>

Серийный номер пера.

</dd> <dt>

*кбпкт* \[ окне\]
</dt> <dd>

Число байтов в пакете данных пера.

</dd> <dt>

*пбпкт* \[ окне\]
</dt> <dd>

Данные пера, указывающие расположение, в котором перо затронуло планшета.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод может возвращать одно из этих значений.



| Код возврата                                                                            | Описание                               |
|----------------------------------------------------------------------------------------|-------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>   | Успешно.<br/>                       |
| <dl> <dt>**\_Ошибка E**</dt> </dl> | Произошла неизвестная ошибка.<br/> |



 

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                              |
| Библиотека<br/>                  | <dl> <dt>Wisptis.exe</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Интерфейс Итаблетевентсинк**](itableteventsink.md)
</dt> </dl>

 

 




