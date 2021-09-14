---
title: Сообщение HDM_SETFILTERCHANGETIMEOUT (Коммктрл. h)
description: Устанавливает интервал времени ожидания между временем изменения атрибутов фильтра и разноски \_ уведомления ХДН филтерчанже. Это сообщение можно отправить явным образом или воспользоваться заголовком \_ макроса сетфилтерчанжетимеаут.
ms.assetid: 9bc8e0e7-d7c1-4dd6-9d39-6ae937f19d60
keywords:
- элементы управления Windows сообщений HDM_SETFILTERCHANGETIMEOUT
topic_type:
- apiref
api_name:
- HDM_SETFILTERCHANGETIMEOUT
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9876634d12cd15001c296151694cb755ed1b34e9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054225"
---
# <a name="hdm_setfilterchangetimeout-message"></a>\_Сообщение СЕТФИЛТЕРЧАНЖЕТИМЕАУТ HDM

Устанавливает интервал времени ожидания между временем изменения атрибутов фильтра и разноски уведомления [ХДН \_ филтерчанже](hdn-filterchange.md) . Это сообщение можно отправить явным образом или воспользоваться [**заголовком макроса \_ сетфилтерчанжетимеаут**](/windows/desktop/api/Commctrl/nf-commctrl-header_setfilterchangetimeout) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Значение времени ожидания в миллисекундах.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает индекс изменяемого элемента управления фильтра.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[ХДН \_ филтерчанже](hdn-filterchange.md)
</dt> </dl>

 

 





