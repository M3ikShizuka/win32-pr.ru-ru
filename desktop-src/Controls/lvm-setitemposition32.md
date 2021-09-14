---
title: Сообщение LVM_SETITEMPOSITION32 (Коммктрл. h)
description: Перемещает элемент в указанную позицию в элементе управления "представление списка" (должен быть в виде значка или маленького значка).
ms.assetid: 77db5fd0-bbc3-47ad-95ef-61ef4ac022bc
keywords:
- элементы управления Windows сообщений LVM_SETITEMPOSITION32
topic_type:
- apiref
api_name:
- LVM_SETITEMPOSITION32
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 450963e4adf5ea2b0644f8d155145ba577efab83
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362688"
---
# <a name="lvm_setitemposition32-message"></a>\_Сообщение LVM SETITEMPOSITION32

Перемещает элемент в указанную позицию в элементе управления "представление списка" (должен быть в виде значка или маленького значка). Это сообщение отличается от сообщения [**LVM \_ сетитемпоситион**](lvm-setitemposition.md) тем, что оно использует 32-разрядные координаты. Это сообщение можно отправить явно или с помощью макроса [**\_ SetItemPosition32 ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_setitemposition32) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Индекс элемента представления списка, для которого задается позиция.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**точек**](/previous-versions//dd162805(v=vs.85)) , содержащую новую позицию элемента, в координатах представления списка.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

