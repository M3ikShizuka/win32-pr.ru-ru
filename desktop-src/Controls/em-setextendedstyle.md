---
title: Сообщение EM_SETEXTENDEDSTYLE (Коммктрл. h)
description: Информирует элемент управления "поле ввода" о необходимости установки расширенных стилей. Отправьте это сообщение или используйте макрос Edit \_ сетекстендедстиле.
ms.assetid: 4ca010c3-2c70-41e5-ade4-11e1895fda26
keywords:
- элементы управления Windows сообщений EM_SETEXTENDEDSTYLE
topic_type:
- apiref
api_name:
- EM_SETEXTENDEDSTYLE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 10/19/2018
ms.openlocfilehash: 560b675927b4497810b8d492fd89b5765aa5a2c2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054361"
---
# <a name="em_setextendedstyle-message"></a>\_Сообщение СЕТЕКСТЕНДЕДСТИЛЕ EM

Информирует элемент управления "поле ввода" о необходимости установки расширенных стилей. Отправьте это сообщение или используйте макрос [**Edit \_ сетекстендедстиле**](/windows/desktop/api/Commctrl/nf-commctrl-edit_setextendedstyle).

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Маска, используемая для выбора устанавливаемых стилей.

</dd> <dt>

*lParam* 
</dt> <dd>

Значение, указывающее расширенный стиль. Дополнительные сведения о стилях см. в разделе [Правка Управление расширенными стилями](edit-control-window-extended-styles.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если это сообщение завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Комментарии

Расширенные стили для элемента управления "поле ввода" не имеют никаких действий с расширенными стилями, используемыми с функцией [**CreateWindowEx**](/windows/desktop/api/winuser/nf-winuser-createwindowexa) или функцией [**SetWindowLong**](/windows/desktop/api/winuser/nf-winuser-setwindowlonga).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, версия 1809 \[ только классические приложения\]<br/>                             |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2019\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

