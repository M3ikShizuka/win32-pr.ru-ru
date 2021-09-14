---
description: Свойство FileAttributes объекта Installer возвращает число, представляющее комбинированные атрибуты файла для указанного пути к файлу или папке.
ms.assetid: a09ac346-4e4d-440f-bfbe-ff8fb3f69823
title: свойство установщика. FileAttributes (Windows. storage. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Installer.FileAttributes
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: e9a4d2b956c7d325fabcda7d6950274249120a0e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171652"
---
# <a name="installerfileattributes-property"></a>Свойство Installer. FileAttributes

Свойство **FileAttributes** объекта [**Installer**](installer-object.md) возвращает число, представляющее комбинированные атрибуты файла для указанного пути к файлу или папке.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Installer.FileAttributes
```



## <a name="property-value"></a>Значение свойства

Требуемый путь к файлу или папке. Частичный путь предполагает наличие текущего каталога.

## <a name="remarks"></a>Комментарии

Свойство **FileAttributes** возвращает следующие значения.



| Атрибут файла              | Значение      | Значение |
|-----------------------------|------------|-------|
| FILE\_ATTRIBUTE\_READONLY   | 0x00000001 | 1     |
| FILE\_ATTRIBUTE\_HIDDEN     | 0x00000002 | 2     |
| FILE\_ATTRIBUTE\_SYSTEM     | 0x00000004 | 4     |
| FILE\_ATTRIBUTE\_DIRECTORY  | 0x00000010 | 16    |
| \_ \_ временный атрибут файла  | 0x00000100 | 256   |
| FILE\_ATTRIBUTE\_COMPRESSED | 0x00000800 | 2048  |
| FILE\_ATTRIBUTE\_OFFLINE    | 0x00001000 | 4096  |



 

Возвращает значение – 1, если файл или папка не существуют или недоступны.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| Заголовок<br/>  | <dl> <dt>Windows. storage. h</dt> </dl>                                                                                                                                                            |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ иинсталлер определен как 000C1090-0000-0000-C000-000000000046<br/>                                                                                                                                                                           |



 

 




