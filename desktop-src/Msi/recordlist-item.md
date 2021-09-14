---
description: Свойство Item является свойством, предназначенным только для чтения и возвращающим запись в коллекции объектов Рекордлист.
ms.assetid: 59646aa8-811c-4658-8b47-42f70abfdfdb
title: Рекордлист. Item, свойство
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- RecordList.Item
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 4c7b9332393c4055cb8052b2b759b93781c0fd73
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057668"
---
# <a name="recordlistitem-property"></a>Рекордлист. Item, свойство

Свойство **Item** является свойством, предназначенным только для чтения и возвращающим запись в коллекции объектов [**рекордлист**](recordlist-object.md) .

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = RecordList.Item
```



## <a name="property-value"></a>Значение свойства

Номер индекса элемента с коллекцией строк. Требуется индекс.

## <a name="remarks"></a>Комментарии

Клиент должен убедиться, что объект [**рекордлист**](recordlist-object.md) существует и не пуст, прежде чем ссылаться на свойство Item.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ ирекордлист определен как 000C1096-0000-0000-C000-000000000046<br/>                                                                                                                                                                          |



 

 




