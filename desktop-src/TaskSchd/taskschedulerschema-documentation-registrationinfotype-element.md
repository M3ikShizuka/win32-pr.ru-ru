---
title: Элемент Documentation (Регистратионинфотипе)
description: Указывает любую дополнительную документацию для задачи.
ms.assetid: 5f0d2df3-4eef-430b-85a9-602bb29b85c7
keywords:
- Элемент Documentation планировщик задач
topic_type:
- apiref
api_name:
- Documentation
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 3407a6611886f867734dc7f32cd867a2930d3d2b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126891509"
---
# <a name="documentation-registrationinfotype-element"></a>Элемент Documentation (Регистратионинфотипе)

Указывает любую дополнительную документацию для задачи.

``` syntax
<xs:element name="Documentation"
    type="string"
    minOccurs="0"
 />
```

Элемент **Documentation** определяется сложным типом [**регистратионинфотипе**](taskschedulerschema-registrationinfotype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                           | Унаследован от                                                                         | Описание                                                                                                                         |
|-----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------|
| [**регистратионинфо**](taskschedulerschema-registrationinfo-tasktype-element.md) | [**регистратионинфотипе**](taskschedulerschema-registrationinfotype-complextype.md) | Указывает административную информацию о задаче, например автора задачи и дату регистрации задачи.<br/> |



## <a name="remarks"></a>Комментарии

Для приложений со скриптами дополнительная документация по задачам указывается с помощью свойства [**регистратионинфо. Documentation**](registrationinfo-documentation.md) .

Для приложений C++ Дополнительная документация по задачам указывается с помощью свойства [**ирегистратионинфо::D kumentace**](/windows/desktop/api/taskschd/nf-taskschd-iregistrationinfo-get_documentation) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[планировщик задач элементы схемы](task-scheduler-schema-elements.md)
</dt> </dl>

 

 





