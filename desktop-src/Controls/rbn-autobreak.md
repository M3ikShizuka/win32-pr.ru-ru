---
title: Сообщение RBN_AUTOBREAK (Коммктрл. h)
description: Уведомляет родительский элемент главной панели о том, что на панели появится разрыв. Родительский элемент определяет, следует ли сделать перерыв. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: b7a63027-6cfa-4d5a-9ea6-fdd8b4fb6864
keywords:
- элементы управления Windows сообщений RBN_AUTOBREAK
topic_type:
- apiref
api_name:
- RBN_AUTOBREAK
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d614277d89578cb66e528ba16656ed55681ebbcf
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167244"
---
# <a name="rbn_autobreak-message"></a>\_Сообщение об АВТОразрыве РБН

Уведомляет родительский элемент [главной панели](rebar-controls.md) о том, что на панели появится разрыв. Родительский элемент определяет, следует ли сделать перерыв. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
RBN_AUTOBREAK

    pnmRebarAutoBreak = (LPNMREBARAUTOBREAK) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмребараутобреак**](/windows/win32/api/commctrl/ns-commctrl-nmrebarautobreak) , содержащую сведения о коде уведомления.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение для этого уведомления не используется.

## <a name="remarks"></a>Remarks

Значение элемента **фаутобреак** структуры [**нмребараутобреак**](/windows/win32/api/commctrl/ns-commctrl-nmrebarautobreak) указывает, должно ли в главной панели произойти прерывание.

Чтобы использовать этот код уведомления, укажите Comctl32.dll версии 6 в манифесте. Дополнительные сведения о манифестах см. в разделе [Включение визуальных стилей](cookbook-overview.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





