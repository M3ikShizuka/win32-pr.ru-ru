---
title: Сообщение CB_GETEDITSEL (Winuser. h)
description: Возвращает начальные и конечные позиции символов текущего выделения в элементе управления "поле ввода" поля со списком.
ms.assetid: 72b64135-e35a-4f72-9fc7-e6bedf495f23
keywords:
- элементы управления Windows сообщений CB_GETEDITSEL
topic_type:
- apiref
api_name:
- CB_GETEDITSEL
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 319ce4a3c7a5a61903d4fc3bf04eed223e749787
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054796"
---
# <a name="cb_geteditsel-message"></a>\_Сообщение ЖЕТЕДИТСЕЛ CB

Возвращает начальные и конечные позиции символов текущего выделения в элементе управления "поле ввода" поля со списком.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Указатель на значение **DWORD** , получающее начальную точку выделения. Этот параметр может принимать значение **NULL**.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на значение **DWORD** , которое получает конечную точку выделения. Этот параметр может принимать значение **NULL**.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение — это отсчитываемое от нуля значение **типа DWORD** с начальной позицией выбора в [**ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85)) и с конечной позицией первого символа после последнего выбранного символа в [**HIWORD**](/previous-versions/windows/desktop/legacy/ms632657(v=vs.85)).

## <a name="examples"></a>Примеры

В следующем примере кода показаны два способа получения текущего диапазона выбора.


```C++
DWORD start, end;

// Get the range from [out] parameters.
// hwnd is the handle of the combo box control.
SendMessage(hwnd, CB_GETEDITSEL, (WPARAM)&start, (LPARAM)&end;

// Get the range from the return value.
DWORD range = SendMessage(hwnd, CB_GETEDITSEL, NULL, NULL);
start = LOWORD(range);
end = HIWORD(range);
```



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

[**\_СЕТЕДИТСЕЛ CB**](cb-seteditsel.md)
</dt> <dt>

**Другие ресурсы**
</dt> <dt>

[**HIWORD**](/previous-versions/windows/desktop/legacy/ms632657(v=vs.85))
</dt> <dt>

[**ловорд**](/previous-versions/windows/desktop/legacy/ms632659(v=vs.85))
</dt> </dl>

 

