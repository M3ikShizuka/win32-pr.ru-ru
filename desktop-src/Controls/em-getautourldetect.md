---
title: Сообщение EM_GETAUTOURLDETECT (RichEdit. h)
description: Указывает, включено ли автоматическое обнаружение URL-адресов в элементе управления Rich Edit.
ms.assetid: f723f15c-bf8f-41ab-aef0-bd8f2c0b9e5d
keywords:
- элементы управления Windows сообщений EM_GETAUTOURLDETECT
topic_type:
- apiref
api_name:
- EM_GETAUTOURLDETECT
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d60fc8efdc6e554e379a9381239920cf70ef07ffca22240e62cfc6892ca2e636
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119019952"
---
# <a name="em_getautourldetect-message"></a>\_Сообщение ЖЕТАУТАУРЛДЕТЕКТ EM

Указывает, включено ли автоматическое обнаружение URL-адресов в элементе управления Rich Edit.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Не используется; должно быть равно нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если автоматическое обнаружение URL-адресов активно, возвращается значение 1.

Если автоматическое обнаружение URL-адресов неактивно, возвращается значение 0.

## <a name="remarks"></a>Remarks

Если включено автоматическое обнаружение URL-адресов, Microsoft Rich Edit постоянно проверяет вводимый текст на наличие допустимого URL-адреса. Расширенное редактирование распознает URL-адреса, которые начинаются с этих префиксов:

-   http:
-   file.
-   mailto:
-   адресов
-   https:
-   Протокол
-   Разверните
-   Просперо:
-   Telnet
-   Интернета
-   WAIS
-   невозможно

Расширенное редактирование также распознает имена стандартных путей, начинающихся с \\ \\ . Когда форматируемый текст находит URL-адрес, он изменяет цвет текста URL-адреса, подчеркивает текст и уведомляет клиента по [ \_ ссылке EN](en-link.md).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[\_ссылка EN](en-link.md)
</dt> </dl>

 

 





