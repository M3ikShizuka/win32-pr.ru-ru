---
title: Код уведомления CBEN_INSERTITEM (Коммктрл. h)
description: Посылается при вставке нового элемента в элемент управления. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: caf60156-10d2-4cfb-91c4-def6ee99c471
keywords:
- CBEN_INSERTITEM кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- CBEN_INSERTITEM
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 63ccd05ea75015479ef32415d920bbe639664ac2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127173899"
---
# <a name="cben_insertitem-notification-code"></a>\_Код уведомления кбен INSERTITEM

Посылается при вставке нового элемента в элемент управления. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
CBEN_INSERTITEM

    pNMInfo = (PNMCOMBOBOXEX) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмкомбобоксекс**](/windows/desktop/api/Commctrl/ns-commctrl-nmcomboboxexa) , содержащую сведения о коде уведомления и вставленном элементе.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Приложение, обрабатывающее этот код уведомления, должно возвращать ноль.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





