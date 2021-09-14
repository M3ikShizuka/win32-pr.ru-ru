---
title: тлссерверусеаллпурпосецерт
description: Раздел реестра Тлссерверусеаллпурпосецерт определяет, используются ли для проверки подлинности EAP-TLS сертификаты всех целей.
ms.assetid: a672cecb-6bba-4ba6-b362-f6d5a220184b
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 7b7cb767a8f6c8f40b377cca84d948b384170486
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127342247"
---
# <a name="tlsserveruseallpurposecert"></a>тлссерверусеаллпурпосецерт

Раздел реестра Тлссерверусеаллпурпосецерт определяет, используются ли для проверки подлинности EAP-TLS сертификаты всех целей.

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\Rasman\PPP\EAP\13
   TlsServerUseAllPurposeCert = value
```

## <a name="remarks"></a>Remarks

Это значение **reg \_ DWORD** .



| Значение        | Описание                                                                                                      |
|--------------|------------------------------------------------------------------------------------------------------------------|
| 1            | Для проверки подлинности PEAP выбираются сертификаты всех целей в хранилище сертификатов клиента или сервера.     |
| Другие значения | Сертификаты всех целей в хранилище сертификатов клиента или сервера не выбраны для проверки подлинности PEAP. |



 

Если это значение реестра отсутствует, для проверки подлинности EAP-TLS выбираются сертификаты всех целей в хранилище сертификатов клиента или сервера.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Параметры реестра EAPHost](eaphost-registry-settings.md)
</dt> </dl>

 

 




