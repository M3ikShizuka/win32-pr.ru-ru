---
description: Задает уровень смешения в децибел (dB) в потоке цифрового звука Dolby. Это свойство применяется к кодировщикам цифрового аудио Dolby.
ms.assetid: fcb16d02-af4f-4626-99ee-2831172e5280
title: Свойство Авенкддпродуктионмикслевел (Кодекапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f73f2c9db1a4ddf1b1354ec0354f77b8f87d8a81b3c98dec7a74a45025e67550
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119873214"
---
# <a name="avencddproductionmixlevel-property"></a>Авенкддпродуктионмикслевел, свойство

Задает уровень смешения в децибел (dB) в потоке цифрового звука Dolby. Это свойство применяется к кодировщикам цифрового аудио Dolby.

Это свойство доступно для чтения и записи.

## <a name="data-type"></a>Тип данных

**UINT32** (**VT \_ UI4**)

## <a name="property-guid"></a>GUID свойства

**КОДЕКАПИ \_ авенкддпродуктионмикслевел**

## <a name="property-value"></a>Значение свойства

Это свойство имеет линейный Диапазон значений. Чтобы получить поддерживаемый диапазон, вызовите метод [**икодекапи:: жетпараметерранже**](/windows/desktop/api/Strmif/nf-strmif-icodecapi-getparameterrange).

## <a name="remarks"></a>Remarks

Если это свойство задано, задайте для свойства [**авенкддпродуктионинфоексистс**](avencddproductioninfoexists-property.md) значение **true**.

## <a name="requirements"></a>Requirements (Требования)



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

 

 




