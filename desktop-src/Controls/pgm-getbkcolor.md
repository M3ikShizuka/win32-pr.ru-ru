---
title: Сообщение PGM_GETBKCOLOR (Коммктрл. h)
description: Возвращает текущий цвет фона для элемента управления страничного навигатора. Это сообщение можно отправить явным образом или использовать \_ макрос Жетбкколор пейджера.
ms.assetid: c39ad721-fe39-44e9-8305-67444acc5d65
keywords:
- элементы управления Windows сообщений PGM_GETBKCOLOR
topic_type:
- apiref
api_name:
- PGM_GETBKCOLOR
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4b58b139dd1caafcdefc6893e2b8a5e3312d3e28
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167727"
---
# <a name="pgm_getbkcolor-message"></a>\_Сообщение ЖЕТБККОЛОР PGM

Возвращает текущий цвет фона для элемента управления страничного навигатора. Это сообщение можно отправить явным образом или использовать макрос [**\_ жетбкколор пейджера**](/windows/desktop/api/Commctrl/nf-commctrl-pager_getbkcolor) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **COLORREF** , содержащее текущий цвет фона.

## <a name="remarks"></a>Remarks

По умолчанию элемент управления страничный навигатор будет использовать цвет значка системной кнопки в качестве цвета фона. Это тот же цвет, который можно извлечь, вызвав [**жетсисколорбруш**](/windows/desktop/api/winuser/nf-winuser-getsyscolorbrush) с \_ бтнфаце Color.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

