---
description: Свойство Медиадискс перечисляет все диски носителя для данного экземпляра продукта. Это свойство вызывает Мсисаурцелистенуммедиадискс. Возвращает сведения о диске в виде массива объектов записи.
ms.assetid: 02faf211-16c8-4d2f-b192-c2ce8f3f2c66
title: Свойство patch. Медиадискс
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Patch.MediaDisks
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 462d5b267670804bf2974cf59c848c2684f9e25a07b60488d3a9c0566d89e862
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119558744"
---
# <a name="patchmediadisks-property"></a>Свойство patch. Медиадискс

Свойство **медиадискс** перечисляет все диски носителя для данного экземпляра продукта. Это свойство вызывает [**мсисаурцелистенуммедиадискс**](/windows/desktop/api/Msi/nf-msi-msisourcelistenummediadisksa). Возвращает сведения о диске в виде массива объектов [**записи**](record-object.md) .

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Patch.MediaDisks
```



## <a name="property-value"></a>Значение свойства

## <a name="remarks"></a>Remarks

В каждой записи первое поле содержит идентификатор диска, второе поле содержит метку тома, а третье поле содержит запрос диска, зарегистрированный для диска.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик 3,0 или более поздней версии на Windows Server 2003, Windows XP и Windows 2000<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                                                   |
| IID<br/>     | IID \_ ипатч определен как 000C10A1-0000-0000-C000-000000000046<br/>                                                                                                                                                                                                            |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Обновление**](patch-object.md)
</dt> <dt>

[**мсисаурцелистенуммедиадискс**](/windows/desktop/api/Msi/nf-msi-msisourcelistenummediadisksa)
</dt> <dt>

[**Record**](record-object.md)
</dt> <dt>

[не поддерживается в установщик Windows 2,0 и более ранних версиях](not-supported-in-windows-installer-version-2-0.md)
</dt> </dl>

 

 




