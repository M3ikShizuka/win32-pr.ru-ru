---
title: Сообщение TDM_SET_PROGRESS_BAR_POS (Коммктрл. h)
description: Задает расположение индикатора выполнения в диалоговом окне задачи.
ms.assetid: 82247d70-8527-4195-87af-5c4e5fd1d1a2
keywords:
- элементы управления Windows сообщений TDM_SET_PROGRESS_BAR_POS
topic_type:
- apiref
api_name:
- TDM_SET_PROGRESS_BAR_POS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c68bd3e4bfe8579eb2c6800eb600abc6eb72f704122850982e131ad3109b7517
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120104564"
---
# <a name="tdm_set_progress_bar_pos-message"></a>TDM \_ Задание \_ индикатора \_ выполнения \_ сообщение POS

Задает расположение индикатора выполнения в диалоговом окне задачи.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* \[ окне\]
</dt> <dd>

Значение **типа int** , указывающее новую точку.

</dd> <dt>

*lParam* \[ окне\]
</dt> <dd>

Должен равняться нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает предыдущее расположение.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





