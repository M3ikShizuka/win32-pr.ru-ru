---
description: задает состояния автоскрытия и always on в верхней части Windows панели задач.
title: Сообщение ABM_SETSTATE (Шеллапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.assetid: a60e156d-19ef-49b9-83fc-138d1a2169f2
api_name:
- ABM_SETSTATE
api_type:
- HeaderDef
api_location:
- Shellapi.h
topic_type:
- APIRef
- kbSyntax
ms.openlocfilehash: 3cd21ca49d1a57d870c26e010420f978f1d9b88a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127346379"
---
# <a name="abm_setstate-message"></a>\_Сообщение АБМ SETSTATE

задает состояния автоскрытия и always on в верхней части Windows панели задач.


```C++
SHAppBarMessage(ABM_SETSTATE, pabd); 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пабд* 
</dt> <dd>

Указатель на структуру [**аппбардата**](/windows/desktop/api/Shellapi/ns-shellapi-appbardata) . При отправке этого сообщения необходимо указать элементы **кбсизе** и **HWND** . Данные для требуемого состояния отправляются в член **lParam** с помощью одного из следующих значений.

<dt>

<span id="0"></span>

<span id="0"></span>**0,0**


</dt> <dd>

Автоскрытие и постоянное выключение в начало

</dd> <dt>

<span id="ABS_ALWAYSONTOP"></span><span id="abs_alwaysontop"></span>

<span id="ABS_ALWAYSONTOP"></span><span id="abs_alwaysontop"></span>**ABS \_ алвайсонтоп**


</dt> <dd>

Always On-On — Автоскрытие отключено

</dd> <dt>

<span id="ABS_AUTOHIDE"></span><span id="abs_autohide"></span>

<span id="ABS_AUTOHIDE"></span><span id="abs_autohide"></span>**Автоскрытие ABS \_**


</dt> <dd>

Автоматическое скрытие вкл., всегда включено — сверху

</dd> <dt>

<span id="ABS_AUTOHIDE___ABS_ALWAYSONTOP"></span><span id="abs_autohide___abs_alwaysontop"></span>

<span id="ABS_AUTOHIDE___ABS_ALWAYSONTOP"></span><span id="abs_autohide___abs_alwaysontop"></span>**\_АВТОскрытие ABS \| \_ алвайсонтоп**


</dt> <dd>

Автоскрытие и постоянное включение в начало

</dd> </dl> </dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Всегда возвращает **значение true**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Шеллапи. h</dt> </dl> |



 

 




