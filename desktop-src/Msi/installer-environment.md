---
description: Свойство Environment объекта Installer — это свойство для чтения и записи, которое является строковым значением для переменной среды текущего процесса.
ms.assetid: f59a270f-9bd8-4d17-96e2-cb3c62a31cad
title: Свойство установщика. Environment
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Installer.Environment
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 3983eceecd8bc709bea4a094c61c9886c73def3a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171671"
---
# <a name="installerenvironment-property"></a>Свойство установщика. Environment

Свойство **Environment** объекта [**Installer**](installer-object.md) — это свойство для чтения и записи, которое является строковым значением для переменной среды текущего процесса.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Installer.Environment
Installer.Environment = propVal 
```



## <a name="property-value"></a>Значение свойства

Имя переменной среды, которая должна быть прочитана или записана. Это не учитывает регистр.

## <a name="remarks"></a>Комментарии

Установка переменной среды со свойством **Environment** влияет только на активный сеанс. Чтобы внести постоянные изменения в переменную среды, используйте [таблицу среда](environment-table.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ иинсталлер определен как 000C1090-0000-0000-C000-000000000046<br/>                                                                                                                                                                           |



 

 




