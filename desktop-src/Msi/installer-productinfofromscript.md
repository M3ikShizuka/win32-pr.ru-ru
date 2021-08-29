---
description: Свойство Продуктинфофромскрипт объекта Installer возвращает значение указанного атрибута, хранящегося в скрипте объявления.
ms.assetid: 92aa479b-2b4c-482c-a186-a290461bc6d8
title: Установщик::P свойство Родуктинфофромскрипт
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Installer.ProductInfoFromScript
- Installer.put_ProductInfoFromScript
- Installer.ProductInfoFromScript
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 7b0319c83cc981f36bc4d744bb34e96a684adf8d203bdf4f4dc6ab8472033639
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120129374"
---
# <a name="installerproductinfofromscript-property"></a>Установщик::P свойство Родуктинфофромскрипт

Свойство **продуктинфофромскрипт** объекта [**Installer**](installer-object.md) возвращает значение указанного атрибута, хранящегося в скрипте объявления.

Это свойство доступно только на запись.

## <a name="syntax"></a>Синтаксис


```JScript
Installer.ProductInfoFromScript = propVal 
```



## <a name="property-value"></a>Значение свойства

## <a name="error-codes"></a>Коды ошибок

Строковое или целочисленное значение, зависящее от запрошенного атрибута.

## <a name="remarks"></a>Remarks

Свойство **продуктинфофромскрипт** использует функцию [**мсижетпродуктинфофромскрипт**](/windows/desktop/api/Msi/nf-msi-msigetproductinfofromscripta) .

## <a name="examples"></a>Примеры

В следующем примере скрипта демонстрируется использование свойства **продуктинфофромскрипт** .


```VB
Dim installer
Set installer = CreateObject("WindowsInstaller.Installer")

' 
' Create an advertise script for Orca
'

installer.CreateAdvertiseScript "\\products\public\orca\orca.msi", "c:\scratch\orca.aas"

' 
' Output ProductName Information From Script
'

MsgBox  installer.ProductInfoFromScript("c:\scratch\orca.aas", 3)
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик 4,5 на Windows Server 2003 и Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                           |
| IID<br/>     | IID \_ иинсталлер определен как 000C1090-0000-0000-C000-000000000046<br/>                                                                                                                                                                                |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Установщик**](installer-object.md)
</dt> <dt>

[не поддерживается в установщик Windows 3,1 и более ранних версиях](not-supported-in-windows-installer-version-3-1.md)
</dt> </dl>

 

 




