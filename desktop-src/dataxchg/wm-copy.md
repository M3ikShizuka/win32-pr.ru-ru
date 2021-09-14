---
title: Сообщение WM_COPY (Winuser. h)
description: Приложение отправляет \_ сообщение копии WM в элемент управления или поле со списком, чтобы скопировать текущий выделенный фрагмент в буфер обмена в \_ ТЕКСТОВОМ формате CF.
ms.assetid: dcac3ad3-1e70-4b71-accd-261587224e60
keywords:
- WM_COPY Exchange данных сообщений
topic_type:
- apiref
api_name:
- WM_COPY
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b298248d75b1d25d1bfef8347347fe2f1a6c7916
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056114"
---
# <a name="wm_copy-message"></a>\_Сообщение о копировании WM

Приложение отправляет сообщение **\_ копии WM** в элемент управления или поле со списком, чтобы скопировать текущий выделенный фрагмент в буфер обмена в [**\_ текстовом формате CF**](standard-clipboard-formats.md) .


```C++
#define WM_COPY                         0x0301
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Этот параметр не используется и должен быть равен нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Этот параметр не используется и должен быть равен нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ненулевое значение при успешном выполнении, в противном случае — ноль.

## <a name="remarks"></a>Комментарии

При отправке в поле со списком сообщение **о \_ копировании WM** обрабатывается его элементом управления "поле ввода". Это сообщение не действует при отправке в поле со списком со стилем [**\_ DROPDOWNLIST в CBS**](../controls/combo-box-styles.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                               |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

**Ссылки**
</dt> <dt>

[**WM \_ clear**](wm-clear.md)
</dt> <dt>

[**Вырезание WM \_**](wm-cut.md)
</dt> <dt>

[**\_Вставка WM**](wm-paste.md)
</dt> <dt>

[**\_Отмена изменений WM**](/windows/desktop/Controls/wm-undo)
</dt> <dt>

**Основные понятия**
</dt> <dt>

[Буфер обмена](clipboard.md)
</dt> </dl>

 

