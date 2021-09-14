---
title: Сообщение LVM_HASGROUP (Коммктрл. h)
description: Определяет, имеет ли элемент управления "представление списка" указанную группу.
ms.assetid: 0b8a9208-5221-4f66-8b26-7de55afe485f
keywords:
- элементы управления Windows сообщений LVM_HASGROUP
topic_type:
- apiref
api_name:
- LVM_HASGROUP
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: bb05fed8466188aa0025d2128ce64ad7f1512c07
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054058"
---
# <a name="lvm_hasgroup-message"></a>\_Сообщение LVM хасграуп

Определяет, имеет ли элемент управления "представление списка" указанную группу.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Идентификатор группы.</dd> <dt>

*lParam* 
</dt> <dd>Должен иметь **значение NULL**.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если элемент управления "представление списка" имеет указанную группу, или **значение false** в противном случае.

## <a name="remarks"></a>Комментарии

> [!Note]  
> Чтобы использовать это сообщение, необходимо указать манифест, указывающий Comclt32.dll версии 6,0. Дополнительные сведения о манифестах см. в разделе [Включение визуальных стилей](cookbook-overview.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





