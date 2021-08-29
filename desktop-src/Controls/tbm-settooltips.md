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
ms.openlocfilehash: a17aad8324946a96ab47344c2edc05abf76e02fba64a459b85f4af7b924bc7a6
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119261394"
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

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





