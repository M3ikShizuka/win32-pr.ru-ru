---
title: Элемент File (Аттачментстипе)
description: Содержит путь к файлу, отправленному в виде вложения в сообщение электронной почты.
ms.assetid: a53f591b-ac59-43b4-8cc2-661e76d307cc
keywords:
- планировщик задач элемента File
topic_type:
- apiref
api_name:
- File
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: ed07d4b31f9054f6caefcff0585d9683faa90c7f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127259352"
---
# <a name="file-attachmentstype-element"></a>Элемент File (Аттачментстипе)

Содержит путь к файлу, отправленному в виде вложения в сообщение электронной почты.

``` syntax
<xs:element name="File"
    type="nonEmptyString"
 />
```

Элемент **File** определяется сложным типом [**аттачментстипе**](taskschedulerschema-attachmentstype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                                      | Унаследован от                                                               | Описание                                                     |
|----------------------------------------------------------------------------------------------|----------------------------------------------------------------------------|-----------------------------------------------------------------|
| [**Вложения (Сендемаилтипе)**](taskschedulerschema-attachments-sendemailtype-element.md) | [**аттачментстипе**](taskschedulerschema-attachmentstype-complextype.md) | Содержит список вложений в сообщении электронной почты.<br/> |



## <a name="remarks"></a>Remarks

Сведения о разработке на языке C++ см. в разделе [**свойство вложений иемаилактион**](/windows/desktop/api/taskschd/nf-taskschd-iemailaction-get_attachments).

Сведения о разработке сценариев см. в разделе [**емаилактион. вложениям**](emailaction-attachments.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





