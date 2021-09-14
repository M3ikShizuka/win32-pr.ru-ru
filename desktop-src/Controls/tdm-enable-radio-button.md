---
title: Сообщение TDM_ENABLE_RADIO_BUTTON (Коммктрл. h)
description: Включает или отключает переключатель в диалоговом окне задачи.
ms.assetid: da605ce0-b2d5-481a-a0e1-628ae5b65726
keywords:
- элементы управления Windows сообщений TDM_ENABLE_RADIO_BUTTON
topic_type:
- apiref
api_name:
- TDM_ENABLE_RADIO_BUTTON
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a78445158c5edc920eb329cdfc52d44f9cb7d6f3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166144"
---
# <a name="tdm_enable_radio_button-message"></a>TDM \_ включить \_ сообщение переключателя \_

Включает или отключает переключатель в диалоговом окне задачи.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* \[ окне\]
</dt> <dd>

Значение **типа int** , указывающее идентификатор переключателя, который должен быть включен или отключен.

</dd> <dt>

*lParam* \[ окне\]
</dt> <dd>

Указывает состояние кнопки. Задайте значение 0, чтобы отключить кнопку. Задайте для параметра значение ненулевой, чтобы включить кнопку.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение игнорируется.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





