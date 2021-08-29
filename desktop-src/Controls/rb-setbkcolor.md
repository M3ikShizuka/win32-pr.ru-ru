---
title: Сообщение RB_SETBKCOLOR (Коммктрл. h)
description: Задает цвет фона элемента управления главной панели по умолчанию.
ms.assetid: 450a1e16-24f6-4f86-8e46-14009da05efc
keywords:
- элементы управления Windows сообщений RB_SETBKCOLOR
topic_type:
- apiref
api_name:
- RB_SETBKCOLOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8a2fb502558b53603b59cf7f140248a72f1bf3e22366a85a6e8f740066775fb4
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119696604"
---
# <a name="rb_setbkcolor-message"></a>\_Сообщение СЕТБККОЛОР RB

Задает цвет фона элемента управления главной панели по умолчанию.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Значение [**COLORREF**](/windows/desktop/gdi/colorref) , представляющее новый цвет фона по умолчанию.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение [**COLORREF**](/windows/desktop/gdi/colorref) , представляющее предыдущий цвет фона по умолчанию.

## <a name="remarks"></a>Remarks

Цвет фона по умолчанию элемента управления главной панели используется для рисования фона в элементе управления главной панели и всех полос, добавленных после отправки сообщения. Цвет фона по умолчанию для определенного диапазона можно переопределить при добавлении или изменении диапазона, установив \_ флаг рббим Colors в **фмаск** и установив **клрбакк** в структуре [**ребарбандинфо**](/windows/win32/api/commctrl/ns-commctrl-rebarbandinfoa) .

Если стили оформления включены, это сообщение не действует.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**\_ЖЕТБККОЛОР RB**](rb-getbkcolor.md)
</dt> </dl>

 

