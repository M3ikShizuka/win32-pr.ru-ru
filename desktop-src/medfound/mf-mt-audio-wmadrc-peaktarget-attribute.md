---
description: целевой пиковый уровень громкости Windowsного звукового файла мультимедиа.
ms.assetid: 73f4e763-dcb7-48cd-ab80-37635d973da0
title: Атрибут MF_MT_AUDIO_WMADRC_PEAKTARGET (Мфапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 806f81c0095481ab5e0694614a54e8374d8bd73445b825493253898ff6f6f0f6
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119955854"
---
# <a name="mf_mt_audio_wmadrc_peaktarget-attribute"></a>\_Атрибут MF \_ Audio \_ вмадрк \_ пеактаржет

целевой пиковый уровень громкости Windowsного звукового файла мультимедиа.

## <a name="data-type"></a>Тип данных

**UINT32**

## <a name="remarks"></a>Remarks

этот атрибут применяется к типам аудио media для кодеков Windows media audio. Он указывает целевой пиковый уровень содержимого. Декодер может использовать это значение для выполнения динамического управления диапазоном.

Метод [**имфасфконтентинфо::P арсехеадер**](/windows/desktop/api/wmcontainer/nf-wmcontainer-imfasfcontentinfo-parseheader) добавляет этот атрибут к типу мультимедиа, если заголовок ASF содержит атрибут [**WM/вмадркпеактаржет**](../wmformat/wm-wmadrcpeaktarget.md) . этот атрибут описан в документации по пакету SDK для Windows Media Format.

Константа GUID для этого атрибута экспортируется из мфууид. lib.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Приложения UWP для классических приложений Vista \|\]<br/>                              |
| Минимальная версия сервера<br/> | Windows \[Приложения UWP для классических приложений сервера 2008 \|\]<br/>                        |
| Заголовок<br/>                   | <dl> <dt>Мфапи. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[**Имфаттрибутес:: UINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint32)
</dt> <dt>

[**Имфаттрибутес:: SetUINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint32)
</dt> <dt>

[**имфмедиатипе**](/windows/desktop/api/mfobjects/nn-mfobjects-imfmediatype)
</dt> <dt>

[Атрибуты типа мультимедиа](media-type-attributes.md)
</dt> </dl>

 

 
