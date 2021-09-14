---
title: Код уведомления ACN_STOP (Коммктрл. h)
description: Уведомляет родительское окно элемента управления анимации о том, что связанный ролик AVI прекратил воспроизведение. Этот код уведомления отправляется в виде \_ командного сообщения WM.
ms.assetid: 2f21a2ec-975f-4592-8b21-956bd5311ef4
keywords:
- ACN_STOP кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- ACN_STOP
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7cbdb27677439b7f08b489cba9024d44f3ebee6d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127174296"
---
# <a name="acn_stop-notification-code"></a>АКН \_ код уведомления о прерывании

Уведомляет родительское окно элемента управления анимации о том, что связанный ролик AVI прекратил воспроизведение. Этот код уведомления отправляется в виде [**\_ командного сообщения WM**](/windows/desktop/menurc/wm-command) .


```C++
ACN_STOP     

    WPARAM wParam;
    LPARAM lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

[**Ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85)) содержит идентификатор элемента управления анимацией. [**HIWORD**](/previous-versions/windows/desktop/legacy/ms632657(v=vs.85)) указывает код уведомления.

</dd> <dt>

*lParam* 
</dt> <dd>

**HWND** , указывающий дескриптор для элемента управления анимации.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

