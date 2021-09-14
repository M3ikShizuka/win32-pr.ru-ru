---
title: Сообщение PGM_SETBKCOLOR (Коммктрл. h)
description: Задает текущий цвет фона для элемента управления страничного навигатора. Это сообщение можно отправить явным образом или использовать \_ макрос Сетбкколор пейджера.
ms.assetid: 720a25d7-3854-4f28-b227-bafab7b1e8c9
keywords:
- элементы управления Windows сообщений PGM_SETBKCOLOR
topic_type:
- apiref
api_name:
- PGM_SETBKCOLOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: fa9e8dc1c0cad3e60bdde3f3c05d77d8c57b98ca
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167695"
---
# <a name="pgm_setbkcolor-message"></a>\_Сообщение СЕТБККОЛОР PGM

Задает текущий цвет фона для элемента управления страничного навигатора. Это сообщение можно отправить явным образом или использовать макрос [**\_ сетбкколор пейджера**](/windows/desktop/api/Commctrl/nf-commctrl-pager_setbkcolor) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Значение **COLORREF** , содержащее новый цвет фона для элемента управления страничного навигатора.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **COLORREF** , содержащее предыдущий цвет фона.

## <a name="remarks"></a>Remarks

По умолчанию элемент управления страничный навигатор будет использовать цвет значка системной кнопки в качестве цвета фона. Это тот же цвет, который можно извлечь, вызвав [**жетсисколорбруш**](/windows/desktop/api/winuser/nf-winuser-getsyscolorbrush) с \_ бтнфаце Color.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

