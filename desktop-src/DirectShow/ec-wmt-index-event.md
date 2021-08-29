---
description: посылается, когда приложение использует фильтр модуля записи WM ASF для индексирования Windows мультимедийных видеофайлов.
ms.assetid: e5f69aa1-f9b0-4403-acab-25d1f971a876
title: EC_WMT_INDEX_EVENT (DShow. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f76518e72249eb325cb07626c66c66ad7668d772f4b4bc8fe2e0236ff4b37b44
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119928414"
---
# <a name="ec_wmt_index_event-dshowh"></a>EC_WMT_INDEX_EVENT (DShow. h)

посылается, когда приложение использует фильтр [модуля записи WM ASF](wm-asf-writer-filter.md) для индексирования Windows мультимедийных видеофайлов.

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="lParam1"></span><span id="lparam1"></span><span id="LPARAM1"></span>*lParam1*
</dt> <dd>

Может быть одним из следующих сообщений **\_ о состоянии ВМТ** .



| Значение                | Описание              |
|----------------------|--------------------------|
| ВМТ \_ запущен         | Индексирование начато.      |
| ВМТ \_ закрыт          | Индексирование завершено.  |
| \_ \_ ход выполнения индекса ВМТ | Выполняется индексирование. |



 

</dd> <dt>

<span id="lParam2"></span><span id="lparam2"></span><span id="LPARAM2"></span>*lParam2*
</dt> <dd>

Если *LPARAM1* ВМТ \_ Closed или ВМТ \_ Started, то *lParam2* равен нулю. Если *lParam1* является ВМТ \_ \_ ходом выполнения индекса, то *lParam2* — это **DWORD** , который указывает текущий ход выполнения в процентах от общего размера загрузки.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------|------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>DShow. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Коды уведомлений о событиях](event-notification-codes.md)
</dt> <dt>

[Уведомление о событии в DirectShow](event-notification-in-directshow.md)
</dt> </dl>

 

 




