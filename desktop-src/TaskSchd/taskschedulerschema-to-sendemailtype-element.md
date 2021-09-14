---
title: To (Сендемаилтипе), элемент
description: Содержит адреса электронной почты, на которые будет отправлено электронное письмо.
ms.assetid: bf3aa878-967b-4ebd-9397-a2a499686a9f
keywords:
- В элемент планировщик задач
topic_type:
- apiref
api_name:
- To
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: b9e0643220915ecb1c8f2cd1fe842e0dc3f21d8f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126968601"
---
# <a name="to-sendemailtype-element"></a>To (Сендемаилтипе), элемент

Содержит адреса электронной почты, на которые будет отправлено электронное письмо.

``` syntax
<xs:element name="To"
    type="string"
 />
```

Элемент **to** определяется сложным типом [**сендемаилтипе**](taskschedulerschema-sendemailtype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                              | Унаследован от                                                           | Описание                                                  |
|--------------------------------------------------------------------------------------|------------------------------------------------------------------------|--------------------------------------------------------------|
| [**SendEmail (actionGroup)**](taskschedulerschema-sendemail-actiongroup-element.md) | [**сендемаилтипе**](taskschedulerschema-sendemailtype-complextype.md) | Представляет действие, которое отправляет сообщение электронной почты.<br/> |



## <a name="remarks"></a>Комментарии

Сведения о разработке на языке C++ см. [**в разделе свойство объекта иемаилактион**](/windows/desktop/api/taskschd/nf-taskschd-iemailaction-get_to).

Сведения о разработке сценариев см. в разделе [**EmailAction.to**](emailaction-to.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





