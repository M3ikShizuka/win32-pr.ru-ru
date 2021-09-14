---
title: Сообщение LVM_ISITEMVISIBLE (Коммктрл. h)
description: Указывает, является ли видимым элемент в элементе управления "представление списка". Отправьте это сообщение явным образом или с помощью \_ макроса Иситемвисибле ListView.
ms.assetid: 355be527-e2b9-46be-96a0-951d72216d92
keywords:
- элементы управления Windows сообщений LVM_ISITEMVISIBLE
topic_type:
- apiref
api_name:
- LVM_ISITEMVISIBLE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 2a95116d2d6da6e3554e63a8149c9b91d6c97f76
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126972050"
---
# <a name="lvm_isitemvisible-message"></a>\_Сообщение LVM иситемвисибле

Указывает, является ли видимым элемент в элементе управления "представление списка". Отправьте это сообщение явным образом или с помощью макроса [**\_ иситемвисибле ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_isitemvisible) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* \[ окне\]
</dt> <dd>

Индекс элемента в элементе управления List-View.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если видимое, или **false** в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





