---
description: Возвращает объект Рекордлист, в котором перечислены продукты, использующие указанный установленный компонент.
ms.assetid: c9756526-68d7-4d04-97e2-56a5eaf816be
title: Свойство Installer. Клиентсекс
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Installer.ClientsEx
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 5a609ab0ba6edc5b0e3e9bbd26bc3539858ebdee
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171735"
---
# <a name="installerclientsex-property"></a>Свойство Installer. Клиентсекс

Это свойство возвращает объект [**рекордлист**](recordlist-object.md) , в котором перечислены продукты, использующие указанный установленный компонент. Это свойство вызывает [**мсиенумклиентсекс**](/windows/desktop/api/Msi/nf-msi-msienumclientsexa).

**[установщик Windows 4,5 или более ранней версии](not-supported-in-windows-installer-4-5.md):** Не поддерживается. это свойство доступно, начиная с установщик Windows 5,0.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Installer.ClientsEx
```



## <a name="property-value"></a>Значение свойства

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                      |
| IID<br/>     | IID \_ иинсталлер определен как 000C1090-0000-0000-C000-000000000046<br/>                           |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**мсиенумклиентсекс**](/windows/desktop/api/Msi/nf-msi-msienumclientsexa)
</dt> </dl>

 

 




