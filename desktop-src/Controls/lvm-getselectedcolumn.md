---
title: Сообщение LVM_GETSELECTEDCOLUMN (Коммктрл. h)
description: Извлекает целое число, указывающее выбранный столбец.
ms.assetid: 5aba5d96-50fd-439b-9782-fd5d8684b17f
keywords:
- элементы управления Windows сообщений LVM_GETSELECTEDCOLUMN
topic_type:
- apiref
api_name:
- LVM_GETSELECTEDCOLUMN
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 24ffae9a9c7812f025241f5b46f3b1ea61bb88bd
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054067"
---
# <a name="lvm_getselectedcolumn-message"></a>\_Сообщение LVM жетселектедколумн

Извлекает целое число, указывающее выбранный столбец.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение типа **uint** , указывающее выбранный столбец.

## <a name="remarks"></a>Комментарии

> [!Note]  
> Чтобы использовать это сообщение, необходимо указать манифест, указывающий Comclt32.dll версии 6,0. Дополнительные сведения о манифестах см. в разделе [Включение визуальных стилей](cookbook-overview.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





