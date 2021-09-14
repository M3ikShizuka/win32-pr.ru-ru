---
title: Код уведомления TCN_GETOBJECT (Коммктрл. h)
description: Посылается элементом управления "Вкладка", когда он имеет \_ \_ Расширенный стиль TCS ex регистердроп, и объект перетаскивается над элементом вкладки в элементе управления. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: 0beddabe-0e97-4fe7-bcf7-adaba0d72dfe
keywords:
- TCN_GETOBJECT кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- TCN_GETOBJECT
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0e442a122397db717b25e71b17487866227476ad
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166172"
---
# <a name="tcn_getobject-notification-code"></a>\_Код уведомления ТКН GetObject

Посылается элементом управления "Вкладка", когда он имеет расширенный стиль [**TCS \_ ex \_ регистердроп**](tab-control-extended-styles.md) , и объект перетаскивается над элементом вкладки в элементе управления. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
TCN_GETOBJECT

    lpnmon = (LPNMOBJECTNOTIFY) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмобжектнотифи**](/windows/win32/api/commctrl/ns-commctrl-nmobjectnotify) , содержащую сведения об элементе вкладки, на который перетаскивается объект, и получает данные, возвращаемые приложением в ответ на это сообщение.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Приложение, обрабатывающее этот код уведомления, должно возвращать ноль.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





