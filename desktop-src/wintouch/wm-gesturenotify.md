---
title: Сообщение WM_GESTURENOTIFY (Winuser. h)
description: Дает возможность задать конфигурацию жестов.
ms.assetid: 83c23928-86ce-421d-bb84-5c41a770bf60
keywords:
- сообщение WM_GESTURENOTIFY Windows Touch
topic_type:
- apiref
api_name:
- WM_GESTURENOTIFY
api_location:
- winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5e900e4b607760df16938080a49f97a3ab0cf2ed
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570270"
---
# <a name="wm_gesturenotify-message"></a>\_Сообщение ЖЕСТУРЕНОТИФИ WM

Дает возможность задать конфигурацию жестов.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Не используется.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на [**жестуренотифиструкт**](/windows/win32/api/winuser/ns-winuser-gesturenotifystruct).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Значение должно возвращаться из [дефвиндовпрок](/windows/win32/api/winuser/nf-winuser-defwindowproca).

## <a name="remarks"></a>Remarks

Когда получено сообщение **WM \_ жестуренотифи** , приложение может использовать [**сетжестуреконфиг**](/windows/desktop/api/winuser/nf-winuser-setgestureconfig) для указания получаемых жестов. Это сообщение всегда должно быть собрано с помощью функции [дефвиндовпрок](/windows/win32/api/winuser/nf-winuser-defwindowproca) .

> [!Note]  
> Обработка сообщения **WM \_ жестуренотифи** изменит конфигурацию жестов на время существования окна, а не только на следующий жест.

 

## <a name="examples"></a>Примеры

В следующем примере показано, как включить все жесты. Дополнительные примеры см. в разделе [**сетжестуреконфиг**](/windows/desktop/api/winuser/nf-winuser-setgestureconfig).


```C++
    switch (message)
    {
    case WM_GESTURENOTIFY:
        GESTURECONFIG gc = {0,GC_ALLGESTURES,0};
        BOOL bResult = SetGestureConfig(hWnd,0,1,&gc,sizeof(GESTURECONFIG));
            
        if(!bResult)
        {
            // an error
        }
        return DefWindowProc(hWnd, WM_GESTURENOTIFY, wParam, lParam);
    }
      
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                                               |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/>                                                  |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Уведомления](notifications.md)
</dt> <dt>

[Windows Инструкции по программированию сенсорных жестов](guide-multi-touch-gestures.md)
</dt> <dt>

[**жестуренотифиструкт**](/windows/win32/api/winuser/ns-winuser-gesturenotifystruct)
</dt> <dt>

[**сетжестуреконфиг**](/windows/desktop/api/winuser/nf-winuser-setgestureconfig)
</dt> </dl>

 

