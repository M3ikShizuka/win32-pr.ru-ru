---
title: Элемент BCC (Сендемаилтипе)
description: Содержит адреса электронной почты, используемые в строке СК сообщения электронной почты.
ms.assetid: c80407d0-3b3f-4efe-91de-7a3a7abc996f
keywords:
- Элемент скрытой планировщик задач
topic_type:
- apiref
api_name:
- Bcc
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: f262b8f5d74018a4622f915def85df5e16108cdb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126886456"
---
# <a name="bcc-sendemailtype-element"></a>Элемент BCC (Сендемаилтипе)

Содержит адреса электронной почты, используемые в строке СК сообщения электронной почты.

``` syntax
<xs:element name="Bcc"
    type="string"
 />
```

Элемент **BCC** определяется сложным типом [**сендемаилтипе**](taskschedulerschema-sendemailtype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                              | Унаследован от                                                           | Описание                                                  |
|--------------------------------------------------------------------------------------|------------------------------------------------------------------------|--------------------------------------------------------------|
| [**SendEmail (actionGroup)**](taskschedulerschema-sendemail-actiongroup-element.md) | [**сендемаилтипе**](taskschedulerschema-sendemailtype-complextype.md) | Представляет действие, которое отправляет сообщение электронной почты.<br/> |



## <a name="remarks"></a>Комментарии

Сведения о разработке на языке C++ см. в разделе [**свойство BCC объекта иемаилактион**](/windows/desktop/api/taskschd/nf-taskschd-iemailaction-get_bcc).

Сведения о разработке сценариев см. в разделе [**емаилактион. BCC**](emailaction-bcc.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





