---
title: Код уведомления RBN_CHEVRONPUSHED (Коммктрл. h)
description: Посылается элементом управления "Главная панель" при нажатии шеврона. Этот код уведомления отправляется в виде \_ сообщения WM notify.
ms.assetid: 58aa2c9d-8ab6-46ee-b32f-5c04fb7afa84
keywords:
- RBN_CHEVRONPUSHED кода уведомления Windows элементы управления
topic_type:
- apiref
api_name:
- RBN_CHEVRONPUSHED
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ab28d992b6d4a617b7aa7ee144eb50aef3b0e834
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127167235"
---
# <a name="rbn_chevronpushed-notification-code"></a>\_Код уведомления РБН чевронпушед

Посылается элементом управления "Главная панель" при нажатии шеврона. Этот код уведомления отправляется в виде сообщения [**WM \_ Notify**](wm-notify.md) .


```C++
RBN_CHEVRONPUSHED

    lpnm = (NMREBARCHEVRON) lParam;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**нмребарчеврон**](/windows/win32/api/commctrl/ns-commctrl-nmrebarchevron) полосы.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение для этого уведомления не используется.

## <a name="remarks"></a>Remarks

Когда приложение получает этот код уведомления, оно отвечает за отображение всплывающего меню с элементами для каждого скрытого инструмента. Используйте элемент **RC** структуры [**нмребарчеврон**](/windows/win32/api/commctrl/ns-commctrl-nmrebarchevron) , чтобы найти правильную точку для всплывающего меню.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





