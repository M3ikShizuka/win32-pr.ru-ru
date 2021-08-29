---
description: Посылается окну после того, как оно попадает в модальный цикл перемещения или изменения размера.
ms.assetid: fe09db71-2c79-47f2-b575-516e960915d4
title: Сообщение WM_ENTERSIZEMOVE (Winuser. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c0ffbd3ac8c65b68998a37e64df2593c183b61adb3f8eba1fa140251174b503d
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118436259"
---
# <a name="wm_entersizemove-message"></a>\_Сообщение ЕНТЕРСИЗЕМОВЕ WM

Посылается окну после того, как оно попадает в модальный цикл перемещения или изменения размера. Окно перемещается в модальный цикл перемещения или изменения размера, когда пользователь щелкает заголовок окна или границу изменения размера, или когда окно передает сообщение [**WM \_ сискомманд**](../menurc/wm-syscommand.md) в функцию [**Дефвиндовпрок**](/windows/desktop/api/winuser/nf-winuser-defwindowproca) , а параметр *wParam* сообщения указывает значение **SC \_ Move** или **SC \_ size** . Операция завершается, когда [**дефвиндовпрок**](/windows/desktop/api/winuser/nf-winuser-defwindowproca) возвращает.

Система отправляет сообщение **WM \_ ентерсиземове** независимо от того, включено ли перетаскивание всех окон.

Окно получает это сообщение через функцию [**WindowProc**](/previous-versions/windows/desktop/legacy/ms633573(v=vs.85)) .


```C++
#define WM_ENTERSIZEMOVE                0x0231
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Этот параметр не используется.

</dd> <dt>

*lParam* 
</dt> <dd>

Этот параметр не используется.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **lResult**

Приложение должно вернуть нуль, если оно обрабатывает это сообщение.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                               |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылки**
</dt> <dt>

[**дефвиндовпрок**](/windows/desktop/api/winuser/nf-winuser-defwindowproca)
</dt> <dt>

[**WM \_ екситсиземове**](wm-exitsizemove.md)
</dt> <dt>

[**WM \_ сискомманд**](../menurc/wm-syscommand.md)
</dt> <dt>

**Зрения**
</dt> <dt>

[Windows](windows.md)
</dt> </dl>

 

 
