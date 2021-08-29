---
title: Код уведомления HDN_FILTERCHANGE (Коммктрл. h)
description: Сообщает родительскому окну элемента управления заголовка, что атрибуты фильтра элемента управления заголовков изменяются или редактируются. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: 0a46af14-569a-4119-881f-549a130f9b0d
keywords:
- HDN_FILTERCHANGE кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- HDN_FILTERCHANGE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: df9cb23123460e06bd2d8c3a5a38e2465e4382f80d223f978c82a1ea8702dfd8
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119435524"
---
# <a name="hdn_filterchange-notification-code"></a>\_Код уведомления ХДН филтерчанже

Сообщает родительскому окну элемента управления заголовка, что атрибуты фильтра элемента управления заголовков изменяются или редактируются. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
HDN_FILTERCHANGE

    pNMHeader =  (LPNMHEADER) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмхеадер**](/windows/win32/api/commctrl/ns-commctrl-nmheadera) , содержащую сведения о элементе управления заголовка и элементе заголовка, включая атрибуты, которые необходимо изменить.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_СЕТФИЛТЕРЧАНЖЕТИМЕАУТ HDM**](hdm-setfilterchangetimeout.md)
</dt> </dl>

 

 





