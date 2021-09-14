---
title: Duration (Идлесеттингстипе), элемент
description: Указывает, как долго компьютер должен находиться в состоянии простоя перед выполнением задачи.
ms.assetid: 89584694-0685-44e2-b8b7-69e47ee28d5d
keywords:
- Элемент Duration планировщик задач
topic_type:
- apiref
api_name:
- Duration
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 31ad092693c72dcc33357f4b7e21436e2cba8af8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126891504"
---
# <a name="duration-idlesettingstype-element"></a>Duration (Идлесеттингстипе), элемент

Указывает, как долго компьютер должен находиться в состоянии простоя перед выполнением задачи. Формат этой строки — Пнинмндтнхнмнс, где Нью-то число лет, nM — это количество месяцев, а — число дней, равное, т. е. в качестве разделителя даты и времени, nH — это количество часов, а в качестве значения nS — количество секунд (например, PT5M указывает 5 минут, а P1M4DT2H5M — один месяц, четыре дня, два часа и пять минут). Минимальное значение — одна минута. Дополнительные сведения о типе длительности см. в разделе <https://go.microsoft.com/fwlink/p/?linkid=106886> .

``` syntax
<xs:element name="Duration"
    default="PT10M"
    minOccurs="0"
>
    <xs:simpleType>
        <xs:restriction
            base="duration"
        >
            <xs:minInclusive
                value="PT1M"
             />
        </xs:restriction>
    </xs:simpleType>
</xs:element>
```

Элемент определяется сложным типом [**идлесеттингстипе**](taskschedulerschema-idlesettingstype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                       | Унаследован от                                                                 | Описание                                                                                       |
|-------------------------------------------------------------------------------|------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|
| [**идлесеттингс**](taskschedulerschema-idlesettings-settingstype-element.md) | [**идлесеттингстипе**](taskschedulerschema-idlesettingstype-complextype.md) | Указывает, как планировщик задач выполняет задачи, когда компьютер находится в состоянии простоя.<br/> |



## <a name="remarks"></a>Комментарии

Для программирования скриптов этот параметр простоя указывается с помощью свойства [**идлесеттингс. идледуратион**](idlesettings-idleduration.md) .

При программировании на C++ этот параметр простоя указывается с помощью свойства [**иидлесеттингс:: идледуратион**](/windows/desktop/api/taskschd/nf-taskschd-iidlesettings-get_idleduration) .

## <a name="examples"></a>Примеры

Следующий XML-код определяет параметр бездействия, который разрешает запуск задачи в течение 5 минут.


```XML
<IdleSettings>
    <Duration>PT5M</Duration>
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
</dt> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

 





