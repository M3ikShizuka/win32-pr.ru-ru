---
description: Тип настраиваемого события.
ms.assetid: a54a446c-0e96-467b-90f6-0f64a7c1727d
title: Событие Микстендедтипе (Мфобжектс. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 520c0076365c4cea720b0fb04bab5f409206079e776da363d9a448ff5fd3eaa2
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120013604"
---
# <a name="meextendedtype-event"></a>Событие Микстендедтипе

Тип настраиваемого события. Этот тип события можно использовать для определения пользовательских событий для компонента. Для обнаружения события используйте тип расширенного события. Тип расширенного события — это значение GUID, связанное с событием. Дополнительные сведения см. в разделе [**имфмедиаевент:: жетекстендедтипе**](/windows/desktop/api/mfobjects/nf-mfobjects-imfmediaevent-getextendedtype).

## <a name="event-values"></a>Значения событий

Возможные значения, полученные из [**имфмедиаевент:: GetValue**](/windows/desktop/api/mfobjects/nf-mfobjects-imfmediaevent-getvalue) , включают следующее.



| VARTYPE              | Описание                           |
|----------------------|---------------------------------------|
| VT \_ пуст<br/> | Нет данных события.<br/> <br/> |



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Мфобжектс. h (включение Мфидл. h)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[События Media Foundation](media-foundation-events.md)
</dt> </dl>

 

 




