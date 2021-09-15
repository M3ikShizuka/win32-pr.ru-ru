---
description: Указывает максимальное количество дополнительных выборок PCM, которые могут быть возвращены в конце после декодирования файла.
ms.assetid: 82b3676c-7653-421c-aac7-7f20a642779f
title: Свойство MFPKEY_Decoder_MaxNumPCMSamplesWithPaddedSilence (Вмкодекдсп. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4b1f97b55c2eedd8cc7d6d524379569073fa35d9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572750"
---
# <a name="mfpkey_decoder_maxnumpcmsampleswithpaddedsilence-property"></a>\_Свойство макснумпкмсамплесвиспаддедсиленце декодера мфпкэй \_

Указывает максимальное количество дополнительных выборок PCM, которые могут быть возвращены в конце после декодирования файла.

## <a name="constant-for-ipropertybag"></a>Константа для Ипропертибаг

Доступно только с помощью [**ипропертисторе**](/windows/win32/api/propsys/nn-propsys-ipropertystore).

## <a name="data-type"></a>Тип данных

VT \_ I4

## <a name="default-value"></a>Значение по умолчанию

2048

## <a name="remarks"></a>Комментарии

Это свойство можно использовать для оценки искусственного тишина, который вставляется между песнями по мере того, как они помещаются в декодер один за другим.

для Windows media audio 10 Professional и Windows декодеров media audio 9 без потерь это свойство всегда равно 0.

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

 

 
