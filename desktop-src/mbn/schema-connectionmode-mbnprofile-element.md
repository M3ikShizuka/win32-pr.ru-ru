---
description: Задает параметр автоматического подключения, используемый для устройства мобильной широкополосной связи.
ms.assetid: 789016d5-47f1-4506-bcb9-1a4019d236fd
title: ConnectionMode (Мбнпрофиле), элемент
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ConnectionMode
api_type:
- Schema
ms.openlocfilehash: d0f2290928fba4be65d39129017a171fbd3d1e66e6ebab715f616e4edec9b13e
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119607144"
---
# <a name="connectionmode-mbnprofile-element"></a>ConnectionMode (Мбнпрофиле), элемент

Элемент **ConnectionMode (мбнпрофиле)** задает параметр автоматического подключения, который будет использоваться для устройства мобильной широкополосной связи.

Этот элемент может иметь одно из следующих значений.



| Значение       | Значение                                                                |
|-------------|------------------------------------------------------------------------|
| документации    | Никогда не подключайтесь к сети автоматически.                            |
| Выбор      | Всегда автоматически подключаться к сети.                           |
| "Авто-Домашняя" | Автоматически подключаться к сети, кроме случаев, когда в роуминге сеть. |



 

Этот элемент может иметь максимум одно вхождение.

Этот обязательный элемент.

``` syntax
<xs:element name="ConnectionMode">
    <xs:simpleType>
        <xs:restriction
            base="string"
        >
            <xs:enumeration
                value="manual"
             />
            <xs:enumeration
                value="auto"
             />
            <xs:enumeration
                value="auto-home"
             />
        </xs:restriction>
    </xs:simpleType>
</xs:element>
```

Элемент **ConnectionMode** определяется элементом [**мбнпрофиле**](schema-mbnprofile-element.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------|
| Минимальная версия клиента<br/> | \[приложения UWP для классических приложений Windows 7 \|\]<br/> |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                         |



## <a name="see-also"></a>См. также

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**мбнпрофиле**](schema-mbnprofile-element.md)
</dt> <dt>

**Возможный непосредственный родительский элемент в экземпляре схемы**
</dt> <dt>

[**мбнпрофиле**](schema-mbnprofile-element.md)
</dt> </dl>

 

 




