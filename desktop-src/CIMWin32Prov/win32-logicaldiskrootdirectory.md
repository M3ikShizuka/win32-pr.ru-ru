---
description: '\_Класс WMI взаимосвязей Win32 логикалдискрутдиректори связывает логический диск и структуру каталогов.'
ms.assetid: 860cd28a-2a59-4ce3-be26-8fdc869c70d1
ms.tgt_platform: multiple
title: Класс Win32_LogicalDiskRootDirectory
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Win32_LogicalDiskRootDirectory
- Win32_LogicalDiskRootDirectory.GroupComponent
- Win32_LogicalDiskRootDirectory.PartComponent
api_type:
- DllExport
api_location:
- CIMWin32.dll
ms.openlocfilehash: e4b015891a37c5cc92bbf102482f48306d537bb6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127273448"
---
# <a name="win32_logicaldiskrootdirectory-class"></a>\_Класс Win32 логикалдискрутдиректори

[Класс WMI](/windows/desktop/WmiSdk/retrieving-a-class) взаимосвязей **Win32 \_ логикалдискрутдиректори** связывает логический диск и структуру каталогов.

Следующий пример синтаксиса — упрощенный MOF-код, который включает все наследуемые свойства. Свойства и методы имеют алфавитный порядок, а не порядок MOF.

## <a name="syntax"></a>Синтаксис

``` syntax
[Dynamic, Provider("CIMWin32"), UUID("{F25FE468-783E-11d2-90BF-0060081A46FD}"), AMENDMENT]
class Win32_LogicalDiskRootDirectory : CIM_Component
{
  Win32_LogicalDisk REF GroupComponent;
  Win32_Directory   REF PartComponent;
};
```

## <a name="members"></a>Участники

Класс **Win32 \_ логикалдискрутдиректори** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **Win32 \_ логикалдискрутдиректори** имеет следующие свойства.

<dl> <dt>

**Ссылка**
</dt> <dd> <dl> <dt>

Тип данных: **Win32 \_ LogicalDisk**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**ключ**](/windows/desktop/WmiSdk/key-qualifier), [**Переопределение**](/windows/desktop/WmiSdk/standard-qualifiers) ("GroupComponent"), [**маппингстрингс**](/windows/desktop/WmiSdk/standard-qualifiers) ("WMI \| Win32 \_ LogicalDisk")
</dt> </dl>

Ссылка на экземпляр, представляющий свойства логического диска.

</dd> <dt>

**PartComponent**
</dt> <dd> <dl> <dt>

Тип данных: **\_ Каталог Win32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**ключ**](/windows/desktop/WmiSdk/key-qualifier), [**Переопределение**](/windows/desktop/WmiSdk/standard-qualifiers) ("PartComponent"), [**маппингстрингс**](/windows/desktop/WmiSdk/standard-qualifiers) ("WMI- \| \_ Каталог Win32")
</dt> </dl>

Ссылка на экземпляр, представляющий свойства структуры каталогов файлов.

</dd> </dl>

## <a name="remarks"></a>Комментарии

Класс **Win32 \_ логикалдискрутдиректори** является производным от [**\_ компонента CIM**](cim-component.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                          |
| Пространство имен<br/>                | Корневой \\ CIMV2<br/>                                                                  |
| MOF<br/>                      | <dl> <dt>CIMWin32. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>CIMWin32.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Компонент CIM**](cim-component.md)
</dt> <dt>

[Классы операционной системы](/previous-versions//aa392727(v=vs.85))
</dt> </dl>

 

