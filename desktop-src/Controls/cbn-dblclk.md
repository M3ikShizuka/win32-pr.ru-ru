---
title: Код уведомления CBN_DBLCLK (Winuser. h)
description: Посылается, когда пользователь дважды щелкает строку в поле со списком. Родительское окно поля со списком получает этот код уведомления через \_ командное сообщение WM.
ms.assetid: 79ca3fd3-4a71-4bd5-be68-efc867a4ad22
keywords:
- CBN_DBLCLK кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- CBN_DBLCLK
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 841c68079572e1740f074034c1a8097ba6a86253
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173895"
---
# <a name="cbn_dblclk-notification-code"></a>\_Код уведомления КБН дблклк

Посылается, когда пользователь дважды щелкает строку в поле со списком. Родительское окно поля со списком получает этот код уведомления через [**\_ командное сообщение WM**](/windows/desktop/menurc/wm-command) .


```C++
CBN_DBLCLK

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

Этот код уведомления имеет место только для полей со списком, [**имеющих \_ простой стиль CBS**](combo-box-styles.md) . В поле со списком, имеющем [**\_ раскрывающийся список CBS**](combo-box-styles.md) или стиль [**\_ DROPDOWNLIST**](combo-box-styles.md) , двойной щелчок не может произойти, поскольку один щелчок закрывает окно списка.

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

**Другие ресурсы**
</dt> <dt>

[**HIWORD**](/previous-versions/windows/desktop/legacy/ms632657(v=vs.85))
</dt> <dt>

[**ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85))
</dt> <dt>

[**\_команда WM**](/windows/desktop/menurc/wm-command)
</dt> </dl>

 

