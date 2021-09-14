---
description: Свойство StringData объекта Record — это свойство, доступное для чтения и записи, которое передает строковые данные в указанное поле в записи или из него. Если было сохранено целое число или объект, возвращается его строковое значение.
ms.assetid: ffa163eb-41b3-47ae-b01d-39a3890990a3
title: Свойство Record. StringData
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Record.StringData
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 21f72c35795696875aa55f2d5d791564c6f1fee5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057675"
---
# <a name="recordstringdata-property"></a>Свойство Record. StringData

Свойство **StringData** объекта [**Record**](record-object.md) — это свойство, доступное для чтения и записи, которое передает строковые данные в указанное поле в записи или из него. Если было сохранено целое число или объект, возвращается его строковое значение.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Record.StringData
Record.StringData = propVal 
```



## <a name="property-value"></a>Значение свойства

Обязательный номер поля значения в записи, 1.

## <a name="remarks"></a>Комментарии

Возвращенное значение несуществующего поля является пустой строкой. Чтобы задать для поля записи строки значение null, используйте пустой вариант или пустую строку. Попытка сохранить значение в несуществующем поле приводит к ошибке.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ ирекорд определен как 000C1093-0000-0000-C000-000000000046<br/>                                                                                                                                                                              |



 

 




