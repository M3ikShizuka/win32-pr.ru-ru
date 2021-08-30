---
description: Отправляется непосредственно перед тем, как редактор IME создает строку композиции в результате нажатия клавиши. Окно получает это сообщение через функцию WindowProc.
ms.assetid: 2740d009-8685-4f70-9b01-67b71f4ddcbd
title: Сообщение WM_IME_STARTCOMPOSITION (Winuser. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 2c1c45e429277fc2621956646f2f4d5c1162a5ad516b90fd2d4d1e60ffe01e30
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120086484"
---
# <a name="wm_ime_startcomposition-message"></a>\_Сообщение старткомпоситион редактора IME WM \_

Отправляется непосредственно перед тем, как редактор IME создает строку композиции в результате нажатия клавиши. Окно получает это сообщение через функцию [*WindowProc*](/previous-versions/windows/desktop/legacy/ms633573(v=vs.85)) .


```C++
LRESULT CALLBACK WindowProc(
  HWND  hwnd,                
  WM_IME_STARTCOMPOSITION,  
  WPARAM wParam,            
  LPARAM lParam             
);
```



## <a name="parameters"></a>Параметры

Это сообщение не содержит параметров.

<dl></dl>

## <a name="return-value"></a>Возвращаемое значение

Это сообщение не имеет возвращаемого значения.

## <a name="remarks"></a>Remarks

Это сообщение является уведомлением для окна редактора IME, чтобы открыть его окно композиции. Приложение должно обработать это сообщение, если оно отображает сами символы композиции.

Если приложение создало окно IME, оно должно передать это сообщение в это окно. Функция [**дефвиндовпрок**](/windows/desktop/api/winuser/nf-winuser-defwindowproca) обрабатывает сообщение, передавая его в окно IME по умолчанию.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                               |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Диспетчер метода ввода](input-method-manager.md)
</dt> <dt>

[Сообщения диспетчера методов ввода](input-method-manager-messages.md)
</dt> </dl>

 

 
