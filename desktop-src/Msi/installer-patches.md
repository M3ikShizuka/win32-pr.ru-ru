---
description: Свойство "исправления только для чтения" объекта установщика возвращает объект Стринглист, содержащий все исправления, примененные к продукту.
ms.assetid: a8d46073-399b-480e-b4b0-a7a2f832e160
title: Свойство Installer. Патчs
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Installer.Patches
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: fd94c5853b3e455cf4d814dfb3c4078705ac727b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065593"
---
# <a name="installerpatches-property"></a>Свойство Installer. Патчs

Свойство " **исправления** только для чтения" объекта [**установщика**](installer-object.md) возвращает объект [**стринглист**](stringlist-object.md) , содержащий все исправления, примененные к продукту.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Installer.Patches
```



## <a name="property-value"></a>Значение свойства

Указывает код продукта.

## <a name="remarks"></a>Remarks

Чтобы перечислить исправления, приложение выполняет итерацию объекта [**стринглист**](stringlist-object.md) , используя для каждой конструкции. Поскольку исправления не упорядочены, каждое новое исправление имеет произвольный индекс. Это означает, что функция может возвращать исправления в любом порядке.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ иинсталлер определен как 000C1090-0000-0000-C000-000000000046<br/>                                                                                                                                                                           |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**мсиенумпатчес**](/windows/desktop/api/Msi/nf-msi-msisourcelistaddmediadiska)
</dt> </dl>

 

 




