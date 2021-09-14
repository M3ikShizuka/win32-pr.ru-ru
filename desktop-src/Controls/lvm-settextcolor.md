---
title: Сообщение LVM_SETTEXTCOLOR (Коммктрл. h)
description: Задает цвет текста для элемента управления "представление списка". Это сообщение можно отправить явно или с помощью \_ макроса Сеттекстколор ListView.
ms.assetid: ff90c18b-0cd7-4331-bcd8-61044e891d1f
keywords:
- элементы управления Windows сообщений LVM_SETTEXTCOLOR
topic_type:
- apiref
api_name:
- LVM_SETTEXTCOLOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 64b30c965bd523cd5638c894b47fc4785ffbdd09
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362656"
---
# <a name="lvm_settextcolor-message"></a>\_Сообщение LVM сеттекстколор

Задает цвет текста для элемента управления "представление списка". Это сообщение можно отправить явно или с помощью макроса [**\_ сеттекстколор ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_settextcolor) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Объект [**COLORREF**](/windows/desktop/gdi/colorref) , указывающий новый цвет текста.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если успешно, или **false** в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

