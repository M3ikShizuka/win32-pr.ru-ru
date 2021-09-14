---
title: Сообщение TCM_GETTOOLTIPS (Коммктрл. h)
description: Получает маркер для элемента управления ToolTip, связанного с элементом управления "Вкладка". Это сообщение можно отправить явным образом или с помощью \_ макроса табктрл.
ms.assetid: d7dcca4f-8629-4eeb-844f-b3171438f528
keywords:
- элементы управления Windows сообщений TCM_GETTOOLTIPS
topic_type:
- apiref
api_name:
- TCM_GETTOOLTIPS
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4e49334a1fa7124dd6e7a0f0b739cd1ebd24b51b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166244"
---
# <a name="tcm_gettooltips-message"></a>\_Сообщение о подсказках TCM

Получает маркер для элемента управления ToolTip, связанного с элементом управления "Вкладка". Это сообщение можно отправить явным образом или с помощью макроса [**табктрл \_**](/windows/desktop/api/Commctrl/nf-commctrl-tabctrl_gettooltips) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает маркер для элемента управления ToolTip, если он успешно, или **значение NULL** в противном случае.

## <a name="remarks"></a>Remarks

Элемент управления "Вкладка" создает элемент управления ToolTip, если он имеет стиль [**\_ подсказок TCS**](tab-control-styles.md) . Элемент управления ToolTip можно также назначить элементу управления "Вкладка" с помощью сообщения [**TCM \_ сеттултипс**](tcm-settooltips.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





