---
description: Возвращает статистику для приемника мультимедиа Digital живая Network Alliance (DLNA).
ms.assetid: 1fa6ea9f-fd30-4fa2-a0e6-1647273bcc35
title: Атрибут MF_MP2DLNA_STATISTICS (Mfmp2dlna. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a51620c1ca093a422a5e4657edcfbfaa66ae6cd3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462122"
---
# <a name="mf_mp2dlna_statistics-attribute"></a>\_ \_ Атрибут статистики MF MP2DLNA

Возвращает статистику для приемника мультимедиа Digital живая Network Alliance (DLNA).

## <a name="data-type"></a>Тип данных

**[**MFMPEG2DLNASINKSTATS**](/windows/desktop/api/mfmp2dlna/ns-mfmp2dlna-mfmpeg2dlnasinkstats)** хранится в **виде \[ \] байта**

## <a name="getset"></a>Get/Set

Чтобы получить этот атрибут, вызовите метод [**имфаттрибутес::-BLOB**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getblob).

## <a name="remarks"></a>Remarks

Во время потоковой передачи приемник мультимедиа DLNA обновляет этот атрибут со статистикой о кодировке и мультиплексировании потоков MPEG-2. Приложение может в любое время запросить этот атрибут для получения последних значений.

Установка этого атрибута для приемника мультимедиа DLNA не оказывает никакого воздействия.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Mfmp2dlna. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> </dl>

 

 




