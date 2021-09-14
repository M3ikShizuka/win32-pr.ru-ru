---
title: Стопонидлинд (Идлесеттингстипе), элемент
description: Указывает, что планировщик задач будет прекращать выполнение задачи, если условие простоя заканчивается до завершения задачи.
ms.assetid: 5e8e4fd9-bba1-4ede-a0b3-9f50feb1b6f3
keywords:
- планировщик задач элемента Стопонидлинд
topic_type:
- apiref
api_name:
- TerminateOnIdleEnd
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: a47a01d7d77f3dd20f055bce8e4bb12fad82c771
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126968610"
---
# <a name="stoponidleend-idlesettingstype-element"></a>Стопонидлинд (Идлесеттингстипе), элемент

Указывает, что планировщик задач будет прекращать выполнение задачи, если условие простоя заканчивается до завершения задачи.

``` syntax
<xs:element name="StopOnIdleEnd"
    type="boolean"
    minOccurs="0"
    default="true"
 />
```

Элемент **стопонидлинд** определяется сложным типом [**идлесеттингстипе**](taskschedulerschema-idlesettingstype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                       | Унаследован от                                                                 | Описание                                                                                       |
|-------------------------------------------------------------------------------|------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|
| [**идлесеттингс**](taskschedulerschema-idlesettings-settingstype-element.md) | [**идлесеттингстипе**](taskschedulerschema-idlesettingstype-complextype.md) | Указывает, как планировщик задач выполняет задачи, когда компьютер находится в состоянии простоя.<br/> |



## <a name="remarks"></a>Комментарии

Сведения о разработке на языке C++ см. в разделе [**свойство стопонидлинд объекта иидлесеттингс**](/windows/desktop/api/taskschd/nf-taskschd-iidlesettings-get_stoponidleend).

Сведения о разработке сценариев см. в разделе [**идлесеттингс. стопонидлинд**](idlesettings-stoponidleend.md).

## <a name="examples"></a>Примеры

Следующий XML-код определяет параметр простоя, указывающий, что задачу не следует выполнять при завершении условия простоя.


```XML
<IdleSettings>
    <StopOnIdleEnd>false</StopOnIdleEnd>
</IdleSettings>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[планировщик задач элементы схемы](task-scheduler-schema-elements.md)
</dt> </dl>

 

 





