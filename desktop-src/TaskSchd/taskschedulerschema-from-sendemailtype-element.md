---
title: From (Сендемаилтипе), элемент
description: Содержит адрес электронной почты отправителя электронной почты.
ms.assetid: b80733de-e050-4026-a2fe-f63833ec2660
keywords:
- Из планировщик задач элемента
topic_type:
- apiref
api_name:
- From
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 9f50704212fe6a4fec7ce0fc21bacd7ea33e402c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127259344"
---
# <a name="from-sendemailtype-element"></a>From (Сендемаилтипе), элемент

Содержит адрес электронной почты отправителя электронной почты.

``` syntax
<xs:element name="From"
    type="string"
 />
```

Элемент **from** определяется сложным типом [**сендемаилтипе**](taskschedulerschema-sendemailtype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                              | Унаследован от                                                           | Описание                                                  |
|--------------------------------------------------------------------------------------|------------------------------------------------------------------------|--------------------------------------------------------------|
| [**SendEmail (actionGroup)**](taskschedulerschema-sendemail-actiongroup-element.md) | [**сендемаилтипе**](taskschedulerschema-sendemailtype-complextype.md) | Представляет действие, которое отправляет сообщение электронной почты.<br/> |



## <a name="remarks"></a>Remarks

Для разработки на C++ см. [**свойство From объекта иемаилактион**](/windows/desktop/api/taskschd/nf-taskschd-iemailaction-get_from).

Сведения о разработке сценариев см. [**в разделе емаилактион. from**](emailaction-from.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





