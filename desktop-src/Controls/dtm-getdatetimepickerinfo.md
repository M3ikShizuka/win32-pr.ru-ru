---
title: Сообщение DTM_GETDATETIMEPICKERINFO (Коммктрл. h)
description: Возвращает сведения об элементе управления "Выбор даты и времени" (DTP).
ms.assetid: 04847b68-ac45-4b28-8f62-2cd68ffe48d4
keywords:
- элементы управления Windows сообщений DTM_GETDATETIMEPICKERINFO
topic_type:
- apiref
api_name:
- DTM_GETDATETIMEPICKERINFO
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 2398a2543caa6d7104339fb8debd83fcee3ac71f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126892384"
---
# <a name="dtm_getdatetimepickerinfo-message"></a>\_Сообщение DTM жетдатетимепиккеринфо

Возвращает сведения об элементе управления "Выбор даты и времени" (DTP).

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Должен равняться нулю.

</dd> <dt>

*lParam* \[ окне\]
</dt> <dd> Указатель на <a href="/windows/win32/api/commctrl/ns-commctrl-datetimepickerinfo">**датетимепиккеринфо**</a> для получения информации. Вызывающий объект отвечает за выделение памяти для этой структуры. Перед отправкой этого сообщения установите для элемента **кбсизе** структуры значение sizeof (датетимепиккеринфо).</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение не учитывается.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





