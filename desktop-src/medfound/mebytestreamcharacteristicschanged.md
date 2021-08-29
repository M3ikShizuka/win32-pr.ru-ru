---
description: Отправляется потоком байтов при изменении характеристик потока байтов.
ms.assetid: EC34A7A3-BF01-4F9E-BA79-131B76D4C58F
title: Событие Мебитестреамчарактеристиксчанжед (Мфобжектс. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f1401f420bf1c40a5449a91e2af9a6e1c328ea6591ee3b8eeacedd34213eab4a
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119941764"
---
# <a name="mebytestreamcharacteristicschanged-event"></a>Событие Мебитестреамчарактеристиксчанжед

Отправляется потоком байтов при изменении характеристик потока байтов.

## <a name="event-values"></a>Значения событий

Возможные значения, полученные из [**имфмедиаевент:: GetValue**](/windows/desktop/api/mfobjects/nf-mfobjects-imfmediaevent-getvalue) , включают следующее.



| VARTYPE               | Описание                           |
|-----------------------|---------------------------------------|
| VT \_ пуст <br/> | Нет данных события.<br/> <br/> |



## <a name="remarks"></a>Remarks

Это событие означает, что изменилась одна или несколько из следующих характеристик:

-   Флаги возможностей ([**имфбитестреам:: Capabilities**](/windows/desktop/api/mfobjects/nf-mfobjects-imfbytestream-getcapabilities))
-   Флаг конца потока ([**имфбитестреам:: исендофстреам**](/windows/desktop/api/mfobjects/nf-mfobjects-imfbytestream-isendofstream))
-   Length ([**имфбитестреам:: DATALENGTH**](/windows/desktop/api/mfobjects/nf-mfobjects-imfbytestream-getlength))

Это событие поддерживают не все реализации [**имфбитестреам**](/windows/desktop/api/mfobjects/nn-mfobjects-imfbytestream) . Чтобы получить событие, запросите объект байтового потока для интерфейса [**имфмедиаевентженератор**](/windows/desktop/api/mfobjects/nn-mfobjects-imfmediaeventgenerator) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                                               |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Мфобжектс. h (включение Мфидл. h)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[События Media Foundation](media-foundation-events.md)
</dt> </dl>

 

 




