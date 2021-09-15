---
description: Указывает число пропущенных видеокадров, так как они являлись дубликатами предыдущих кадров.
ms.assetid: ef4aa5a0-3788-493e-b541-c3a24509d939
title: Свойство MFPKEY_ZEROBYTEFRAMES (Вмкодекдсп. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ffcf29d099b3a3fb27a307e970af7af1a5c3d58b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460852"
---
# <a name="mfpkey_zerobyteframes-property"></a>МФПКЭЙ \_ зеробитефрамес, свойство

Указывает число пропущенных видеокадров, так как они являлись дубликатами предыдущих кадров.

## <a name="constant-for-ipropertybag"></a>Константа для Ипропертибаг

g \_ всзвмвкзеробитефрамес

## <a name="data-type"></a>Тип данных

VT \_ I4

## <a name="remarks"></a>Remarks

Это значение не вычитается из общего числа переданных кадров ([мфпкэй \_ тоталфрамес](mfpkey-totalframesproperty.md)) при вычислении количества закодированных кадров ([мфпкэй \_ кодедфрамес](mfpkey-codedframesproperty.md)).

Вы можете запретить кодеку пропускать дубликаты кадров, установив для [мфпкэй \_ ПРОДУЦЕДУММИФРАМЕС](mfpkey-producedummyframesproperty.md) значение Variant \_ true.

Это значение можно получить после завершения передачи образцов.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                    |
| Заголовок<br/>                   | <dl> <dt>Вмкодекдсп. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства Media Foundation](media-foundation-properties.md)
</dt> </dl>

 

 




