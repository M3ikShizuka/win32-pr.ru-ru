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
ms.openlocfilehash: 33337dffee30deb70833d9ac9e0e3a28b58c4e607de1211c4c8a21a805fb013b
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120047594"
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

## <a name="remarks"></a>Remarks

Родительское окно всегда будет получать сообщение [**WM \_ Notify**](wm-notify.md) для этого события, оно не требует отправки маски уведомления с [**\_ SETEVENTMASK EM**](em-seteventmask.md).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

**Ссылки**
</dt> <dt>

[**енсавеклипбоард**](/windows/desktop/api/Richedit/ns-richedit-ensaveclipboard)
</dt> </dl>

 

 





