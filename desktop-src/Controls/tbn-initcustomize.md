---
title: Код уведомления TBN_INITCUSTOMIZE (Коммктрл. h)
description: Сообщает родительскому окну панели инструментов, что настройка запущена. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: f4b9a1b0-94f7-4b2b-81b3-772da09134d2
keywords:
- TBN_INITCUSTOMIZE кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- TBN_INITCUSTOMIZE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b9bbf66e9974e444fd8544e20cb4878e662bb94b4b1f958404794783e52664c0
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119876614"
---
# <a name="tbn_initcustomize-notification-code"></a>\_Код уведомления ТБН иниткустомизе

Сообщает родительскому окну панели инструментов, что настройка запущена. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
TBN_INITCUSTOMIZE 

    lpnmhdr = (LPNMHDR) lParam; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**NMHDR**](/windows/desktop/api/richedit/ns-richedit-nmhdr) панели инструментов.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ТБНРФ \_ хидехелп, чтобы отключить кнопку "Справка".

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





