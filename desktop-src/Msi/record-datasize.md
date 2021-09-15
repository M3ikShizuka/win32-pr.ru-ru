---
description: Свойство DataSize объекта Record является свойством, предназначенным только для чтения и возвращающим размер данных для указанного поля.
ms.assetid: 6f89321e-bdb2-4c18-bdf8-01dea38b47c9
title: Свойство Record. DataSize
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Record.DataSize
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 500ee0039f4bfe638f4eca3740669e821c97ca6b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127348882"
---
# <a name="recorddatasize-property"></a>Свойство Record. DataSize

Свойство **DataSize** объекта [**Record**](record-object.md) является свойством, предназначенным только для чтения и возвращающим размер данных для указанного поля. Если данные являются потоком, возвращается длина потока в байтах. Если данные являются строкой, то возвращается длина строки без значения NULL. Если данные являются целым числом, возвращается значение 4 (что означает размер целого числа). Если данные равны NULL, возвращается значение 0.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Record.DataSize
```



## <a name="property-value"></a>Значение свойства

Обязательный номер поля значения в записи, 1.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ ирекорд определен как 000C1093-0000-0000-C000-000000000046<br/>                                                                                                                                                                              |



 

 




