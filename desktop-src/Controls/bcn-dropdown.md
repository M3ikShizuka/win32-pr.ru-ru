---
title: Код уведомления BCN_DROPDOWN (Winuser. h)
description: Посылается, когда пользователь щелкает стрелку раскрывающегося списка на кнопке. Родительское окно элемента управления получает этот код уведомления в виде \_ сообщения WM notify.
ms.assetid: 61503b8d-193e-4855-b9eb-35c0dc636c02
keywords:
- BCN_DROPDOWN кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- BCN_DROPDOWN
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e78512419f62beaa82aff42ccaf951d34130fe3a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126968730"
---
# <a name="bcn_dropdown-notification-code"></a>\_Код уведомления для раскрывающегося списка BCN

Посылается, когда пользователь щелкает стрелку раскрывающегося списка на кнопке. Родительское окно элемента управления получает этот код уведомления в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
BCN_DROPDOWN
        
    pnmdropdown = (NMBCDROPDOWN*) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмбкдропдовн**](/windows/win32/api/commctrl/ns-commctrl-nmbcdropdown) . Для элемента **ркбуттон** задано описание раскрывающегося области.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Комментарии

Получатель уведомлений выполняет приведение **lParam** для получения структуры [**нмбкдропдовн**](/windows/win32/api/commctrl/ns-commctrl-nmbcdropdown) . **WParam** содержит идентификатор элемента управления, который отправляет это сообщение. Элемент управления "Кнопка" должен иметь стиль кнопки раскрывающегося списка.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



 

 





