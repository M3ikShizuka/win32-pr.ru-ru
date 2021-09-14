---
title: Элемент Command (Ексектипе)
description: Указывает исполняемый файл или документ для запуска.
ms.assetid: dedf8627-926c-43c6-8add-21ff298d697a
keywords:
- Элемент Command планировщик задач
topic_type:
- apiref
api_name:
- Command
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: c9d27eb5b40d652035882efc311d9735bcbdd23e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064510"
---
# <a name="command-exectype-element"></a>Элемент Command (Ексектипе)

Указывает исполняемый файл или документ для запуска.

``` syntax
<xs:element name="Command"
    type="pathType"
 />
```

Элемент **Command** определяется сложным типом [**ексектипе**](taskschedulerschema-exectype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                      | Унаследован от                                                 | Описание                                                            |
|--------------------------------------------------------------|--------------------------------------------------------------|------------------------------------------------------------------------|
| [**Exec**](taskschedulerschema-exec-actiongroup-element.md) | [**ексектипе**](taskschedulerschema-exectype-complextype.md) | Указывает действие, выполняющее операцию командной строки.<br/> |



## <a name="remarks"></a>Remarks

Сведения о разработке на языке C++ см. в описании [**свойства arguments объекта иексекактион**](/windows/desktop/api/taskschd/nf-taskschd-iexecaction-get_arguments).

Сведения о разработке скриптов см. в разделе [**ексекактион. Arguments**](execaction-arguments.md).

## <a name="examples"></a>Примеры

Полный пример XML-кода для задачи, использующей исполняемое действие, см. в разделе [пример триггера времени (XML)](time-trigger-example--xml-.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[планировщик задач элементы схемы](task-scheduler-schema-elements.md)
</dt> </dl>

 

 





