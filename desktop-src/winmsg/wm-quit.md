---
description: Обозначает запрос на завершение приложения и создается, когда приложение вызывает функцию Посткуитмессаже. Это сообщение приводит к тому, что функция передачи сообщений возвращает ноль.
ms.assetid: a9bff5dc-cab8-4e08-838e-d92c87c265d6
title: Сообщение WM_QUIT (Winuser. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 26f6b999ff23d964c1998fe1cc2a9991e11ecfe71760800b1d678e2f71b89273
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119881524"
---
# <a name="wm_quit-message"></a>\_Сообщение о выходе WM

Обозначает запрос на завершение приложения и создается, когда приложение вызывает функцию [**посткуитмессаже**](/windows/win32/api/winuser/nf-winuser-postquitmessage) . Это сообщение приводит к тому, что функция передачи [**сообщений**](/windows/win32/api/winuser/nf-winuser-getmessage) возвращает ноль.


```C++
#define WM_QUIT                         0x0012
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Код выхода, заданный в функции [**посткуитмессаже**](/windows/win32/api/winuser/nf-winuser-postquitmessage) .

</dd> <dt>

*lParam* 
</dt> <dd>

Этот параметр не используется.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **lResult**

Это сообщение не имеет возвращаемого значения, так как оно приводит к завершению цикла обработки сообщений перед отправкой сообщения в процедуру окна приложения.

## <a name="remarks"></a>Remarks

Сообщение **WM \_ Quit** не связано с окном и, следовательно, никогда не будет получено с помощью оконной процедуры окна. Он извлекается только с помощью функций [**PeekMessage**](/windows/win32/api/winuser/nf-winuser-peekmessagea) или функции WITH [**Message**](/windows/win32/api/winuser/nf-winuser-getmessage) .

Не перемещайте сообщение **WM \_ Quit** с помощью функции [**onmessage**](/windows/win32/api/winuser/nf-winuser-postmessagea) ; используйте [**посткуитмессаже**](/windows/win32/api/winuser/nf-winuser-postquitmessage).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                               |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

**Ссылки**
</dt> <dt>

[**GetMessage**](/windows/win32/api/winuser/nf-winuser-getmessage)
</dt> <dt>

[**PeekMessage**](/windows/win32/api/winuser/nf-winuser-peekmessagea)
</dt> <dt>

[**посткуитмессаже**](/windows/win32/api/winuser/nf-winuser-postquitmessage)
</dt> <dt>

**Зрения**
</dt> <dt>

[Windows](windows.md)
</dt> </dl>

 

 
