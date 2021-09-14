---
title: Сообщение WM_ASKCBFORMATNAME (Winuser. h)
description: Отправляется в окно просмотра владельцу буфера обмена для запроса имени \_ формата буфера обмена CF овнердисплай.
ms.assetid: eee026ec-58db-41b3-9705-30a17eebbd70
keywords:
- WM_ASKCBFORMATNAME Exchange данных сообщений
topic_type:
- apiref
api_name:
- WM_ASKCBFORMATNAME
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b14a7f2fc2ff57076d6b694061466fd60e09dce0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056124"
---
# <a name="wm_askcbformatname-message"></a>\_Сообщение АСККБФОРМАТНАМЕ WM

Отправляется в окно просмотра владельцу буфера обмена для запроса имени формата буфера обмена [**CF \_ овнердисплай**](standard-clipboard-formats.md) .

Окно получает это сообщение через функцию [**WindowProc**](/previous-versions/windows/desktop/legacy/ms633573(v=vs.85)) .


```C++
#define WM_ASKCBFORMATNAME              0x030C
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Размер (в символах) буфера, на который указывает параметр *lParam* .

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на буфер, который должен получить имя формата буфера обмена.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если приложение обрабатывает это сообщение, оно должно вернуть ноль.

## <a name="remarks"></a>Комментарии

В ответ на это сообщение владелец буфера обмена должен скопировать имя формата, отображаемого владельцем, в указанный буфер, не превышающий размер буфера, указанный параметром *wParam* .

Окно просмотра буфера обмена отправляет это сообщение владельцу буфера обмена, чтобы определить имя формата [**CF \_ овнердисплай**](standard-clipboard-formats.md) , например, чтобы инициализировать список доступных форматов.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                               |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[Общие сведения о буфере обмена](clipboard.md)
</dt> </dl>

 

