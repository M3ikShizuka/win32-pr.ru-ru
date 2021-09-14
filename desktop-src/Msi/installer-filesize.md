---
description: Метод размер файла объекта Installer использует вызовы API Win32 для получения размера файла, указанного в параметре Path.
ms.assetid: d7119e5e-9315-4b20-a904-bc1104f3a4e4
title: Метод Installer. Размер файла
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Installer.FileSize
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 593319b88e3942ae6caa1399adbe2e596bf6e737
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065614"
---
# <a name="installerfilesize-method"></a>Метод Installer. Размер файла

Метод **Размер файла** объекта [**Installer**](installer-object.md) использует вызовы API Win32 для получения размера файла, указанного в параметре *path*.

## <a name="syntax"></a>Синтаксис


```JScript
Installer.FileSize(
  Path
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Путь* 
</dt> <dd>

Обязательная строка, содержащая путь к файлу.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ иинсталлер определен как 000C1090-0000-0000-C000-000000000046<br/>                                                                                                                                                                           |



 

 




