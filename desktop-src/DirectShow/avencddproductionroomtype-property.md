---
description: Указывает тип комнаты для потока цифрового аудио Dolby. Это свойство применяется к кодировщикам цифрового аудио Dolby.
ms.assetid: d19b6b9d-9606-48a8-ac8e-cdbf15588a8f
title: Свойство Авенкддпродуктионрумтипе (Кодекапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4e740138f90d06da8934fdfe1dc8f4d4f3e1afd37537c6c91e1e5bd774847eb6
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120103414"
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

## <a name="remarks"></a>Remarks

*Тип комнаты* относится к размеру комнаты, используемой в рабочей среде. Если это свойство задано, задайте для свойства [**авенкддпродуктионинфоексистс**](avencddproductioninfoexists-property.md) значение **true**.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional приложения \[ UWP для классических приложений \|\]<br/>                     |
| Минимальная версия сервера<br/> | \[приложения UWP для классических приложений Windows 2000 \|\]<br/>                           |
| Заголовок<br/>                   | <dl> <dt>Кодекапи. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Свойства кодека API](codec-api-properties.md)
</dt> <dt>

[**Интерфейс Икодекапи**](/windows/desktop/api/Strmif/nn-strmif-icodecapi)
</dt> </dl>

 

