---
title: Код уведомления NM_RELEASEDCAPTURE (монскал) (Коммктрл. h)
description: Сообщает родительскому окну элемента управления монскал, что элемент управления освобождает захват мыши. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: c05d3331-26f3-41f4-8032-36ed38d47917
keywords:
- NM_RELEASEDCAPTURE (монскал) код уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- NM_RELEASEDCAPTURE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0b9c743a076c8046aa57ba4306145248ed00f0fe
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167899"
---
# <a name="nm_releasedcapture-monthcal-notification-code"></a>\_Код уведомления NM релеаседкаптуре (монскал)

Сообщает родительскому окну элемента управления монскал, что элемент управления освобождает захват мыши. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
NM_RELEASEDCAPTURE

    lpnmh = (LPNMHDR) lParam; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**NMHDR**](/windows/desktop/api/richedit/ns-richedit-nmhdr) , содержащую дополнительные сведения об этом уведомлении.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Элемент управления игнорирует возвращаемое значение из этого кода уведомления.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





