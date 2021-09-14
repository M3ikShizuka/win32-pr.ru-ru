---
title: Сообщение WM_CTLCOLORLISTBOX (Winuser. h)
description: Отправляется в родительское окно списка до того, как система выводит список. Выполнив ответ на это сообщение, родительское окно может задать цвета текста и фона списка с помощью указанного маркера контекста устройства вывода.
ms.assetid: e128e77f-e966-44c4-9f0e-efcf421b6c82
keywords:
- элементы управления Windows сообщений WM_CTLCOLORLISTBOX
topic_type:
- apiref
api_name:
- WM_CTLCOLORLISTBOX
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8e949af76bd05aa9ad3a3e720c89be33cfe76ed8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165223"
---
# <a name="wm_ctlcolorlistbox-message"></a>\_Сообщение КТЛКОЛОРЛИСТБОКС WM

Отправляется в родительское окно списка до того, как система выводит список. Выполнив ответ на это сообщение, родительское окно может задать цвета текста и фона списка с помощью указанного маркера контекста устройства вывода.


```C++
WM_CTLCOLORLISTBOX

    WPARAM wParam;
    LPARAM lParam; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Обрабатывайте контекст устройства для списка.

</dd> <dt>

*lParam* 
</dt> <dd>

Обработайте с списком.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если приложение обрабатывает это сообщение, оно должно возвращать маркер кисти. Система использует кисть для рисования фона списка.

## <a name="remarks"></a>Комментарии

По умолчанию функция [**дефвиндовпрок**](/windows/desktop/api/winuser/nf-winuser-defwindowproca) выбирает системные цвета по умолчанию для списка.

Сообщение **WM \_ ктлколорлистбокс** никогда не передается между потоками. Он отправляется только в пределах одного потока.

Если процедура диалогового окна обрабатывает это сообщение, необходимо привести требуемое возвращаемое значение к типу **int \_ ptr** и вернуть значение напрямую. Если процедура диалогового окна возвращает **значение false**, выполняется обработка сообщений по умолчанию. Значение **\_ мсгресулт DWL** , заданное функцией [**SetWindowLong**](/windows/desktop/api/winuser/nf-winuser-setwindowlonga) , игнорируется.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Другие ресурсы**
</dt> <dt>

[**реализепалетте**](/windows/desktop/api/wingdi/nf-wingdi-realizepalette)
</dt> <dt>

[**селектпалетте**](/windows/desktop/api/wingdi/nf-wingdi-selectpalette)
</dt> <dt>

[**дефвиндовпрок**](/windows/desktop/api/winuser/nf-winuser-defwindowproca)
</dt> </dl>

 

