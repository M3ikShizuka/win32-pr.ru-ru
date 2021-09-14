---
title: Код уведомления CBN_SELENDOK (Winuser. h)
description: Посылается, когда пользователь выбирает элемент списка или выбирает элемент, а затем закрывает список. Указывает, что выбор пользователя должен быть обработан. Родительское окно поля со списком получает этот код уведомления через \_ командное сообщение WM.
ms.assetid: ef0ac46f-2db9-40d6-ba82-7e90d71fdd37
keywords:
- CBN_SELENDOK кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- CBN_SELENDOK
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8a0b04fcce0ec2b3f6a2bf5b5e04fa4110ad6ceb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173864"
---
# <a name="cbn_selendok-notification-code"></a>\_Код уведомления КБН селендок

Посылается, когда пользователь выбирает элемент списка или выбирает элемент, а затем закрывает список. Указывает, что выбор пользователя должен быть обработан. Родительское окно поля со списком получает этот код уведомления через [**\_ командное сообщение WM**](/windows/desktop/menurc/wm-command) .


```C++
CBN_SELENDOK

    WPARAM wParam;
    LPARAM lParam; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

[**Ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85)) содержит идентификатор элемента управления поля со списком. [**HIWORD**](/previous-versions/windows/desktop/legacy/ms632657(v=vs.85)) указывает код уведомления.

</dd> <dt>

*lParam* 
</dt> <dd>

Обработайте с полем со списком.

</dd> </dl>

## <a name="remarks"></a>Remarks

В поле со списком с [**\_ простым**](combo-box-styles.md) стилем CBS \_ код уведомления КБН селендок отправляется непосредственно перед каждым кодом уведомления [КБН \_ селчанже](cbn-selchange.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылки**
</dt> <dt>

[КБН \_ селчанже](cbn-selchange.md)
</dt> <dt>

[КБН \_ селендканцел](cbn-selendcancel.md)
</dt> <dt>

**Другие ресурсы**
</dt> <dt>

[**HIWORD**](/previous-versions/windows/desktop/legacy/ms632657(v=vs.85))
</dt> <dt>

[**ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85))
</dt> <dt>

[**\_команда WM**](/windows/desktop/menurc/wm-command)
</dt> </dl>

 

