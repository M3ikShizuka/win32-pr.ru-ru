---
title: Сообщение MCM_GETCALID (Коммктрл. h)
description: Возвращает идентификатор календаря для данного элемента управления "Календарь". Это сообщение можно отправить явным образом или с помощью \_ макроса монскал жеткалид.
ms.assetid: ecfab4f3-a5af-445d-8b90-243b646524a6
keywords:
- элементы управления Windows сообщений MCM_GETCALID
topic_type:
- apiref
api_name:
- MCM_GETCALID
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: cb4a780d5107a7761d7dcac9b27a7cb01f3de744
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127362568"
---
# <a name="mcm_getcalid-message"></a>\_Сообщение MCM жеткалид

Возвращает идентификатор календаря для данного элемента управления "Календарь". Это сообщение можно отправить явным образом или с помощью макроса [**монскал \_ жеткалид**](/windows/desktop/api/Commctrl/nf-commctrl-monthcal_getcalid) .

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

Идентификатор текущего календаря. Одна из констант [идентификаторов календаря](/windows/desktop/Intl/calendar-identifiers) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

