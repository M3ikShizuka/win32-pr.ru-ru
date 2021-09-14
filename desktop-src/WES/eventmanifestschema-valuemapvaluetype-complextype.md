---
title: Сложный тип Валуемапвалуетипе
description: Определяет сопоставление между целочисленным значением и строковым значением. | Сложный тип Валуемапвалуетипе
ms.assetid: 8fd3b3ed-5b62-4e2e-b6f9-8e1bf6d83a35
keywords:
- Журнал событий сложных типов Валуемапвалуетипе
topic_type:
- apiref
api_name:
- ValueMapValueType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 197eb7e402068f541dc5a385eca14a631de2488c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127242692"
---
# <a name="valuemapvaluetype-complex-type"></a>Сложный тип Валуемапвалуетипе

Определяет сопоставление между целочисленным значением и строковым значением.

``` syntax
<xs:complexType name="ValueMapValueType"
    mixed="true"
>
    <xs:simpleContent>
        <xs:extension
            base="string"
        >
            <xs:attribute name="value"
                type="UInt32Type"
                use="required"
             />
            <xs:attribute name="message"
                type="strTableRef"
                use="required"
             />
            <xs:attribute name="symbol"
                type="CSymbolType"
                use="optional"
             />
        </xs:extension>
    </xs:simpleContent>
</xs:complexType>
```

## <a name="attributes"></a>Атрибуты



| Имя    | Тип                                                              | Описание                                                                                                                                                                                                                                                                                                    |
|---------|-------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| message | [**стртаблереф**](eventmanifestschema-strtableref-simpletype.md) | Локализованное строковое значение, с которым сопоставляется целочисленное значение. Строка сообщения ссылается на локализованную строку в разделе " [**STRINGTABLE**](eventmanifestschema-stringtable-resources-element.md) " манифеста. <br/>                                                                              |
| символ  | [**ксимболтипе**](eventmanifestschema-csymboltype-simpletype.md) | Символ, используемый для ссылки на карту в приложении. [**Компилятор сообщений (MC.exe)**](message-compiler--mc-exe-.md) использует символ для создания константы для Map в файле заголовка, создаваемого компилятором. Если не указать символ, компилятор создаст его.<br/> |
| value   | [**UInt32Type**](eventmanifestschema-hexint32type-simpletype.md) | Целочисленное значение, сопоставляемое со строковым значением.<br/>                                                                                                                                                                                                                                                       |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



 

 





