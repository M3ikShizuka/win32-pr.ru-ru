---
title: noncreatable - атрибут
description: Атрибут \ "\ несоздаваемый \" определяет объект, который не может быть создан самим по себе.
ms.assetid: 75d7b978-0f82-4e8a-89c2-ffd5b9a691d6
keywords:
- несоздаваемый атрибут MIDL
topic_type:
- apiref
api_name:
- noncreatable
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c2aa54be3416087c06651a4bb58902a0469e8f0c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127143566"
---
# <a name="noncreatable-attribute"></a>noncreatable - атрибут

**\[ Несоздаваемый \]** атрибут определяет объект, который не может быть создан самим по себе.

``` syntax
[
  coclass-attribute-list, 
    noncreatable
]
coclass coclass-name
{
  coclass-interface-list
}
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*Список атрибутов coclass* 
</dt> <dd>

Другие атрибуты, которые применяются к классу.

</dd> <dt>

*имя класса* 
</dt> <dd>

Имя класса.

</dd> <dt>

*coclass-интерфейс-список* 
</dt> <dd>

Список интерфейсов для класса.

</dd> </dl>

## <a name="remarks"></a>Remarks

Используйте **\[ несоздаваемый \]** атрибут в операторе [**coclass**](coclass.md) , чтобы указать пользователям, что они не могут создать новый объект этого класса на верхнем уровне, то есть путем вызова **CreateInstance** **или CoCreateInstance**. Для создания экземпляра объекта этого класса требуется вызов метода другого объекта. например, в Microsoft Excel объект "Cell" является несоздаваемым и должен быть получен из объекта листа Microsoft Excel.

Методы, возвращающие экземпляры несоздаваемых классов, должны возвращать точный тип объекта, а не типы **Variant** или **IDispatch** \* .

### <a name="typeflag-representation"></a>Типефлаг:

Отсутствие ТИПЕФЛАГ \_ фканкреате.

## <a name="examples"></a>Примеры

``` syntax
[
    uuid(12345678-1234-1234-1234-123456789ABC),
    helpstring("This is MyCOClass"),
    noncreatable
]
coclass MyCoClass
{
    [default] interface IMyClass;
    [default, source] dispinterface IMyClassEvents;
}
```

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**кокласс**](coclass.md)
</dt> <dt>

[Синтаксис файла ODL](/previous-versions/windows/desktop/automat/odl-file-syntax)
</dt> <dt>

[Пример файла ODL](/previous-versions/windows/desktop/automat/odl-file-example)
</dt> <dt>

[Создание библиотеки типов с помощью MIDL](generating-a-type-library-with-midl-2.md)
</dt> </dl>

 

 