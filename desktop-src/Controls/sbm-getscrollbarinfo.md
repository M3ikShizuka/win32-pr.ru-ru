---
title: Сообщение SBM_GETSCROLLBARINFO (Winuser. h)
description: Отправляется приложением для получения сведений об указанной полосе прокрутки.
ms.assetid: db6f704f-99ee-448c-ae7a-dd5a23399fb6
keywords:
- элементы управления Windows сообщений SBM_GETSCROLLBARINFO
topic_type:
- apiref
api_name:
- SBM_GETSCROLLBARINFO
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b8bdd78eb665bd069d854538bb2bdfae1a946765
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167080"
---
# <a name="sbm_getscrollbarinfo-message"></a>\_Сообщение СБМ жетскроллбаринфо

Отправляется приложением для получения сведений об указанной полосе прокрутки.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**скроллбаринфо**](/windows/win32/api/winuser/ns-winuser-scrollbarinfo) , которая получает сведения.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ненулевое значение в случае успеха или ноль в противном случае.

Дополнительные сведения об ошибке можно получить, вызвав [**GetLastError**](/windows/desktop/api/errhandlingapi/nf-errhandlingapi-getlasterror).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылка**
</dt> <dt>

[**жетскроллбаринфо**](/windows/desktop/api/Winuser/nf-winuser-getscrollbarinfo)
</dt> <dt>

[**скроллбаринфо**](/windows/win32/api/winuser/ns-winuser-scrollbarinfo)
</dt> </dl>

 

