---
title: Сообщение LVM_GETHOTITEM (Коммктрл. h)
description: Извлекает индекс горячего элемента. Это сообщение можно отправить явным образом или использовать \_ макрос Жесотитем ListView.
ms.assetid: f80189da-6c8b-4faf-925a-0c33fedf8c4e
keywords:
- элементы управления Windows сообщений LVM_GETHOTITEM
topic_type:
- apiref
api_name:
- LVM_GETHOTITEM
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 56c7bbfb845518eb40b55556df5294d59cff3d7c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054084"
---
# <a name="lvm_gethotitem-message"></a>\_Сообщение LVM жесотитем

Извлекает индекс горячего элемента. Это сообщение можно отправить явным образом или использовать макрос [**\_ жесотитем ListView**](/windows/desktop/api/Commctrl/nf-commctrl-listview_gethotitem) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает индекс неактивного элемента.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





