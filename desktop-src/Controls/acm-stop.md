---
title: Сообщение ACM_STOP (Коммктрл. h)
description: Останавливает воспроизведение фрагмента AVI в элементе управления Animation. Это сообщение можно отправить явным образом или с помощью \_ макроса анимации.
ms.assetid: ba39a579-665e-4d45-8f1f-f190acd76db7
keywords:
- элементы управления Windows сообщений ACM_STOP
topic_type:
- apiref
api_name:
- ACM_STOP
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6e81cfc92ac2778ae559fcd9fb8db2b0cd7bb866
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058132"
---
# <a name="acm_stop-message"></a>Сообщение о фатальной ошибке ACM \_

Останавливает воспроизведение фрагмента AVI в элементе управления Animation. Это сообщение можно отправить явным образом или с помощью макроса [**анимации \_**](/windows/desktop/api/Commctrl/nf-commctrl-animate_stop) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ненулевое значение в случае успеха или ноль в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





