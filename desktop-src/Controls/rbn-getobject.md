---
title: Код уведомления RBN_GETOBJECT (Коммктрл. h)
description: Посылается элементом управления "Главная панель", созданным с помощью \_ стиля RBS регистердроп, при перетаскивании объекта на полосу в элементе управления. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: 057474c1-5f65-4290-973e-4366b760365a
keywords:
- RBN_GETOBJECT кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- RBN_GETOBJECT
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9a390bc5c5f74a577805ca8ae1128fbb24e6b10b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167208"
---
# <a name="rbn_getobject-notification-code"></a>\_Код уведомления РБН GetObject

Посылается элементом управления "Главная панель", созданным с помощью стиля [**RBS \_ регистердроп**](rebar-control-styles.md) , при перетаскивании объекта на полосу в элементе управления. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
RBN_GETOBJECT

    lpnmon = (LPNMOBJECTNOTIFY) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмобжектнотифи**](/windows/win32/api/commctrl/ns-commctrl-nmobjectnotify) , содержащую сведения о полосе, на которую перетаскивается объект, а также данные, предоставленные принимающим приложением в ответ на этот код уведомления.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение для этого кода уведомления должно быть равно нулю.

## <a name="remarks"></a>Remarks

Чтобы получить \_ код уведомления РБН GetObject, инициализируйте OLE с помощью вызова [**Олеинитиализе**](/windows/desktop/api/ole2/nf-ole2-oleinitialize) или [**CoInitialize**](/windows/desktop/api/objbase/nf-objbase-coinitialize).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

