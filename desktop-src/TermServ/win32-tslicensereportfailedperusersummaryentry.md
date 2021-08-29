---
title: Класс Win32_TSLicenseReportFailedPerUserSummaryEntry
description: Содержит сведения о доменах, для которых не удалось выдачу на пользователя.
ms.assetid: f7265734-ac4d-439f-ae8b-3694e6f81f2a
ms.tgt_platform: multiple
keywords:
- Класс Win32_TSLicenseReportFailedPerUserSummaryEntry службы удаленных рабочих столов
- Службы удаленных рабочих столов класса Win32_TSLicenseReportFailedPerUserSummaryEntry, описание
topic_type:
- apiref
api_name:
- Win32_TSLicenseReportFailedPerUserSummaryEntry
- Win32_TSLicenseReportFailedPerUserSummaryEntry.DomainName
- Win32_TSLicenseReportFailedPerUserSummaryEntry.FailedIssuanceCount
api_location:
- TlsWmiProv.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f3eefa2e4547bb42f2888fd1cc466e9a9abbb97f0b381f6fc439244bdb59a065
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120008434"
---
# <a name="win32_tslicensereportfailedperusersummaryentry-class"></a>\_Класс Win32 тслиценсерепортфаиледперусерсуммарентри

Содержит сведения о доменах, для которых не удалось выдачу на пользователя.

Следующий пример синтаксиса — упрощенный MOF-код, который включает все наследуемые свойства.

## <a name="syntax"></a>Синтаксис

``` syntax
[AMENDMENT]
class Win32_TSLicenseReportFailedPerUserSummaryEntry
{
  string DomainName;
  uint32 FailedIssuanceCount;
};
```

## <a name="members"></a>Члены

Класс **Win32 \_ тслиценсерепортфаиледперусерсуммарентри** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **Win32 \_ тслиценсерепортфаиледперусерсуммарентри** имеет следующие свойства.

<dl> <dt>

**DomainName**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: [ **ключ**](/windows/desktop/WmiSdk/key-qualifier)
</dt> </dl>

Указывает имя домена, в котором произошел сбой при выдаче лицензии.

</dd> <dt>

**фаиледиссуанцекаунт**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Количество неудачных выдачи.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                                 |
| Минимальная версия сервера<br/> | Windows Server 2012<br/>                                                            |
| Пространство имен<br/>                | Root\\CIMv2<br/>                                                                    |
| MOF<br/>                      | <dl> <dt>Тлсвмипров. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>TlsWmiProv.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**фетчрепортфаиледперусерсуммарентриес**](fetchreportfailedperusersummaryentries-win32-tslicensereport.md)
</dt> </dl>

 

