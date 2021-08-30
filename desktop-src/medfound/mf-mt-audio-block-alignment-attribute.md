---
description: Выравнивание блокировки (в байтах) для типа звукового носителя. Выравнивание блока — это минимальная атомарная единица данных для звукового формата.
ms.assetid: 7d304826-ad81-4243-a675-2f55b668b348
title: Атрибут MF_MT_AUDIO_BLOCK_ALIGNMENT (Мфапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d5985485313bda76221a9a45dc4a6aa9f257884766398dce8a9301401d49ea2f
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120113894"
---
# <a name="mf_mt_audio_block_alignment-attribute"></a>\_ \_ \_ Атрибут выравнивания звукового блока MF MT \_

Выравнивание блокировки (в байтах) для типа звукового носителя. Выравнивание блока — это минимальная атомарная единица данных для звукового формата.

## <a name="data-type"></a>Тип данных

**UINT32**

## <a name="remarks"></a>Remarks

Для звуковых форматов PCM выравнивание блока равно числу звуковых каналов, умноженному на число байтов на каждый образец звука.

Этот атрибут соответствует элементу **нблоккалигн** структуры [**вавеформатекс**](/previous-versions/dd757713(v=vs.85)) .

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

 

 
