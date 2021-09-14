---
title: Сообщение PBM_SETBKCOLOR (Коммктрл. h)
description: Задает цвет фона на индикаторе выполнения.
ms.assetid: e28af958-babb-4c2e-9202-89b608c22f8e
keywords:
- элементы управления Windows сообщений PBM_SETBKCOLOR
topic_type:
- apiref
api_name:
- PBM_SETBKCOLOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8ddfaf84695221cf998275d76a9d2d67773150da
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167760"
---
# <a name="pbm_setbkcolor-message"></a>\_Сообщение СЕТБККОЛОР PBM

Задает цвет фона на индикаторе выполнения.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Должен равняться нулю.

</dd> <dt>

*lParam* 
</dt> <dd>

Значение **COLORREF** , указывающее новый цвет фона. Укажите \_ значение по умолчанию CLR, чтобы индикатор выполнения использовал цвет фона по умолчанию.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает предыдущий цвет фона или \_ значение по умолчанию CLR, если цвет фона является цветом по умолчанию.

## <a name="remarks"></a>Remarks

Если стили оформления включены, это сообщение не действует.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





