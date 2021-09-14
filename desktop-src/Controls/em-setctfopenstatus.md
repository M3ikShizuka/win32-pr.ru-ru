---
title: Сообщение EM_SETCTFOPENSTATUS (RichEdit. h)
description: Открывает или закрывает клавиатуру платформы текстовых служб (TSF).
ms.assetid: 9bdabf5a-93db-4b0e-9528-807d262de866
keywords:
- элементы управления Windows сообщений EM_SETCTFOPENSTATUS
topic_type:
- apiref
api_name:
- EM_SETCTFOPENSTATUS
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: cf4163a415f129dfc5d3f98aa06578d13bb462e5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054366"
---
# <a name="em_setctfopenstatus-message"></a>\_Сообщение СЕТКТФОПЕНСТАТУС EM

Открывает или закрывает клавиатуру платформы текстовых служб (TSF).

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Чтобы включить клавиатуру TSF, используйте **значение true**. Чтобы отключить клавиатуру TSF, используйте **значение false**.

</dd> <dt>

*lParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

В случае успеха это сообщение возвращает **значение true**. В случае неудачи это сообщение возвращает **значение false**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP с пакетом обновления 1 (SP1), \[ только классические приложения\]<br/>                                  |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**EM \_ жетктфопенстатус**](em-getctfopenstatus.md)
</dt> </dl>

 

 





