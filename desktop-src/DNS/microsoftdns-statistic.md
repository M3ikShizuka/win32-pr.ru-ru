---
title: Класс MicrosoftDNS_Statistic
description: '\_Класс статистики микрософтднс представляет собой отдельную статистику DNS-сервера.'
ms.assetid: 49ee79d6-b93f-4a9b-8054-1ad290d092d6
keywords:
- DNS класса MicrosoftDNS_Statistic
- DNS-MicrosoftDNS_Statistic класса, описание
topic_type:
- apiref
api_name:
- MicrosoftDNS_Statistic
- MicrosoftDNS_Statistic.DnsServerName
- MicrosoftDNS_Statistic.CollectionName
- MicrosoftDNS_Statistic.CollectionId
- MicrosoftDNS_Statistic.Name
- MicrosoftDNS_Statistic.Value
- MicrosoftDNS_Statistic.StringValue
api_location:
- Root\MicrosoftDNS
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4a489f8a4d9e3d442d4157243594c187a799d20a1d07b3ccc68135e73ddce288
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119815664"
---
# <a name="microsoftdns_statistic-class"></a>\_Класс статистики микрософтднс

Класс **\_ статистики микрософтднс** представляет собой ОТДЕЛЬНУЮ статистику DNS-сервера.

Следующий синтаксис упрощен из MOF-кода.

## <a name="syntax"></a>Синтаксис

``` syntax
class MicrosoftDNS_Statistic
{
  string DnsServerName;
  string CollectionName;
  uint32 CollectionId;
  string Name;
  uint32 Value;
  string StringValue;
};
```

## <a name="members"></a>Члены

Класс **\_ статистики микрософтднс** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **\_ статистики микрософтднс** имеет следующие свойства.

<dl> <dt>

**CollectionId**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Числовое представление **CollectionName**.

</dd> <dt>

**CollectionName**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Имя коллекции, которой принадлежит статистика.

</dd> <dt>

**днссервернаме**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Указывает полное доменное имя (FQDN) или IP-адрес DNS-сервера, содержащего статистику.

</dd> <dt>

**Имя**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Имя статистики.

</dd> <dt>

**StringValue**
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Строковое значение статистики, используемое только в том случае, если значение статистики не представлено в виде DWORD.

</dd> <dt>

**Значение**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> </dl>

Числовое значение статистики, представленное в виде типа DWORD.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                              |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                   |
| Пространство имен<br/>                | Корневой \\ микрософтднс<br/>                                                          |
| MOF<br/>                      | <dl> <dt>Днспров. mof</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Микрософтднс \_ статистикколлектион](microsoftdns-statisticcollection.md)
</dt> </dl>

 

 





