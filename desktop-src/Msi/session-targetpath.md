---
description: Свойство TargetPath объекта Session — это свойство, доступное для чтения и записи, которое предоставляет полный путь к указанной папке на целевом диске установки.
ms.assetid: 563b874e-c669-4f5b-b3fa-eeb6b6e578f2
title: Свойство Session. TargetPath
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Session.TargetPath
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: bd265602e9a4d517ad01a07e79ace43722fcb6cfe0062091a5f0379a5ab264a7
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119628754"
---
# <a name="sessiontargetpath-property"></a>Свойство Session. TargetPath

Свойство **TargetPath** объекта [**Session**](session-object.md) — это свойство, доступное для чтения и записи, которое предоставляет полный путь к указанной папке на целевом диске установки.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Session.TargetPath
Session.TargetPath = propVal 
```



## <a name="property-value"></a>Значение свойства

Обязательное с учетом регистра имя свойства папки, заданное первичным ключом [таблицы Directory](directory-table.md). Если папка не существует, возникает ошибка.

## <a name="remarks"></a>Remarks

Не пытайтесь настроить целевой путь, если компоненты, использующие эти пути, уже установлены для текущего пользователя или для другого пользователя. Проверьте свойство [**продуктстате**](productstate.md) , чтобы определить, установлен ли продукт, содержащий компонент.

Если свойство завершается неудачно, можно получить расширенные сведения об ошибке с помощью метода [**ластерроррекорд**](installer-lasterrorrecord.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ ISession определяется как 000C109E-0000-0000-C000-000000000046<br/>                                                                                                                                                                             |



 

 




