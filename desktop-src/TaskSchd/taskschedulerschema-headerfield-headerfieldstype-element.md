---
title: Хеадерфиелд (Хеадерфиелдстипе), элемент
description: Содержит поле для заголовка в сообщении электронной почты.
ms.assetid: ec6fc593-8798-4dd0-b589-48657b7cdeb1
keywords:
- планировщик задач элемента Хеадерфиелд
topic_type:
- apiref
api_name:
- HeaderField
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 1f7ac79a16bb0464f6e81d90eba38384a3c2b483
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127259328"
---
# <a name="headerfield-headerfieldstype-element"></a>Хеадерфиелд (Хеадерфиелдстипе), элемент

Содержит поле для заголовка в сообщении электронной почты.

``` syntax
<xs:element name="HeaderField"
    type="headerFieldType"
 />
```

Элемент **хеадерфиелд** определяется сложным типом [**хеадерфиелдстипе**](taskschedulerschema-headerfieldstype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                        | Унаследован от                                                                 | Описание                                                                                      |
|--------------------------------------------------------------------------------|------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| [**хеадерфиелдс**](taskschedulerschema-headerfields-sendemailtype-element.md) | [**хеадерфиелдстипе**](taskschedulerschema-headerfieldstype-complextype.md) | Задает поля заголовка и их значения, используемые в заголовке сообщения электронной почты.<br/> |



## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                            | Тип                                                                    | Описание                                                            |
|--------------------------------------------------------------------|-------------------------------------------------------------------------|------------------------------------------------------------------------|
| [**Безымян**](taskschedulerschema-name-headerfieldtype-element.md)   | [**нонемптистринг**](taskschedulerschema-nonemptystring-simpletype.md) | Задает имя поля заголовка в сообщении электронной почты.<br/> |
| [**Значение**](taskschedulerschema-value-headerfieldtype-element.md) | **строка**                                                              | Задает значение поля заголовка в сообщении электронной почты.<br/>  |



## <a name="remarks"></a>Remarks

Сведения о разработке на языке C++ см. в разделе [**свойство хеадерфиелдс объекта иемаилактион**](/windows/desktop/api/taskschd/nf-taskschd-iemailaction-get_headerfields).

Сведения о разработке сценариев см. в разделе [**емаилактион. хеадерфиелдс**](emailaction-headerfields.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





