---
title: Сообщение TVM_SETTEXTCOLOR (Коммктрл. h)
description: Задает цвет текста элемента управления. Это сообщение можно отправить явно или с помощью \_ макроса Сеттекстколор TreeView.
ms.assetid: eb57dfd5-3e7b-4cda-a659-be9e03470a44
keywords:
- элементы управления Windows сообщений TVM_SETTEXTCOLOR
topic_type:
- apiref
api_name:
- TVM_SETTEXTCOLOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: da0049c2666faccce7879146c78ddecc70825e8b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165616"
---
# <a name="tvm_settextcolor-message"></a>\_Сообщение TVM сеттекстколор

Задает цвет текста элемента управления. Это сообщение можно отправить явно или с помощью макроса [**\_ сеттекстколор TreeView**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_settextcolor) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Значение [**COLORREF**](/windows/desktop/gdi/colorref) , содержащее новый цвет текста. Если этот аргумент равен-1, элемент управления вернется к использованию системного цвета для цвета текста.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **COLORREF** , представляющее предыдущий цвет текста. Если это значение равно-1, элемент управления использует системный цвет для цвета текста.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**TVM \_ жеттекстколор**](tvm-gettextcolor.md)
</dt> </dl>

 

