---
title: Сообщение EM_CANREDO (RichEdit. h)
description: Определяет, есть ли какие либо действия в очереди повторов элемента управления.
ms.assetid: 4a76adc8-f815-4cf7-8742-b7695e5a0f64
keywords:
- элементы управления Windows сообщений EM_CANREDO
topic_type:
- apiref
api_name:
- EM_CANREDO
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ccfb12f8e72bdf5321151cd3a70b74f322a46591
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246874"
---
# <a name="em_canredo-message"></a>\_Сообщение КАНРЕДО EM

Определяет, есть ли какие либо действия в очереди повторов элемента управления.

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

Если в очереди повторов элемента управления есть действия, возвращаемое значение будет ненулевым.

Если очередь повтора пуста, возвращаемое значение равно нулю.

## <a name="remarks"></a>Remarks

Чтобы повторить последнюю операцию отмены, отправьте сообщение о [**\_ возврате EM**](em-redo.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылки**
</dt> <dt>

[**EM \_ жетредонаме**](em-getredoname.md)
</dt> <dt>

[**EM \_ жетундонаме**](em-getundoname.md)
</dt> <dt>

[**\_Повтор EM**](em-redo.md)
</dt> <dt>

[**\_Отмена EM**](em-undo.md)
</dt> </dl>

 

 





