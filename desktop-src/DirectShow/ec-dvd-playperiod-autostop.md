---
description: Указывает, что навигатор завершил воспроизведение сегмента, указанного в вызове IDvdControl2::P Лайпериодинтитлеаутостоп.
ms.assetid: 1716eabe-f106-436a-8a6a-ca43cee9341c
title: EC_DVD_PLAYPERIOD_AUTOSTOP (Двдевкоде. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- EC_DVD_PLAYPERIOD_AUTOSTOP
api_type:
- HeaderDef
api_location:
- dvdevcode.h
ms.openlocfilehash: 4a44495f40608580268cdc162e26dc47b45ffa452a8017a5faff4d672b388704
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119928434"
---
# <a name="ec_dvd_playperiod_autostop"></a>\_автозавершение плайпериод для диска EC DVD \_ \_

Указывает, что навигатор завершил воспроизведение сегмента, указанного в вызове [**IDvdControl2::P лайпериодинтитлеаутостоп**](/windows/desktop/api/Strmif/nf-strmif-idvdcontrol2-playperiodintitleautostop).

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="lParam1"></span><span id="lparam1"></span><span id="LPARAM1"></span>*lParam1*
</dt> <dd>

Ноль.

</dd> <dt>

<span id="lParam2"></span><span id="lparam2"></span><span id="LPARAM2"></span>*lParam2*
</dt> <dd>

Ноль.

</dd> </dl>

## <a name="remarks"></a>Remarks

Это событие возникает в домене Title.

Это событие также отправляется, когда воспроизведение отменяется до того, как навигатор завершает воспроизведение указанного сегмента.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Двдевкоде. h (включение DShow. h)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[DVD-приложения](dvd-applications.md)
</dt> <dt>

[Коды уведомлений о событиях DVD](dvd-notification-codes.md)
</dt> <dt>

[Уведомление о событии в DirectShow](event-notification-in-directshow.md)
</dt> <dt>

[**IDvdControl2::P Лайпериодинтитлеаутостоп**](/windows/desktop/api/Strmif/nf-strmif-idvdcontrol2-playperiodintitleautostop)
</dt> </dl>

 

 




