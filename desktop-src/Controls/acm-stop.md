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
ms.openlocfilehash: 210936d102cdf7c55f25106ec5f6dc8e962c3af7679e6c5294ea10b6e833c8f7
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119079408"
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
| Header<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





