---
title: Сообщение PGM_RECALCSIZE (Коммктрл. h)
description: Заставляет элемент управления страничного навигатора повторно вычислить размер автономного окна. Отправка этого сообщения приведет к \_ отправке уведомления ПГН калксизе. Это сообщение можно отправить явным образом или использовать \_ макрос Рекалксизе пейджера.
ms.assetid: 51b75ce8-2b41-4f1a-830e-b25e7d77dccb
keywords:
- элементы управления Windows сообщений PGM_RECALCSIZE
topic_type:
- apiref
api_name:
- PGM_RECALCSIZE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 099f17af0cc4edc79df01fcb03864cdbf2879ae75df701f30f32610a50ae884d
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119540544"
---
# <a name="pgm_recalcsize-message"></a>\_Сообщение РЕКАЛКСИЗЕ PGM

Заставляет элемент управления страничного навигатора повторно вычислить размер автономного окна. Отправка этого сообщения приведет к отправке уведомления [ПГН \_ калксизе](pgn-calcsize.md) . Это сообщение можно отправить явным образом или использовать макрос [**\_ рекалксизе пейджера**](/windows/desktop/api/Commctrl/nf-commctrl-pager_recalcsize) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение не используется.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





