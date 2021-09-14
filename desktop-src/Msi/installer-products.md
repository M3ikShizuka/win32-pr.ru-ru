---
description: Свойство Products является свойством только для чтения, которое возвращает набор всех продуктов, установленных или объявленных для текущего пользователя и компьютера.
ms.assetid: 5c210827-a7cc-4358-bfe6-4d8e9767bd8c
title: Свойство Installer. Products
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Installer.Products
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 8d5b20a770154382e7e7a68cc3fe4d81c350fb1f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065575"
---
# <a name="installerproducts-property"></a>Свойство Installer. Products

Свойство **Products** является свойством только для чтения, которое возвращает [](stringlist-object.md) набор всех продуктов, установленных или объявленных для текущего пользователя и компьютера.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Installer.Products
```



## <a name="property-value"></a>Значение свойства

## <a name="remarks"></a>Remarks

Чтобы перечислить продукты, приложение выполняет итерацию по объекту [**стринглист**](stringlist-object.md) , используя для каждой конструкции. Поскольку продукты не упорядочены, у каждого нового продукта есть произвольный индекс. Это означает, что функция может возвращать продукты в любом порядке.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик на Windows Server 2003 или Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID \_ иинсталлер определен как 000C1090-0000-0000-C000-000000000046<br/>                                                                                                                                                                           |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**мсиенумпродуктс**](/windows/desktop/api/Msi/nf-msi-msienumproductsa)
</dt> </dl>

 

 




