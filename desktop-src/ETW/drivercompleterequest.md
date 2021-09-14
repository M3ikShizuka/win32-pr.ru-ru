---
description: Этот класс является классом типа события для событий запроса драйвера Complete. Следующий синтаксис упрощен из MOF-кода.
ms.assetid: c9c9be05-c1c6-4d77-a47a-44a61ebfcdc7
title: Класс Дриверкомплетерекуест
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- DriverCompleteRequest
- DriverCompleteRequest.RoutineAddr
- DriverCompleteRequest.Irp
- DriverCompleteRequest.UniqMatchId
api_type:
- NA
api_location: ''
ms.openlocfilehash: 57cf49d0e37dc870c0eb46c31ef39e0d81689811
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055386"
---
# <a name="drivercompleterequest-class"></a>Класс Дриверкомплетерекуест

Этот класс является классом типа события для событий запроса драйвера Complete.

Следующий синтаксис упрощен из MOF-кода.

## <a name="syntax"></a>Синтаксис

``` syntax
[EventType{52}, EventTypeName{"DrvComplReq"}]
class DriverCompleteRequest : DiskIo
{
  uint32 RoutineAddr;
  uint32 Irp;
  uint32 UniqMatchId;
};
```

## <a name="members"></a>Участники

Класс **дриверкомплетерекуест** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **дриверкомплетерекуест** имеет следующие свойства.

<dl> <dt>

**IRP**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: Вмидатаид (2), Pointer
</dt> </dl>

Пакет запроса ввода-вывода.

</dd> <dt>

**раутинеаддр**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: Вмидатаид (1), Pointer
</dt> </dl>

Адрес вызываемой функции драйвера.

</dd> <dt>

**уникматчид**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: Вмидатаид (3)
</dt> </dl>

Идентификатор, который однозначно идентифицирует запрос. Используйте этот идентификатор для сопоставления с другими событиями драйвера, например с событием [**дриверкомплетерекуестретурн**](drivercompleterequestreturn.md) .

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**дискио**](diskio.md)
</dt> </dl>

 

 




