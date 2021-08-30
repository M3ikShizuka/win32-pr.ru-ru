---
title: Код уведомления EN_ALIGN_LTR_EC (Winuser. h)
description: Посылается, когда пользователь изменяет направление элемента управления Правка на слева направо. Родительское окно элемента управления "поле ввода" получает этот код уведомления через \_ командное сообщение WM.
ms.assetid: 231f9d00-c5a5-445e-9176-201fe1c14a0e
keywords:
- EN_ALIGN_LTR_EC кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- EN_ALIGN_LTR_EC
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0d865dc837350644fa3247e2f4769051fd605f9bebcd15f9e053c0c3ff8b126d
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120047874"
---
# <a name="en_align_ltr_ec-notification-code"></a>\_ \_ \_ Код уведомления о выровняйте по правому»

Посылается, когда пользователь изменяет направление элемента управления Правка на слева направо. Родительское окно элемента управления "поле ввода" получает этот код уведомления [**через \_ командное сообщение WM**](/windows/desktop/menurc/wm-command) .


```C++
EN_ALIGN_LTR_EC

    WPARAM wParam;
    LPARAM lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

[**Ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85)) содержит идентификатор элемента управления "поле ввода". [**HIWORD**](/previous-versions/windows/desktop/legacy/ms632657(v=vs.85)) указывает код уведомления.

</dd> <dt>

*lParam* 
</dt> <dd>

Маркер элемента управления редактирования, отправляющего код уведомления.

</dd> </dl>

## <a name="remarks"></a>Remarks

Если в системе установлен двунаправленный язык, например арабский или иврит, можно изменить направление элемента управления редактирования с помощью клавиш CTRL + ЛШИФТ (слева направо) и CTRL + РШИФТ (справа налево).

**Расширенное редактирование:** Этот код уведомления не поддерживается.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**\_команда WM**](/windows/desktop/menurc/wm-command)
</dt> </dl>

 

