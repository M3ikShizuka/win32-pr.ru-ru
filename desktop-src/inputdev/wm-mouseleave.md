---
title: Сообщение WM_MOUSELEAVE (Winuser. h)
description: Отправляется в окно, когда курсор покидает клиентскую область окна, указанное в предыдущем вызове метода TrackMouseEven.
ms.assetid: b23d24ff-531a-4b6d-8848-f82ac5568995
keywords:
- WM_MOUSELEAVE ввода сообщений с клавиатуры и мыши
topic_type:
- apiref
api_name:
- WM_MOUSELEAVE
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7dc96022e94df7f518b21b1c9a46895fc9204b08
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127346670"
---
# <a name="wm_mouseleave-message"></a>\_Сообщение WM MOUSELEAVE

Отправляется в окно, когда курсор покидает клиентскую область окна, указанное в предыдущем вызове метода [**TrackMouseEven**](/windows/win32/api/winuser/nf-winuser-trackmouseevent).

Окно получает это сообщение через функцию [**WindowProc**](/previous-versions/windows/desktop/legacy/ms633573(v=vs.85)) .


```C++
#define WM_MOUSELEAVE                   0x02A3
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

Если приложение обрабатывает это сообщение, оно должно вернуть ноль.

## <a name="remarks"></a>Remarks

При создании этого сообщения все записи, запрошенные [**TrackMouseEven**](/windows/win32/api/winuser/nf-winuser-trackmouseevent) , отменяются. Приложение должно вызвать **TrackMouseEven** , когда указатель мыши перейдет в окно, если он требует дополнительного отслеживания поведения при наведении указателя мыши.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                               |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылки**
</dt> <dt>

[**Захват**](/windows/win32/api/winuser/nf-winuser-getcapture)
</dt> <dt>

[**сеткаптуре**](/windows/win32/api/winuser/nf-winuser-setcapture)
</dt> <dt>

[**TrackMouseEven**](/windows/win32/api/winuser/nf-winuser-trackmouseevent)
</dt> <dt>

[**TRACKMOUSEEVEN**](/windows/win32/api/winuser/ns-winuser-trackmouseevent)
</dt> <dt>

[**WM \_ нкмауселеаве**](wm-ncmouseleave.md)
</dt> <dt>

**Основные понятия**
</dt> <dt>

[Ввод с помощью мыши](mouse-input.md)
</dt> </dl>

 

