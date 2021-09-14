---
title: Сообщение LVM_SETTOOLTIPS (Коммктрл. h)
description: Задает элемент управления ToolTip, который будет использоваться элементом управления "представление списка" для отображения всплывающих подсказок. Это сообщение можно отправить явным образом или использовать \_ макрос Сеттултипс ListView.
ms.assetid: 5b4335a4-e9f0-4b13-b00b-516af3b60bf1
keywords:
- элементы управления Windows сообщений LVM_SETTOOLTIPS
topic_type:
- apiref
api_name:
- LVM_SETTOOLTIPS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4ff749c24a35cf73de2d75b8a3b516197b57aac4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362652"
---
# <a name="lvm_settooltips-message"></a>\_Сообщение LVM сеттултипс

Задает элемент управления ToolTip, который будет использоваться элементом управления "представление списка" для отображения всплывающих подсказок. Это сообщение можно отправить явным образом или использовать макрос [**\_ сеттултипс ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_settooltips) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Обрабатываемый элемент управления ToolTip.</dd> <dt>

*lParam* 
</dt> <dd>

Должен равняться нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает маркер предыдущего элемента управления ToolTip.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**LVM \_ подсказки**](lvm-gettooltips.md)
</dt> </dl>

 

 





