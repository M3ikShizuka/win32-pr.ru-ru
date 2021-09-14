---
title: Сообщение BCM_SETDROPDOWNSTATE (Коммктрл. h)
description: Задает раскрывающееся состояние для кнопки с \_ раскрывающимся списком Style тбстиле. Отправляйте это сообщение явным образом или с помощью \_ макроса кнопки сетдропдовнстате.
ms.assetid: 725deff4-0bcb-497d-a6cf-e9c98b05f16e
keywords:
- элементы управления Windows сообщений BCM_SETDROPDOWNSTATE
topic_type:
- apiref
api_name:
- BCM_SETDROPDOWNSTATE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: fc44ec58d40e047708591121f81c84f327ca47c1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170119"
---
# <a name="bcm_setdropdownstate-message"></a>\_Сообщение СЕТДРОПДОВНСТАТЕ BCM

Задает раскрывающееся состояние для кнопки с [**\_ раскрывающимся списком Style тбстиле**](toolbar-control-and-button-styles.md). Отправляйте это сообщение явным образом или с помощью макроса [**кнопки \_ сетдропдовнстате**](/windows/desktop/api/Commctrl/nf-commctrl-button_setdropdownstate) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* \[ окне\]
</dt> <dd>

**Логическое** **значение, истинное** для состояния BST \_ дропдовнпушед, или **false** в противном случае.

</dd> <dt>

*lParam* 
</dt> <dd>

Должен равняться нулю.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если успешно, или **false** в противном случае.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылка**
</dt> <dt>

[Стили кнопок](button-styles.md)
</dt> <dt>

**Основные понятия**
</dt> <dt>

[Типы кнопок](button-types-and-styles.md)
</dt> </dl>

 

 





