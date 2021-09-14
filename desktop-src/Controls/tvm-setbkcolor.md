---
title: Сообщение TVM_SETBKCOLOR (Коммктрл. h)
description: Задает цвет фона элемента управления. Это сообщение можно отправить явно или с помощью \_ макроса Сетбкколор TreeView.
ms.assetid: 087f5e0b-ac73-4db4-b82e-15c7641b681c
keywords:
- элементы управления Windows сообщений TVM_SETBKCOLOR
topic_type:
- apiref
api_name:
- TVM_SETBKCOLOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 151aef7aa61e7c66d436d0c90f2481fada017059
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165663"
---
# <a name="tvm_setbkcolor-message"></a>\_Сообщение TVM сетбкколор

Задает цвет фона элемента управления. Это сообщение можно отправить явно или с помощью макроса [**\_ сетбкколор TreeView**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_setbkcolor) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Значение [**COLORREF**](/windows/desktop/gdi/colorref) , содержащее новый цвет фона. Если это значение равно-1, то элемент управления вернется к использованию системного цвета для цвета фона.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение [**COLORREF**](/windows/desktop/gdi/colorref) , представляющее предыдущий цвет фона. Если это значение равно-1, то элемент управления использовал системный цвет для цвета фона.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**TVM \_ жетбкколор**](tvm-getbkcolor.md)
</dt> </dl>

 

