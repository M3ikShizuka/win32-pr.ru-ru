---
title: Сложный тип Ексектипе
description: Определяет дочерние элементы и сведения о последовательности элемента exec (actionGroup).
ms.assetid: ab23801a-453d-4fab-8584-30c5c9d57dff
keywords:
- планировщик задач сложного типа Ексектипе
topic_type:
- apiref
api_name:
- execType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 8f6186c15e8bbe059abaa6cc33580fca45286cda
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127259395"
---
# <a name="exectype-complex-type"></a>Сложный тип Ексектипе

Определяет дочерние элементы и сведения о последовательности элемента [**exec (actionGroup)**](taskschedulerschema-exec-actiongroup-element.md) .

``` syntax
<xs:complexType name="execType">
    <xs:complexContent>
        <xs:extension
            base="actionBaseType"
        >
            <xs:all>
                <xs:element name="Command"
                    type="pathType"
                 />
                <xs:element name="Arguments"
                    type="string"
                    minOccurs="0"
                 />
                <xs:element name="WorkingDirectory"
                    type="pathType"
                    minOccurs="0"
                 />
            </xs:all>
        </xs:extension>
    </xs:complexContent>
</xs:complexType>
```

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                           | Тип                                                        | Описание                                                                                                  |
|-----------------------------------------------------------------------------------|-------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|
| [**Аргументы**](taskschedulerschema-arguments-exectype-element.md)               | **строка**                                                  | Задает аргументы, связанные с операцией командной строки. <br/>                              |
| [**Команда**](taskschedulerschema-command-exectype-element.md)                   | [**пастипе**](taskschedulerschema-pathtype-simpletype.md) | Указывает исполняемый файл или документ для запуска.<br/>                                              |
| [**WorkingDirectory**](taskschedulerschema-workingdirectory-exectype-element.md) | [**пастипе**](taskschedulerschema-pathtype-simpletype.md) | Указывает каталог, в котором существует исполняемый файл или файлы, используемые исполняемым объектом.<br/> |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[планировщик задач сложные типы схемы](task-scheduler-schema-complex-types.md)
</dt> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

 





