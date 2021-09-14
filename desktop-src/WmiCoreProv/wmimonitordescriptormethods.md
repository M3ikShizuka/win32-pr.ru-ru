---
description: Содержит методы, получающие необработанное содержимое определения входных данных видео с расширенными расширенными данными идентификации (E-EDID) v. 1. x стандартных блоков данных 128-Byte.
ms.assetid: c13d4ddd-d171-44d5-9e70-3a6f89ad55da
title: Класс Вмимонитордескриптормесодс
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- WmiMonitorDescriptorMethods
- WmiMonitorDescriptorMethods.Active
- WmiMonitorDescriptorMethods.InstanceName
api_type:
- DllExport
api_location:
- WmiProv.dll
ms.openlocfilehash: 578c08c48ada4859b69e00655c5eea8c075515fa
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066539"
---
# <a name="wmimonitordescriptormethods-class"></a>Класс Вмимонитордескриптормесодс

Класс WMI **вмимонитордескриптормесодс** содержит методы, которые получают необработанное содержимое распознавания видео с расширенными расширенными данными идентификации (E-EDID) v. 1. x стандартных блоков данных 128-Byte.

## <a name="syntax"></a>Синтаксис

``` syntax
class WmiMonitorDescriptorMethods : MSMonitorClass
{
  boolean Active;
  string  InstanceName;
};
```

## <a name="members"></a>Участники

Класс **вмимонитордескриптормесодс** имеет следующие типы членов:

-   [Методы](#wmimonitordescriptormethods-class)
-   [Свойства](#properties)

### <a name="methods"></a>Методы

Класс **вмимонитордескриптормесодс** содержит следующие методы.



| Метод                                                                                           | Описание                                                                   |
|:-------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------|
| [**WmiGetMonitorRawEEdidV1Block**](wmigetmonitorraweedidv1block-wmimonitordescriptormethods.md) | Обращается к необработанным данным для указанного блока дескрипторов EDID v. 1. x.<br/> |



 

### <a name="properties"></a>Элемент Property

Класс **вмимонитордескриптормесодс** имеет следующие свойства.

<dl> <dt>

**Активен**
</dt> <dd> <dl> <dt>

Тип данных: **логический**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Указывает активный монитор.

</dd> <dt>

**InstanceName**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: **ключ**
</dt> </dl>

Имя конкретного экземпляра монитора.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                               |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                         |
| Пространство имен<br/>                | Корневой \\ инструментарий WMI<br/>                                                                   |
| MOF<br/>                      | <dl> <dt>Вмикоре. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>WmiProv.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**мсмониторкласс**](msmonitorclass.md)
</dt> </dl>

 

 




