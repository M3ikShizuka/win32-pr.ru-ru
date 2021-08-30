---
title: Execution (Системпропертиестипе), элемент
description: Содержит сведения о процессе и потоке, которые зарегистрировали событие.
ms.assetid: 4d2feb0d-a3e6-479c-aa34-cd95a708add5
keywords:
- Журнал событий элемента выполнения
topic_type:
- apiref
api_name:
- Execution
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 1e4b38c5f0fbdbb95925ad6e65aa2ae3ef79f650459210d6bb38a1b917353704
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119904934"
---
# <a name="execution-systempropertiestype-element"></a>Execution (Системпропертиестипе), элемент

Содержит сведения о процессе и потоке, которые зарегистрировали событие.

``` syntax
<xs:element name="Execution">
    <xs:complexType>
        <xs:attribute name="ProcessID"
            type="unsignedInt"
            use="required"
         />
        <xs:attribute name="ThreadID"
            type="unsignedInt"
            use="required"
         />
        <xs:attribute name="ProcessorID"
            type="unsignedByte"
            use="optional"
         />
        <xs:attribute name="SessionID"
            type="unsignedInt"
            use="optional"
         />
        <xs:attribute name="KernelTime"
            type="unsignedInt"
            use="optional"
         />
        <xs:attribute name="UserTime"
            type="unsignedInt"
            use="optional"
         />
        <xs:attribute name="ProcessorTime"
            type="unsignedInt"
            use="optional"
         />
    </xs:complexType>
</xs:element>
```

Элемент **Execution** определяется сложным типом [**системпропертиестипе**](eventschema-systempropertiestype-complextype.md) .

## <a name="attributes"></a>Атрибуты



| Имя          | Тип         | Описание                                                                                               |
|---------------|--------------|-----------------------------------------------------------------------------------------------------------|
| кернелтиме    | unsignedInt  | Затраченное время выполнения инструкций режима ядра в единицах времени ЦП.<br/>                        |
| ProcessID     | unsignedInt  | Указывает процесс, создавший событие.<br/>                                               |
| процессорид   | unsignedByte | Идентификационный номер процессора, который обработал событие.<br/>                          |
| процессортиме | unsignedInt  | Для частных сеансов ETW — затраченное время выполнения инструкций пользовательского режима в тактах ЦП.<br/> |
| SessionID     | unsignedInt  | Идентификационный номер сеанса сервера терминалов, в котором произошло событие.<br/>         |
| ThreadID      | unsignedInt  | Указывает поток, создавший событие.<br/>                                                |
| усертиме      | unsignedInt  | Затраченное время выполнения инструкций пользовательского режима в единицах времени ЦП.<br/>                          |



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**системпропертиестипе**](eventschema-systempropertiestype-complextype.md)
</dt> <dt>

**Возможный непосредственный родительский элемент в экземпляре схемы**
</dt> <dt>

[**Система (EventType)**](eventschema-system-eventtype-element.md)
</dt> </dl>

 

 





