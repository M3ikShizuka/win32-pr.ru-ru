---
title: Сообщение TBM_GETTOOLTIPS (Коммктрл. h)
description: Получает маркер для элемента управления ToolTip, назначенного для TrackBar, если таковой имеется.
ms.assetid: 30efef12-1aec-4635-94a7-1843db404c4f
keywords:
- элементы управления Windows сообщений TBM_GETTOOLTIPS
topic_type:
- apiref
api_name:
- TBM_GETTOOLTIPS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e02b0b757b1aabfef2c9df2e80ca9f96542ba4a1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166467"
---
# <a name="tbm_gettooltips-message"></a>Сообщение ТБМ с \_ ПОДсказками

Получает маркер для элемента управления ToolTip, назначенного для TrackBar, если таковой имеется.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает маркер для элемента управления ToolTip, назначенного для TrackBar, или **значение NULL** , если подсказки не используются. Если элемент управления TrackBar не использует стиль [**\_ подсказок TBS**](trackbar-control-styles.md) , возвращается значение **null**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





