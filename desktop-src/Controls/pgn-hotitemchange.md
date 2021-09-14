---
title: Сообщение PGN_HOTITEMCHANGE (Коммктрл. h)
description: Сообщает родительскому окну элемента управления страничного навигатора, что элемент "горячий" (выделенный) изменился. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: 0f59677c-0251-49f4-b909-6fac6d93f354
keywords:
- элементы управления Windows сообщений PGN_HOTITEMCHANGE
topic_type:
- apiref
api_name:
- PGN_HOTITEMCHANGE
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 573f3dd93a6e4b0b3db6682d36804416d6f6f1e5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167664"
---
# <a name="pgn_hotitemchange-message"></a>\_Сообщение ПГН хотитемчанже

Сообщает родительскому окну элемента управления страничного навигатора, что элемент "горячий" (выделенный) изменился. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
PGN_HOTITEMCHANGE

    pnmPGHotItem = (LPNMPGHOTITEM) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмпгхотитем**](/windows/win32/api/commctrl/ns-commctrl-nmpghotitem) , содержащую сведения об этом коде уведомления.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает ноль для выделения элемента или ненулевого значения, чтобы предотвратить выделение.

## <a name="remarks"></a>Remarks

> [!Note]  
> Чтобы использовать этот код уведомления, необходимо указать манифест, указывающий Comclt32.dll версии 6,0. Дополнительные сведения о манифестах см. в разделе [Включение визуальных стилей](cookbook-overview.md).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





