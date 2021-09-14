---
title: nonbrowsable - атрибут
description: Используйте атрибут \ неотображаемый \, чтобы пометить интерфейс или член disp-интерфейса, который не должен отображаться в браузере свойств.
ms.assetid: 94e868cc-8d9c-4b8a-ac18-1ea513a103da
keywords:
- неотображаемый атрибут MIDL
topic_type:
- apiref
api_name:
- nonbrowsable
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9e24c39511df9637c352245b98b237fe8fd451eb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127143569"
---
# <a name="nonbrowsable-attribute"></a>nonbrowsable - атрибут

Используйте **\[ неотображаемый \]** атрибут, чтобы пометить интерфейс или член disp-интерфейса, который не должен отображаться в браузере свойств.

``` syntax
[property-attribute-list, nonbrowsable]return-type property-name(prop-param-list)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*Property — список атрибутов* 
</dt> <dd>

Другие атрибуты, которые применяются к свойству.

</dd> <dt>

*Тип возвращаемого значения* 
</dt> <dd>

Тип данных, возвращаемых методом.

</dd> <dt>

*property-name* 
</dt> <dd>

Имя свойства или метода.

</dd> <dt>

*Prop-param-List* 
</dt> <dd>

Ноль или более параметров, которые должны быть переданы в метод.

</dd> </dl>

## <a name="remarks"></a>Remarks

Некоторые свойства не должны отображаться в обозревателе свойств. Это может быть вызвано тем, что получение значения займет очень много времени. В этом примере пользователь не пытается получить свойство *Count* , которое возвращает число строк в динамическом наборе. Это число может представлять результаты очень большого запроса.

Другие свойства могут иметь непредвиденные эффекты в браузере. Например, рассмотрим элемент управления со свойством «OnSelected», чтобы определить, выбран ли элемент управления. Если параметру "IsFalse" присвоено значение false, обозреватель свойств, основанный на выборе, будет просматривать другой объект.

Обратите внимание, что свойство, помеченное **\[ \] как недоступное для просмотра** , по-прежнему будет отображаться в обозревателе объектов, в котором не отображаются значения свойств.

### <a name="typeflag-representation"></a>Представление типефлаг

Присутствие ФУНКФЛАГ \_ фнонбровсабле или варфлаг \_ фнонбровсабле.

## <a name="examples"></a>Примеры

``` syntax
[
    dual,
    uuid(12345678-1234-1234-1234-123456789ABC),
    restricted
]
interface IDynaset:IDispatch
{
    [propget, nonbrowsable]HRESULT Count([out, retval] long *Value);
}
```

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Синтаксис файла ODL](/previous-versions/windows/desktop/automat/odl-file-syntax)
</dt> <dt>

[Пример файла ODL](/previous-versions/windows/desktop/automat/odl-file-example)
</dt> <dt>

[Создание библиотеки типов с помощью MIDL](generating-a-type-library-with-midl-2.md)
</dt> </dl>

 

 