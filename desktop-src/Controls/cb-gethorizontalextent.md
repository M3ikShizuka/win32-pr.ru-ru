---
title: Сообщение CB_GETHORIZONTALEXTENT (Winuser. h)
description: Возвращает ширину (в пикселях), в которой окно списка можно прокручивать горизонтально (прокручиваемая ширина). Это применимо только в том случае, если в списке есть горизонтальная полоса прокрутки.
ms.assetid: 7c9fff88-2750-4c94-b7f6-6bdd81c224e9
keywords:
- элементы управления Windows сообщений CB_GETHORIZONTALEXTENT
topic_type:
- apiref
api_name:
- CB_GETHORIZONTALEXTENT
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8a2b1fb7c8fe7549360801516364528c9a2ef1f1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054791"
---
# <a name="cb_gethorizontalextent-message"></a>\_Сообщение ЖЕСОРИЗОНТАЛЕКСТЕНТ CB

Возвращает ширину (в пикселях), в которой окно списка можно прокручивать горизонтально (прокручиваемая ширина). Это применимо только в том случае, если в списке есть горизонтальная полоса прокрутки.

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

Возвращаемое значение является прокручиваемой шириной в пикселях.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>Winuser. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_СЕСОРИЗОНТАЛЕКСТЕНТ CB**](cb-sethorizontalextent.md)
</dt> </dl>

 

 





