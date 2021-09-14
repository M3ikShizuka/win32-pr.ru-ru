---
description: Указывает тип комнаты для потока цифрового аудио Dolby. Это свойство применяется к кодировщикам цифрового аудио Dolby.
ms.assetid: d19b6b9d-9606-48a8-ac8e-cdbf15588a8f
title: Свойство Авенкддпродуктионрумтипе (Кодекапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 2dc2eed0bb491fc982a5102507e5b55bf610880a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127161904"
---
# <a name="avencddproductionroomtype-property"></a>Авенкддпродуктионрумтипе, свойство

Указывает тип комнаты для потока цифрового аудио Dolby. Это свойство применяется к кодировщикам цифрового аудио Dolby.

Это свойство доступно для чтения и записи.

## <a name="data-type"></a>Тип данных

**UINT32** (**VT \_ UI4**)

## <a name="property-guid"></a>GUID свойства

**КОДЕКАПИ \_ авенкддпродуктионрумтипе**

## <a name="property-value"></a>Значение свойства

Значение этого свойства является членом перечисления [**еавенкддпродуктионрумтипе**](/windows/win32/api/codecapi/ne-codecapi-eavencddproductionroomtype) .

## <a name="remarks"></a>Комментарии

*Тип комнаты* относится к размеру комнаты, используемой в рабочей среде. Если это свойство задано, задайте для свойства [**авенкддпродуктионинфоексистс**](avencddproductioninfoexists-property.md) значение **true**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional приложения \[ UWP для классических приложений \|\]<br/>                     |
| Минимальная версия сервера<br/> | \[приложения UWP для классических приложений Windows 2000 \|\]<br/>                           |
| Заголовок<br/>                   | <dl> <dt>Кодекапи. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства кодека API](codec-api-properties.md)
</dt> <dt>

[**Интерфейс Икодекапи**](/windows/desktop/api/Strmif/nn-strmif-icodecapi)
</dt> </dl>

 

