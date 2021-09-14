---
title: Сообщение TB_SETHOTITEM2 (Коммктрл. h)
description: TB_SETHOTITEM2 сообщение — задает горячий элемент на панели инструментов.
ms.assetid: 43666b1d-1197-452f-aa79-eb0a1a23e5b7
keywords:
- элементы управления Windows сообщений TB_SETHOTITEM2
topic_type:
- apiref
api_name:
- TB_SETHOTITEM2
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7daf67839837adccfbec99bf03fc4dfff97738db
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166611"
---
# <a name="tb_sethotitem2-message"></a>\_Сообщение SETHOTITEM2 ТБ

Задает горячий элемент на панели инструментов.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Индекс элемента, который будет активным. Если это значение равно-1, ни один из элементов не будет активным.

</dd> <dt>

*lParam* 
</dt> <dd>Сочетание \_ флагов хикф XXX. См. <a href="/windows/win32/api/commctrl/ns-commctrl-nmtbhotitem">**нмтбхотитем**</a>.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает индекс предыдущего горячего элемента или значение-1, если элемент не был активным.

## <a name="remarks"></a>Remarks

Поведение этого сообщения не определено для панелей инструментов, не имеющих [**\_ неструктурированного стиля тбстиле**](toolbar-control-and-button-styles.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





