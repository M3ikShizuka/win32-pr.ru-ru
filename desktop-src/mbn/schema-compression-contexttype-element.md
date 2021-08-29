---
description: Указывает, будет ли использоваться сжатие по каналу данных для заголовка и передачи данных.
ms.assetid: 2aee93e4-d124-43cb-b974-19f00eb4d6a6
title: Элемент Compression (contextType)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Compression
api_type:
- Schema
ms.openlocfilehash: 9715114bc44cebef9f342795e2c46283b8737c2478d9af9bd983deca50d3114e
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119959854"
---
# <a name="compression-contexttype-element"></a>Элемент Compression (contextType)

Элемент **Compression (ContextType)** указывает, будет ли использоваться сжатие по каналу данных для заголовка и передачи данных.

Этот элемент может иметь одно из следующих значений.

| Значение     | Значение                       |
|-----------|-------------------------------|
| ПАРАМЕТР  | Будет использоваться сжатие.     |
| ВКЛЮЧЕН | Сжатие не будет использоваться. |



 

Этот элемент является необязательным. Если этот элемент не указан, то система мобильной широкополосной связи не будет использовать сжатие.

``` syntax
<xs:element name="Compression">
    <xs:simpleType>
        <xs:restriction
            base="token"
        >
            <xs:enumeration
                value="DISABLE"
             />
            <xs:enumeration
                value="ENABLE"
             />
        </xs:restriction>
    </xs:simpleType>
</xs:element>
```

Элемент **Compression** определяется сложным типом [**ContextType**](schema-contexttype-complextype.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------|
| Минимальная версия клиента<br/> | \[приложения UWP для классических приложений Windows 7 \|\]<br/> |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                         |



## <a name="see-also"></a>См. также

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**contextType**](schema-contexttype-complextype.md)
</dt> <dt>

**Возможный непосредственный родительский элемент в экземпляре схемы**
</dt> <dt>

[**Контекст (Мбнпрофиле)**](schema-context-mbnprofile-element.md)
</dt> </dl>

 

 




