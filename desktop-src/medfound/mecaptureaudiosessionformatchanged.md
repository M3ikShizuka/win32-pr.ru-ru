---
description: Отправляется источником аудиозаписи при изменении формата аудио.
ms.assetid: 8197BBAD-8102-43C3-BA61-8DC3BC13B7D6
title: Событие Мекаптуреаудиосессионформатчанжед (Мфобжектс. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: cfb260d186a9e4d8434669e6a8c3ef08078b93af
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127579963"
---
# <a name="mecaptureaudiosessionformatchanged-event"></a>Событие Мекаптуреаудиосессионформатчанжед

Отправляется источником аудиозаписи при изменении формата аудио.

## <a name="event-values"></a>Значения событий

Возможные значения, полученные из [**имфмедиаевент:: GetValue**](/windows/desktop/api/mfobjects/nf-mfobjects-imfmediaevent-getvalue) , включают следующее.



| VARTYPE               | Описание                           |
|-----------------------|---------------------------------------|
| VT \_ пуст <br/> | Нет данных события.<br/> <br/> |



## <a name="remarks"></a>Remarks

Это событие отправляется потоком мультимедиа источника записи звука.

Источник захвата отправляет это событие при получении события [**иаудиосессионевентс:: онсессиондисконнектед**](/windows/win32/api/audiopolicy/nf-audiopolicy-iaudiosessionevents-onsessiondisconnected) из сеанса аудио с причиной отключения соединения, равной **дисконнектреасонформатчанжед**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                                               |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Мфобжектс. h (включение Мфидл. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[События Media Foundation](media-foundation-events.md)
</dt> </dl>

 

 
