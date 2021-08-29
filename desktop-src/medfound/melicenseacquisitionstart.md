---
description: Вызывается модулем политики, когда начинается получение лицензии. Получение лицензии выполняется с помощью реализации интерфейса Имфконтентпротектионманажер в приложениях.
ms.assetid: c328743c-a69b-431e-8a05-0e140aad9b4d
title: Событие Мелиценсеаккуиситионстарт (Мфобжектс. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ea326ff23c4d546f0b692a813ef92ccfce8e3cc97320a8129daa9cedc4867bfc
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119228974"
---
# <a name="melicenseacquisitionstart-event"></a>Событие Мелиценсеаккуиситионстарт

Вызывается модулем политики, когда начинается получение лицензии. Получение лицензии выполняется с помощью реализации интерфейса [**имфконтентпротектионманажер**](/windows/desktop/api/mfidl/nn-mfidl-imfcontentprotectionmanager) в приложении.

## <a name="event-values"></a>Значения событий

Возможные значения, полученные из [**имфмедиаевент:: GetValue**](/windows/desktop/api/mfobjects/nf-mfobjects-imfmediaevent-getvalue) , включают следующее.



| VARTYPE              | Описание                           |
|----------------------|---------------------------------------|
| VT \_ пуст<br/> | Нет данных события.<br/> <br/> |



## <a name="remarks"></a>Remarks

По завершении приобретения лицензии обработчик политики вызывает событие [мелиценсеаккуиситионкомплетед](melicenseacquisitioncompleted.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                                     |
| Header<br/>                   | <dl> <dt>Мфобжектс. h (включение Мфидл. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[События Media Foundation](media-foundation-events.md)
</dt> </dl>

 

 




