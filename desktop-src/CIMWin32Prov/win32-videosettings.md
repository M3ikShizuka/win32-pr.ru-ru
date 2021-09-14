---
description: '\_Класс WMI взаимосвязей Win32 видеосеттингс связывает видеоконтроллер и параметры видео, которые можно применить к нему.'
ms.assetid: 0cc42352-0a89-434d-a8b6-230c677de49c
ms.tgt_platform: multiple
title: Класс Win32_VideoSettings
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Win32_VideoSettings
- Win32_VideoSettings.Setting
- Win32_VideoSettings.Element
api_type:
- DllExport
api_location:
- CIMWin32.dll
ms.openlocfilehash: 38e949b6b6501dc51b39448d72e6bf61f37fbecb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127251260"
---
# <a name="win32_videosettings-class"></a>\_Класс Win32 видеосеттингс

[Класс WMI](../wmisdk/retrieving-a-class.md) взаимосвязей **Win32 \_ видеосеттингс** связывает видеоконтроллер и параметры видео, которые можно применить к нему.

Следующий пример синтаксиса — упрощенный MOF-код, который включает все наследуемые свойства. Свойства перечислены в алфавитном порядке, а не в MOF.

## <a name="syntax"></a>Синтаксис

``` syntax
[Dynamic, Provider("CIMWin32"), UUID("{1008CCEE-7BFF-11D2-AAD2-006008C78BC7}"), AMENDMENT]
class Win32_VideoSettings : CIM_VideoSetting
{
  CIM_VideoControllerResolution REF Setting;
  Win32_VideoController         REF Element;
};
```

## <a name="members"></a>Участники

Класс **Win32 \_ видеосеттингс** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **Win32 \_ видеосеттингс** имеет следующие свойства.

<dl> <dt>

**Элемент**
</dt> <dd> <dl> <dt>

Тип данных: **Win32 \_ Видеоконтроллер**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**ключ**](../wmisdk/key-qualifier.md), [**Переопределение**](../wmisdk/standard-qualifiers.md) ("элемент"), [**маппингстрингс**](../wmisdk/standard-qualifiers.md) ("WMI \| Win32 \_ Видеоконтроллер")
</dt> </dl>

[**\_ Видеоконтроллер Win32**](win32-videocontroller.md) , содержащий свойства видеоконтроллера, на котором можно использовать параметр видео.

</dd> <dt>

**Параметр**
</dt> <dd> <dl> <dt>

Тип данных: **CIM \_ видеоконтроллерресолутион**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [**ключ**](../wmisdk/key-qualifier.md), [**Переопределение**](../wmisdk/standard-qualifiers.md) ("параметр"), [**маппингстрингс**](../wmisdk/standard-qualifiers.md) ("CIM \| CIM \_ видеоконтроллерресолутион")
</dt> </dl>

[**\_ Видеоконтроллерресолутион CIM**](cim-videocontrollerresolution.md) , содержащий параметры, которые можно применить к видеоконтроллеру.

</dd> </dl>

## <a name="remarks"></a>Remarks

Класс **Win32 \_ видеосеттингс** является производным от [**CIM \_ видеосеттинг**](cim-videosetting.md).

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

[**\_ВИДЕОСЕТТИНГ CIM**](cim-videosetting.md)
</dt> <dt>

[Аппаратные классы системы компьютера](computer-system-hardware-classes.md)
</dt> </dl>

 

 
