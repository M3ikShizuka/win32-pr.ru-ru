---
title: Сообщение WM_PAINTCLIPBOARD (Winuser. h)
description: Посылается владельцу буфера обмена в окне средства просмотра буфера обмена, если в буфере обмена содержатся данные в \_ формате CF овнердисплай, а клиентская область окна просмотра буфера обмена нуждается в перерисовки.
ms.assetid: 85aeefa5-e3d9-4689-a068-47b59ec7b571
keywords:
- WM_PAINTCLIPBOARD Exchange данных сообщений
topic_type:
- apiref
api_name:
- WM_PAINTCLIPBOARD
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8148af6b513fd1fa956d48f22dc86e618544b073
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056113"
---
# <a name="wm_paintclipboard-message"></a>\_Сообщение ПАИНТКЛИПБОАРД WM

Посылается владельцу буфера обмена в окне средства просмотра буфера обмена, если в буфере обмена содержатся данные в формате [**CF \_ овнердисплай**](standard-clipboard-formats.md) , а клиентская область окна просмотра буфера обмена нуждается в перерисовки.


```C++
#define WM_PAINTCLIPBOARD               0x0309
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Маркер окна средства просмотра буфера обмена.

</dd> <dt>

*lParam* 
</dt> <dd>

Маркер объекта глобальной памяти, который содержит структуру [**PAINTSTRUCT**](/windows/win32/api/winuser/ns-winuser-paintstruct) . Структура определяет часть клиентской области для рисования.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если приложение обрабатывает это сообщение, оно должно вернуть ноль.

## <a name="remarks"></a>Комментарии

Чтобы определить, требуется ли перерисовка всей клиентской области или только ее части, владелец буфера обмена должен сравнить размеры области рисования, заданной в элементе **члене rcpaint структуры** элемента [**PAINTSTRUCT**](/windows/win32/api/winuser/ns-winuser-paintstruct) , с измерениями, заданными в последнем сообщении [**WM \_ сизеклипбоард**](wm-sizeclipboard.md) .

Владелец буфера обмена должен использовать функцию [**глобаллокк**](/windows/desktop/api/winbase/nf-winbase-globallock) для блокировки памяти, содержащей структуру [**PAINTSTRUCT**](/windows/win32/api/winuser/ns-winuser-paintstruct) . Перед возвращением владелец буфера обмена должен разблокировать эту память с помощью функции [**глобалунлокк**](/windows/desktop/api/winbase/nf-winbase-globalunlock) .

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

[**WM \_ сизеклипбоард**](wm-sizeclipboard.md)
</dt> <dt>

**Основные понятия**
</dt> <dt>

[Буфер обмена](clipboard.md)
</dt> </dl>

 

