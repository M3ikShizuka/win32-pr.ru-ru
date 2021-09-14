---
title: Сообщение TVM_GETBKCOLOR (Коммктрл. h)
description: Возвращает текущий цвет фона элемента управления. Это сообщение можно отправить явно или с помощью \_ макроса Жетбкколор TreeView.
ms.assetid: 1b9eea90-54cd-47b9-befa-ec0128a0230f
keywords:
- элементы управления Windows сообщений TVM_GETBKCOLOR
topic_type:
- apiref
api_name:
- TVM_GETBKCOLOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8077bc9655c088aceefe239ed019cc45874d38ff
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165768"
---
# <a name="tvm_getbkcolor-message"></a>\_Сообщение TVM жетбкколор

Возвращает текущий цвет фона элемента управления. Это сообщение можно отправить явно или с помощью макроса [**\_ жетбкколор TreeView**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_getbkcolor) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение [**COLORREF**](/windows/desktop/gdi/colorref) , представляющее текущий цвет фона. Если это значение равно-1, то элемент управления использует системный цвет для цвета фона.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**TVM \_ сетбкколор**](tvm-setbkcolor.md)
</dt> </dl>

 

