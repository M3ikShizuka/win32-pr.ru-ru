---
description: Возвращает объект Рекордлист, в котором перечислены установленные компоненты.
ms.assetid: a91656de-2ebc-45b5-86f8-b13f35c6a762
title: Свойство Installer. Компонентсекс
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Installer.ComponentsEx
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 1a48261a924280999d2b8329d635d4115de35753
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171703"
---
# <a name="installercomponentsex-property"></a>Свойство Installer. Компонентсекс

Это свойство возвращает объект [**рекордлист**](recordlist-object.md) , в котором перечислены установленные компоненты. Это свойство вызывает [**мсиенумкомпонентсекс**](/windows/desktop/api/Msi/nf-msi-msienumcomponentsexa).

**[установщик Windows 4,5 или более ранней версии](not-supported-in-windows-installer-4-5.md):** Не поддерживается. это свойство доступно, начиная с установщик Windows 5,0.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Installer.ComponentsEx
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

[**мсиенумкомпонентсекс**](/windows/desktop/api/Msi/nf-msi-msienumcomponentsexa)
</dt> </dl>

 

 




