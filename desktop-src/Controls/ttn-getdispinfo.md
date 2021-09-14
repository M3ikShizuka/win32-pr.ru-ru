---
title: Код уведомления TTN_GETDISPINFO (Коммктрл. h)
description: Посылается элементом управления ToolTip для получения сведений, необходимых для вывода окна подсказки. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: af9ecc27-2004-4c45-9f1d-9ee0b2b50ff6
keywords:
- TTN_GETDISPINFO кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- TTN_GETDISPINFO
- TTN_GETDISPINFOA
- TTN_GETDISPINFOW
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: bc1fe07d12331e523fed9e1ff46b9e265487bc31
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165815"
---
# <a name="ttn_getdispinfo-notification-code"></a>\_Код уведомления ТТН жетдиспинфо

Посылается элементом управления ToolTip для получения сведений, необходимых для вывода окна подсказки. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
TTN_GETDISPINFO

    lpnmtdi = (LPNMTTDISPINFO) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмттдиспинфо**](/windows/win32/api/commctrl/ns-commctrl-nmttdispinfoa) , определяющую средство, которое нуждается в тексте и получает запрошенные сведения.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение для этого уведомления не используется.

## <a name="remarks"></a>Remarks

Заполните соответствующие элементы структуры, чтобы вернуть запрошенные сведения в элемент управления ToolTip. Если обработчик сообщений задает для элемента **уфлагс** структуры [**нмттдиспинфо**](/windows/win32/api/commctrl/ns-commctrl-nmttdispinfoa) значение TTF \_ di \_ сетитем, элемент управления ToolTip сохраняет информацию и не запрашивает их снова.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |
| Имя в кодировке Юникод и ANSI<br/>   | **ТТН \_ ЖЕТДИСПИНФОВ** (Юникод) и **ТТН \_ жетдиспинфоа** (ANSI)<br/>           |



 

 





