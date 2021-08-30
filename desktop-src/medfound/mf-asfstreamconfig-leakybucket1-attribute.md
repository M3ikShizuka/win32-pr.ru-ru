---
description: задает среднее &\# 0034;&\# 0034; параметров (см. примечания) для кодирования Windows файла мультимедиа. Задайте этот атрибут с помощью интерфейса Имфасфстреамконфиг.
ms.assetid: 5aa570eb-1004-4942-9a63-b8f6373d4e53
title: Атрибут MF_ASFSTREAMCONFIG_LEAKYBUCKET1 (Вмконтаинер. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5343d7721d6fad4be4d8623ffdd8f1b3e63fccbe8d90cd4616e0115c35fc2100
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119826824"
---
# <a name="mf_asfstreamconfig_leakybucket1-attribute"></a>\_Атрибут MF асфстреамконфиг \_ LEAKYBUCKET1

задает среднее значение параметров "сегмент утечки" (см. примечания) для кодирования Windowsного файла мультимедиа. Задайте этот атрибут с помощью интерфейса [**имфасфстреамконфиг**](/windows/desktop/api/wmcontainer/nn-wmcontainer-imfasfstreamconfig) .

## <a name="data-type"></a>Тип данных

массив байтов;

## <a name="remarks"></a>Remarks

Значение этого атрибута представляет собой массив из трех **DWORD** в следующем порядке:

-   Скорость в битах в секунду.
-   Окно буфера в миллисекундах.
-   Заполнение начальной буферизации в байтах.

дополнительные сведения о концепции сегмента утечки см. в разделе [модель буферного контейнера с утечкой](the-leaky-bucket-buffer-model.md) данных в документации по Windows Media Format SDK.

Константа GUID для этого атрибута экспортируется из мфууид. lib.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                     |
| Заголовок<br/>                   | <dl> <dt>Вмконтаинер. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Атрибуты ASF](asf-attributes.md)
</dt> <dt>

[**Имфаттрибутес:: BLOB**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getblob)
</dt> <dt>

[**Имфаттрибутес:: SetBlob**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setblob)
</dt> <dt>

[**MF \_ асфстреамконфиг \_ LEAKYBUCKET2**](mf-asfstreamconfig-leakybucket2-attribute.md)
</dt> </dl>

 

 




