---
description: Сигнализирует, что доступный набор методов интерфейса IDvdControl2 изменился.
ms.assetid: dfe698b9-abe5-44a7-9844-f408f11fd0ce
title: EC_DVD_VALID_UOPS_CHANGE (Двдевкоде. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- EC_DVD_VALID_UOPS_CHANGE
api_type:
- HeaderDef
api_location:
- dvdevcode.h
ms.openlocfilehash: 26ab0674b504fac3fe374247f47ca20496b22ddf
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246496"
---
# <a name="ec_dvd_valid_uops_change"></a>\_ \_ изменение УОПС допустимого DVD-диска EC \_ \_

Сигнализирует, что доступный набор методов интерфейса [**IDvdControl2**](/windows/desktop/api/Strmif/nn-strmif-idvdcontrol2) изменился.

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="lParam1"></span><span id="lparam1"></span><span id="LPARAM1"></span>*lParam1*
</dt> <dd>

Значение **типа DWORD** , содержащее сочетание одного или нескольких флагов из [**допустимого \_ перечисления \_ флагов УОП**](/windows/win32/api/strmif/ne-strmif-valid_uop_flag) . Биты указывают, какие команды [**IDvdControl2**](/windows/desktop/api/Strmif/nn-strmif-idvdcontrol2) были явно отключены DVD-диском.

</dd> <dt>

<span id="lParam2"></span><span id="lparam2"></span><span id="LPARAM2"></span>*lParam2*
</dt> <dd>

Ноль.

</dd> </dl>

## <a name="remarks"></a>Remarks

Это событие указывает только, какие операции явно отключены содержимым на DVD-диске. Он не гарантирует, что он может вызывать методы, которые не были отключены. Например, если нет кнопок, метод [**IDvdControl2:: активатебуттон**](/windows/desktop/api/Strmif/nf-strmif-idvdcontrol2-activatebutton) не будет работать, даже если метод явно не отключен.

Это событие возникает во всех доменах.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Двдевкоде. h (включение DShow. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[DVD-приложения](dvd-applications.md)
</dt> <dt>

[Коды уведомлений о событиях DVD](dvd-notification-codes.md)
</dt> <dt>

[Уведомление о событии в DirectShow](event-notification-in-directshow.md)
</dt> </dl>

 

 




