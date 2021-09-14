---
title: Код уведомления EN_SAVECLIPBOARD (RichEdit. h)
description: Сообщает родительскому окну элемента управления Rich Edit, что элемент управления закрывается, а буфер обмена содержит сведения. Форматированный элемент управления "поле ввода" отправляет этот код уведомления в виде \_ сообщения WM notify.
ms.assetid: e8b95e80-6494-4153-8e78-ede9ed17c66f
keywords:
- EN_SAVECLIPBOARD кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- EN_SAVECLIPBOARD
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8a1fd7c6e11ed82a7f77483c692dd68f860395c5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054278"
---
# <a name="en_saveclipboard-notification-code"></a>\_Код уведомления EN савеклипбоард

Сообщает родительскому окну элемента управления Rich Edit, что элемент управления закрывается, а буфер обмена содержит сведения. Форматированный элемент управления "поле ввода" отправляет этот код уведомления в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
EN_SAVECLIPBOARD

    penSaveClipboard = (ENSAVECLIPBOARD *) lParam; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Структура [**енсавеклипбоард**](/windows/desktop/api/Richedit/ns-richedit-ensaveclipboard) , содержащая сведения о содержимом буфера обмена.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает нуль, если буфер обмена должен быть доступен другим приложениям.

Если буфер обмена не должен сохраняться, возвращается ненулевое значение.

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

[**енсавеклипбоард**](/windows/desktop/api/Richedit/ns-richedit-ensaveclipboard)
</dt> </dl>

 

 





