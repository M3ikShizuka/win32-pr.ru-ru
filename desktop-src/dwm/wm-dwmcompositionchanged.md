---
title: Сообщение WM_DWMCOMPOSITIONCHANGED (Winuser. h)
description: Информирует все окна верхнего уровня, которые диспетчер окон рабочего стола (DWM) включены или отключены.
ms.assetid: VS|winui|~\winui\windowsuserinterface\windowing\windows\windowreference\windowmessages\wm_dwmcompositionchanged.htm
keywords:
- Сообщение WM_DWMCOMPOSITIONCHANGED диспетчер окон рабочего стола
topic_type:
- apiref
api_name:
- WM_DWMCOMPOSITIONCHANGED
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8ec25f740e1a5d002edec2c1faeaaf068190583c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066120"
---
# <a name="wm_dwmcompositionchanged-message"></a>\_Сообщение ДВМКОМПОСИТИОНЧАНЖЕД WM

Информирует все окна верхнего уровня, которые диспетчер окон рабочего стола (DWM) включены или отключены.

> [!Note]  
> начиная с Windows 8 композиция DWM всегда включена, поэтому это сообщение не отправляется независимо от изменения видеорежима.

 

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Не используется.

</dd> <dt>

*lParam* 
</dt> <dd>

Не используется.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если приложение обрабатывает это сообщение, оно должно вернуть ноль.

## <a name="remarks"></a>Remarks

Окно получает это сообщение через функцию [**WindowProc**](/previous-versions/windows/desktop/legacy/ms633573(v=vs.85)) .

Функцию [**DwmIsCompositionEnabled**](/windows/desktop/api/Dwmapi/nf-dwmapi-dwmiscompositionenabled) можно использовать для определения текущего состояния композиции.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Winuser. h</dt> </dl> |



 

