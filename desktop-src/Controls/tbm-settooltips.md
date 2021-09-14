---
title: Сообщение TBM_SETTOOLTIPS (Коммктрл. h)
description: Назначает элемент управления ToolTip элементу управления TrackBar.
ms.assetid: 9bba1084-d04e-4631-a5cc-408849a14eb1
keywords:
- элементы управления Windows сообщений TBM_SETTOOLTIPS
topic_type:
- apiref
api_name:
- TBM_SETTOOLTIPS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e8d60c7e108db926b85e7d9e1167f33c1ed807a0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166407"
---
# <a name="tbm_settooltips-message"></a>\_Сообщение ТБМ сеттултипс

Назначает элемент управления ToolTip элементу управления TrackBar.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Обработчик существующего элемента управления ToolTip.

</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение для этого сообщения не используется.

## <a name="remarks"></a>Remarks

При создании элемента управления TrackBar с помощью стиля [**\_ всплывающих подсказок TBS**](trackbar-control-styles.md) создается элемент управления ToolTip по умолчанию, который отображается рядом с ползунком, отображая текущую положение ползунка.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





