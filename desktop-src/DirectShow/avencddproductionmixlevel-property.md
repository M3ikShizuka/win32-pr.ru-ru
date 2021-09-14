---
description: Задает уровень смешения в децибел (dB) в потоке цифрового звука Dolby. Это свойство применяется к кодировщикам цифрового аудио Dolby.
ms.assetid: fcb16d02-af4f-4626-99ee-2831172e5280
title: Свойство Авенкддпродуктионмикслевел (Кодекапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f8a1726db6ab4841b4603a61bcfe39504742db42
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127161907"
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

## <a name="remarks"></a>Комментарии

Если это свойство задано, задайте для свойства [**авенкддпродуктионинфоексистс**](avencddproductioninfoexists-property.md) значение **true**.

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

 

 




