---
title: Сообщение LVM_GETHEADER (Коммктрл. h)
description: Возвращает маркер элемента управления "заголовок", используемый элементом управления "представление списка". Это сообщение можно отправить явным образом или воспользоваться \_ макросом ListView.
ms.assetid: 4708b493-4449-4844-bf0d-e6969bcf0246
keywords:
- элементы управления Windows сообщений LVM_GETHEADER
topic_type:
- apiref
api_name:
- LVM_GETHEADER
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3d53082092118cad373005743849498791f0e1ca
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126972098"
---
# <a name="lvm_getheader-message"></a>\_Сообщение LVM

Возвращает маркер элемента управления "заголовок", используемый элементом управления "представление списка". Это сообщение можно отправить явным образом или воспользоваться макросом [**ListView \_**](/windows/desktop/api/Commctrl/nf-commctrl-listview_getheader) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает маркер элемента управления заголовка.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





