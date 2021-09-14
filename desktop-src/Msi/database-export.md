---
description: Метод Export объекта Database копирует структуру и данные из указанной таблицы в текстовый файл архива.
ms.assetid: b724595f-ef28-456e-bf0b-5df65c659d17
title: Метод Database. Export
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Database.Export
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: e9fbd5be6523db54be5f71b806bf278861f14709
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127141962"
---
# <a name="databaseexport-method"></a>Метод Database. Export

Метод **Export** объекта [**Database**](database-object.md) копирует структуру и данные из указанной таблицы в [текстовый файл архива](text-archive-files.md).

## <a name="syntax"></a>Синтаксис


```JScript
Database.Export(
  table,
  path,
  file
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*table* 
</dt> <dd>

Обязательное имя таблицы базы данных. С учетом регистра, если используется база данных установщика.

</dd> <dt>

*путь* 
</dt> <dd>

Обязательная строка, которая является путем к папке, в которую помещен текстовый файл.

</dd> <dt>

*файл* 
</dt> <dd>

Обязательное имя создаваемого файла. Сюда не входит папка, которая должна быть задана в объекте Path.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

В случае сбоя метода можно получить расширенные сведения об ошибке с помощью метода [**ластерроррекорд**](installer-lasterrorrecord.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ идатабасе определяется как 000C109D-0000-0000-C000-000000000046<br/>                                                                                                                                                                            |



 

 




