---
description: Свойство SourcePath объекта Session является свойством, предназначенным только для чтения и предоставляющим полный путь к указанной папке на исходном носителе или образе сервера.
ms.assetid: ed8eea4f-e15e-4d56-ac0c-e18f9cb46d07
title: Свойство Session. SourcePath
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Session.SourcePath
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: d250c786046c778c5a37c07c0378ea856bafb880fc21478699d79b10b4cfcb45
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119628804"
---
# <a name="sessionsourcepath-property"></a>Свойство Session. SourcePath

Свойство **SourcePath** объекта [**Session**](session-object.md) является свойством, предназначенным только для чтения и предоставляющим полный путь к указанной папке на исходном носителе или образе сервера.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Session.SourcePath
```



## <a name="property-value"></a>Значение свойства

Обязательное с учетом регистра имя свойства папки, заданное первичным ключом [таблицы Directory](directory-table.md). Если папка не существует, возникает ошибка.

## <a name="remarks"></a>Remarks

Если свойство завершается неудачно, можно получить расширенные сведения об ошибке с помощью метода [**ластерроррекорд**](installer-lasterrorrecord.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ ISession определяется как 000C109E-0000-0000-C000-000000000046<br/>                                                                                                                                                                             |



 

 




