---
title: Сообщение LVM_SETINSERTMARKCOLOR (Коммктрл. h)
description: Задает цвет точки вставки.
ms.assetid: dce2c266-672b-4682-ba23-51d9a8e1102b
keywords:
- элементы управления Windows сообщений LVM_SETINSERTMARKCOLOR
topic_type:
- apiref
api_name:
- LVM_SETINSERTMARKCOLOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 260d21d083e2c70d8e82a27628e42596bd1b37eb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362704"
---
# <a name="lvm_setinsertmarkcolor-message"></a>\_Сообщение LVM сетинсертмаркколор

Задает цвет точки вставки.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Структура **COLORREF** , указывающая цвет для установки точки вставки.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает структуру **COLORREF** , установленную на предыдущий цвет.

## <a name="remarks"></a>Комментарии

> [!Note]  
> Чтобы использовать это сообщение, необходимо указать манифест, указывающий Comclt32.dll версии 6,0. Дополнительные сведения о манифестах см. в разделе [Включение визуальных стилей](cookbook-overview.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





