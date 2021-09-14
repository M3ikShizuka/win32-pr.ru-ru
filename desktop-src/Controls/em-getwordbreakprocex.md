---
title: Сообщение EM_GETWORDBREAKPROCEX (RichEdit. h)
description: Извлекает адрес зарегистрированной в настоящий момент расширенной процедуры разбиения по словам для элемента управления расширенного редактирования.
ms.assetid: 391681b6-fba9-4fc8-8778-3b3bd45ee5d6
keywords:
- элементы управления Windows сообщений EM_GETWORDBREAKPROCEX
topic_type:
- apiref
api_name:
- EM_GETWORDBREAKPROCEX
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 890ef921a33dc387b17fddaa504bd15fa61ac505
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054424"
---
# <a name="em_getwordbreakprocex-message"></a>\_Сообщение ЖЕТВОРДБРЕАКПРОЦЕКС EM

Извлекает адрес зарегистрированной в настоящий момент расширенной процедуры разбиения по словам для элемента управления расширенного редактирования.

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

Сообщение возвращает адрес текущей процедуры.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



 

 





