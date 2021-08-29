---
title: Сообщение ACM_ISPLAYING (Коммктрл. h)
description: Проверяет, воспроизводится ли ролик с чередованием Audio-Video (AVI). Это сообщение можно отправить явно или использовать \_ макрос анимации.
ms.assetid: ebb0c92a-99d2-49c1-9de1-8bdbd032be3a
keywords:
- элементы управления Windows сообщений ACM_ISPLAYING
topic_type:
- apiref
api_name:
- ACM_ISPLAYING
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: db85d2b25b0f8498c020a78b3e43cfe48877b0cb0b8b77fe33cbb4caa2a3f311
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119079418"
---
# <a name="acm_isplaying-message"></a>ACM \_ воспроизведение сообщения

Проверяет, воспроизводится ли ролик с чередованием Audio-Video (AVI). Это сообщение можно отправить явно или использовать макрос [**анимации. \_**](/windows/desktop/api/Commctrl/nf-commctrl-animate_isplaying)

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

Возвращает ненулевое значение в случае успеха или ноль в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





