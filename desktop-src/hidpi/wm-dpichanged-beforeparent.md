---
title: Сообщение WM_DPICHANGED_BEFOREPARENT (Winuser. h)
description: Для окон верхнего уровня на мониторе версии 2 это сообщение отправляется во все HWND в дочернем дереве ХВДН окна, которое является изменением DPI. | Сообщение WM_DPICHANGED_BEFOREPARENT (Winuser. h)
ms.assetid: EC8CC313-565F-451F-AE18-66F3B63303CE
keywords:
- WM_DPICHANGED_BEFOREPARENT высокое разрешение для сообщения
topic_type:
- apiref
api_name:
- WM_DPICHANGED_BEFOREPARENT
api_location:
- winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 16641916cb16b789f2349a53b09dbd2af5f520f3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170251"
---
# <a name="wm_dpichanged_beforeparent-message"></a>\_Сообщение WM DPICHANGED \_ бефорепарент

Для окон верхнего уровня [на мониторе версии 2](dpi-awareness-context.md) это сообщение отправляется во все HWND в дочернем дереве хвдн окна, которое является изменением dpi. Это сообщение появляется перед тем, как окно верхнего уровня получает [**WM \_ DPICHANGED**](wm-dpichanged.md)и проходит по дочернему дереву снизу вверх.


```C++
#define WM_DPICHANGED_BEFOREPARENT       0x02E2
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Это значение не используется и будет равняться нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Это значение не используется и будет равняться нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это значение не используется и игнорируется системой.

## <a name="remarks"></a>Remarks

Обработка этого сообщения по умолчанию в [дефвиндовпрок](/windows/win32/api/winuser/nf-winuser-defwindowproca)отсутствует.

Это сообщение отправляется только в том случае, если окно верхнего уровня имеет контекст с отслеживанием DPI для PMv2.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, только для \[ настольных приложений версии 1703\]<br/>                            |
| Минимальная версия сервера<br/> | Windows Server 2016 \[ только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Winuser. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**WM \_ DPICHANGED**](wm-dpichanged.md)
</dt> <dt>

[**WM \_ DPICHANGED \_ афтерпарент**](wm-dpichanged-afterparent.md)
</dt> </dl>

 

