---
title: Сообщение PGM_GETDROPTARGET (Коммктрл. h)
description: Извлекает указатель интерфейса интерфейс IDropTarget элемента управления страничного навигатора. Это сообщение можно отправить явным образом или использовать \_ макрос Жетдроптаржет пейджера.
ms.assetid: 6b548c30-2d32-4372-90e4-346a27dda218
keywords:
- элементы управления Windows сообщений PGM_GETDROPTARGET
topic_type:
- apiref
api_name:
- PGM_GETDROPTARGET
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f1d07add613674166ebc4bf4cba460088e5e95d9704eead5ad382851bf4e79f7
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119985895"
---
# <a name="pgm_getdroptarget-message"></a>\_Сообщение ЖЕТДРОПТАРЖЕТ PGM

Извлекает указатель интерфейса [**интерфейс IDropTarget**](/windows/desktop/api/oleidl/nn-oleidl-idroptarget) элемента управления страничного навигатора. Это сообщение можно отправить явным образом или использовать макрос [**\_ жетдроптаржет пейджера**](/windows/desktop/api/Commctrl/nf-commctrl-pager_getdroptarget) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на указатель [**интерфейс IDropTarget**](/windows/desktop/api/oleidl/nn-oleidl-idroptarget) , получающий указатель интерфейса. Вызов метода [**Release**](/windows/desktop/api/unknwn/nf-unknwn-iunknown-release) с этим указателем, когда он больше не нужен, является обязанностью вызывающего объекта.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение для этого сообщения не используется.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

