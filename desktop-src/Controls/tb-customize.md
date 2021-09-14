---
title: Сообщение TB_CUSTOMIZE (Коммктрл. h)
description: Отображает диалоговое окно Настройка панели инструментов.
ms.assetid: 45249467-d585-4ffd-8bbe-e39739059c40
keywords:
- элементы управления Windows сообщений TB_CUSTOMIZE
topic_type:
- apiref
api_name:
- TB_CUSTOMIZE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: dada0ef195e898b7a46487a2d775e46d6af854ed
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166876"
---
# <a name="tb_customize-message"></a>\_Настраиваемое сообщение (ТБ)

Отображает диалоговое окно **Настройка панели инструментов** .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Должен равняться нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Должен равняться нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Remarks

> [!Note]  
> Панель инструментов должна поддерживать уведомления [ТБН \_ Куеринсерт](tbn-queryinsert.md) и [ТБН \_ куериделете](tbn-querydelete.md) для отображения диалогового окна **Настройка панели инструментов** . Если панель инструментов не обрабатывает эти уведомления, **\_ Настройка ТБ** не влияет.

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





