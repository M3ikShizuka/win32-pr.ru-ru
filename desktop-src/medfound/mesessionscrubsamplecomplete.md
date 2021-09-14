---
description: Вызывается сеансом мультимедиа при завершении запроса на очистку.
ms.assetid: 1ae97022-3fb2-4c5e-9262-d5bdc2a62bee
title: Событие Месессионскрубсамплекомплете (Мфобжектс. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b076c2f2978831cc30521fcf49d71c04620c4dee
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127257888"
---
# <a name="mesessionscrubsamplecomplete-event"></a>Событие Месессионскрубсамплекомплете

Вызывается сеансом мультимедиа при завершении запроса на очистку.

Очистка происходит, когда скорость воспроизведения равна нулю и приложение вызывает [**имфмедиасессион:: Start**](/windows/desktop/api/mfidl/nf-mfidl-imfmediasession-start). Это событие возникает после завершения запроса очистки каждым приемником потока.

## <a name="event-values"></a>Значения событий

Возможные значения, полученные из [**имфмедиаевент:: GetValue**](/windows/desktop/api/mfobjects/nf-mfobjects-imfmediaevent-getvalue) , включают следующее.



| VARTYPE              | Описание:                           |
|----------------------|---------------------------------------|
| VT \_ пуст<br/> | Нет данных события.<br/> <br/> |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Мфобжектс. h (включение Мфидл. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[События Media Foundation](media-foundation-events.md)
</dt> <dt>

[местреамсинкскрубсамплекомплете](mestreamsinkscrubsamplecomplete.md)
</dt> </dl>

 

 




