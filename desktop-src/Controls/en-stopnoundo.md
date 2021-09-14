---
title: Код уведомления EN_STOPNOUNDO (RichEdit. h)
description: Сообщает родительскому окну элемента управления Rich Edit, что произошло действие, для которого элемент управления не может выделить достаточно памяти для сохранения состояния отмены. Форматированный элемент управления "поле ввода" отправляет этот код уведомления в виде \_ сообщения WM notify.
ms.assetid: 5608f6dd-83dc-4712-b485-dd9bc17dea24
keywords:
- EN_STOPNOUNDO кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- EN_STOPNOUNDO
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4ab71e6e1a78c468e6349fc1f42d03e9b68fb043
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054264"
---
# <a name="en_stopnoundo-notification-code"></a>\_Код уведомления EN стопнаундо

Сообщает родительскому окну элемента управления Rich Edit, что произошло действие, для которого элемент управления не может выделить достаточно памяти для сохранения состояния отмены. Форматированный элемент управления "поле ввода" отправляет этот код уведомления в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
EN_STOPNOUNDO

    lpnmhdr = (LPNMHDR) lParam; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Структура [**NMHDR**](/windows/desktop/api/richedit/ns-richedit-nmhdr) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ноль, чтобы продолжить операцию **отмены** .

Чтобы отменить операцию **отмены** , возвращается ненулевое значение.

## <a name="remarks"></a>Комментарии

Родительское окно всегда будет получать сообщение [**WM \_ Notify**](wm-notify.md) для этого события, оно не требует отправки маски уведомления с [**\_ SETEVENTMASK EM**](em-seteventmask.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылки**
</dt> <dt>

[**NMHDR**](/windows/desktop/api/richedit/ns-richedit-nmhdr)
</dt> <dt>

[**\_уведомление WM**](wm-notify.md)
</dt> </dl>

 

 





