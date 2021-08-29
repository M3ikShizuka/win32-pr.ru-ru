---
title: optional - атрибут
description: Атрибут \ Optional \ указывает необязательный параметр для функции-члена.
ms.assetid: 683e5c9e-5b25-4beb-99ce-cfae4fee4ea6
keywords:
- Необязательный атрибут MIDL
topic_type:
- apiref
api_name:
- optional
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 179d152aaa16420139036a5dc9705ad7cc7c8f240f5f93e51b0cee9a95dc911f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "117806682"
---
# <a name="optional-attribute"></a>optional - атрибут

**\[ Необязательный \]** атрибут указывает необязательный параметр для функции-члена.

``` syntax
return-type function-name([optional [, other-attributes]] parameter-type parameter-name)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*Тип возвращаемого значения* 
</dt> <dd>

Указывает тип возвращаемого значения функции.

</dd> <dt>

*имя функции* 
</dt> <dd>

Указывает имя функции, определенное в IDL-файле.

</dd> <dt>

*другие атрибуты* 
</dt> <dd>

Ноль или несколько необязательных атрибутов MIDL.

</dd> <dt>

*тип параметра* 
</dt> <dd>

Тип данных необязательного параметра.

</dd> <dt>

*имя параметра* 
</dt> <dd>

Указывает имя необязательного параметра.

</dd> </dl>

## <a name="remarks"></a>Remarks

**\[ Необязательный \]** атрибут допустим только в том случае, если параметр относится к типу **Variant** или **Variant** в \* .

Компилятор MIDL принимает следующий порядок параметров (слева направо):

1.  Обязательные параметры (параметры, у которых нет **\[** [**DefaultValue**](defaultvalue.md) **\]** или **\[ необязательных \]** атрибутов);
2.  Необязательные параметры с **\[** [](defaultvalue.md) атрибутом DefaultValue или без него **\]**
3.  Параметры с **\[ необязательным \]** атрибутом и без **\[** [](defaultvalue.md) **\]** атрибута DefaultValue,
4.  **\[** параметр [**LCID**](lcid.md) **\]** , если он есть,
5.  **\[**[**retval**](retval.md) **\]** параметр

**\[ Необязательный \]** атрибут нельзя применить к параметру, который также имеет **\[** [](lcid.md) **\]** атрибуты LCID или **\[** [**retval**](retval.md) **\]** .

## <a name="examples"></a>Примеры

``` syntax
HRESULT MyFunc([in, optional] VARIANT Param1, 
               [out, optional] VARIANT Param2)
```

## <a name="see-also"></a>См. также

<dl> <dt>

[**максимально**](defaultvalue.md)
</dt> <dt>

[Создание библиотеки типов с помощью MIDL](generating-a-type-library-with-midl-2.md)
</dt> <dt>

[**намного**](lcid.md)
</dt> <dt>

[Пример файла ODL](/previous-versions/windows/desktop/automat/odl-file-example)
</dt> <dt>

[Синтаксис файла ODL](/previous-versions/windows/desktop/automat/odl-file-syntax)
</dt> <dt>

[**retval**](retval.md)
</dt> </dl>

 

 