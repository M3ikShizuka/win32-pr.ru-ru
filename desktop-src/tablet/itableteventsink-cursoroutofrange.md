---
description: Происходит, когда перо покидает диапазон физического обнаружения (близость) планшета.
ms.assetid: ded01278-126d-415d-9a7b-1e6fe3650a37
title: 'Метод Итаблетевентсинк:: Курсораутофранже'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ITabletEventSink.CursorOutOfRange
api_type:
- COM
api_location:
- wisptis.exe
- wisptis.exe.dll
ms.openlocfilehash: e2250401f3888bd07ff250549c11c34e6a54576d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460231"
---
# <a name="itableteventsinkcursoroutofrange-method"></a>Метод Итаблетевентсинк:: Курсораутофранже

Происходит, когда перо покидает диапазон физического обнаружения (близость) планшета.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT CursorOutOfRange(
  [in] TABLET_CONTEXT_ID tcid,
       t                 cid
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*тЦид* \[ окне\]
</dt> <dd>

Идентификатор планшета.

</dd> <dt>

*согласуется* 
</dt> <dd>

Идентификатор пера.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод может возвращать одно из этих значений.



| Код возврата                                                                            | Описание                               |
|----------------------------------------------------------------------------------------|-------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>   | Успешно.<br/>                       |
| <dl> <dt>**\_Ошибка E**</dt> </dl> | Произошла неизвестная ошибка.<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                              |
| Библиотека<br/>                  | <dl> <dt>Wisptis.exe</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Итаблетевентсинк**](itableteventsink.md)
</dt> </dl>

 

 




