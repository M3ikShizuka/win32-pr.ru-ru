---
description: Свойство Патчфилес возвращает объект Стринглист, содержащий список файлов, которые можно обновить с помощью предоставленного списка исправлений.
ms.assetid: 14549847-8558-4a9a-9ad5-3575c3f4391e
title: Свойство Installer. Патчфилес
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Installer.PatchFiles
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 43491bb384e6f95b31b4e7ae12e5fd32f4fbe8b6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065578"
---
# <a name="installerpatchfiles-property"></a>Свойство Installer. Патчфилес

Свойство **патчфилес** возвращает объект [**стринглист**](stringlist-object.md) , содержащий список файлов, которые можно обновить с помощью предоставленного списка исправлений. Это свойство вызывает [**мсижетпатчфилелист**](/windows/desktop/api/Msi/nf-msi-msigetpatchfilelista). Дополнительные сведения об использовании свойства **патчфилес** см. [в разделе Список файлов, которые можно обновить](listing-the-files-that-can-be-updated.md).

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Installer.PatchFiles
```



## <a name="property-value"></a>Значение свойства

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик 4,5 на Windows Server 2003 и Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                           |
| IID<br/>     | IID \_ иинсталлер определен как 000C1090-0000-0000-C000-000000000046<br/>                                                                                                                                                                                |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект установщика**](installer-object.md)
</dt> <dt>

[не поддерживается в установщик Windows 3,1 и более ранних версиях](not-supported-in-windows-installer-version-3-1.md)
</dt> </dl>

 

 




