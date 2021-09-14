---
title: Сообщение PGM_GETPOS (Коммктрл. h)
description: Извлекает текущее расположение прокрутки элемента управления страничного навигатора. Это сообщение можно отправить явным образом или использовать \_ макрос Жетпос пейджера.
ms.assetid: 1e0f967a-3290-43b7-b812-8cf56abf2d32
keywords:
- элементы управления Windows сообщений PGM_GETPOS
topic_type:
- apiref
api_name:
- PGM_GETPOS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 611a27e9cb952c5be190fa041af3d238f0184b03
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167700"
---
# <a name="pgm_getpos-message"></a>\_Сообщение ЖЕТПОС PGM

Извлекает текущее расположение прокрутки элемента управления страничного навигатора. Это сообщение можно отправить явным образом или использовать макрос [**\_ жетпос пейджера**](/windows/desktop/api/Commctrl/nf-commctrl-pager_getpos) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение типа INT, содержащее текущую точку прокрутки в пикселях.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





