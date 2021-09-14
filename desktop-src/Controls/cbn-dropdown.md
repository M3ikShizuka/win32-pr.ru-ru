---
title: Код уведомления CBN_DROPDOWN (Winuser. h)
description: Посылается, когда список поля со списком станет видимым. Родительское окно поля со списком получает этот код уведомления через \_ командное сообщение WM.
ms.assetid: 2ee9bb19-951b-46bb-a90d-1ade92c2d76c
keywords:
- CBN_DROPDOWN кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- CBN_DROPDOWN
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 018dac2a17a656c11ac697836390ee64e55875db
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173891"
---
# <a name="cbn_dropdown-notification-code"></a>\_Код уведомления раскрывающегося списка КБН

Посылается, когда список поля со списком станет видимым. Родительское окно поля со списком получает этот код уведомления через [**\_ командное сообщение WM**](/windows/desktop/menurc/wm-command) .


```C++
CBN_DROPDOWN

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

Этот код уведомления отправляется, только если поле со списком имеет [**\_ раскрывающийся список CBS**](combo-box-styles.md) или стиль [**\_ DROPDOWNLIST**](combo-box-styles.md) .

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

[КБН \_ крупный план](cbn-closeup.md)
</dt> <dt>

**Другие ресурсы**
</dt> <dt>

[**HIWORD**](/previous-versions/windows/desktop/legacy/ms632657(v=vs.85))
</dt> <dt>

[**ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85))
</dt> <dt>

[**\_команда WM**](/windows/desktop/menurc/wm-command)
</dt> </dl>

 

