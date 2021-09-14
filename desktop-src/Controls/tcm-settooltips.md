---
title: Сообщение TCM_SETTOOLTIPS (Коммктрл. h)
description: Назначает элемент управления ToolTip элементу управления "Вкладка". Это сообщение можно отправить явным образом или с помощью \_ макроса табктрл сеттултипс.
ms.assetid: c1b173b1-9da6-441a-a2b6-3875e2c343f8
keywords:
- элементы управления Windows сообщений TCM_SETTOOLTIPS
topic_type:
- apiref
api_name:
- TCM_SETTOOLTIPS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 25e00166fb97c49c33b22811d28b79165bed4e9b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166187"
---
# <a name="tcm_settooltips-message"></a>\_Сообщение СЕТТУЛТИПС TCM

Назначает элемент управления ToolTip элементу управления "Вкладка". Это сообщение можно отправить явным образом или с помощью макроса [**табктрл \_ сеттултипс**](/windows/desktop/api/Commctrl/nf-commctrl-tabctrl_settooltips) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Обработчик для элемента управления ToolTip.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Remarks

Элемент управления ToolTip, связанный с элементом управления "Вкладка", можно получить с помощью сообщения [**TCM- \_ ToolTips**](tcm-gettooltips.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





