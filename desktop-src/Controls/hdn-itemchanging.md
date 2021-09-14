---
title: Код уведомления HDN_ITEMCHANGING (Коммктрл. h)
description: Сообщает родительскому окну элемента управления заголовка, что атрибуты элемента заголовка будут изменены. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: c3361f88-69d4-425f-b548-0ad3b2a00af4
keywords:
- HDN_ITEMCHANGING кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- HDN_ITEMCHANGING
- HDN_ITEMCHANGINGA
- HDN_ITEMCHANGINGW
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c803f9bde466b524b2ca1cb89062f5fc89d6865f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054185"
---
# <a name="hdn_itemchanging-notification-code"></a>\_Код уведомления ХДН итемчангинг

Сообщает родительскому окну элемента управления заголовка, что атрибуты элемента заголовка будут изменены. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
HDN_ITEMCHANGING

    pNMHeader = (LPNMHEADER) lParam; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмхеадер**](/windows/win32/api/commctrl/ns-commctrl-nmheadera) , содержащую сведения о элементе управления заголовка и элементе заголовка, включая атрибуты, которые необходимо изменить.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение false** , чтобы разрешить изменения, или **true** , чтобы предотвратить их.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |
| Имя в кодировке Юникод и ANSI<br/>   | **ХДН \_ ИТЕМЧАНГИНГВ** (Юникод) и **ХДН \_ итемчангинга** (ANSI)<br/>         |



 

 





