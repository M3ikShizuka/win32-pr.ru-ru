---
description: Указывает длительность презентации в единицах 100-наносекундных.
ms.assetid: abc21696-ea97-41ff-9341-6d9e9dcb19ec
title: Атрибут MF_PD_DURATION (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9662e68c2380ad1ef9d009302a08d8798ab228fae0fe2b00528d37a4f7269c33
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119664104"
---
# <a name="mf_pd_duration-attribute"></a>\_ \_ Атрибут DURATION для MF PD

Указывает длительность презентации в единицах 100-наносекундных.

## <a name="data-type"></a>Тип данных

**UINT64**

Рассматривать как значение **лонглонг** .

## <a name="remarks"></a>Remarks

Источники мультимедиа могут установить этот атрибут для дескриптора презентации, чтобы указать длительность презентации.

Этот атрибут имеет значение со знаком, хотя оно хранится в виде **UINT64**. Однако атрибут не должен содержать отрицательное значение.

Константа GUID для этого атрибута экспортируется из мфууид. lib.

## <a name="examples"></a>Примеры

В следующем примере показано, как получить длительность презентации из источника мультимедиа.


```C++
HRESULT GetSourceDuration(IMFMediaSource *pSource, MFTIME *pDuration)
{
    *pDuration = 0;

    IMFPresentationDescriptor *pPD = NULL;

    HRESULT hr = pSource->CreatePresentationDescriptor(&pPD);
    if (SUCCEEDED(hr))
    {
        hr = pPD->GetUINT64(MF_PD_DURATION, (UINT64*)pDuration);
        pPD->Release();
    }
    return hr;
}
```



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Приложения UWP для классических приложений Vista \|\]<br/>                              |
| Минимальная версия сервера<br/> | Windows \[Приложения UWP для классических приложений сервера 2008 \|\]<br/>                        |
| Заголовок<br/>                   | <dl> <dt>Мфидл. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[**Имфаттрибутес:: UINT64**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getuint64)
</dt> <dt>

[**Имфаттрибутес:: SetUINT64**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint64)
</dt> <dt>

[**имфпресентатиондескриптор**](/windows/desktop/api/mfidl/nn-mfidl-imfpresentationdescriptor)
</dt> <dt>

[Атрибуты дескриптора представления](presentation-descriptor-attributes.md)
</dt> <dt>

[Дескрипторы представления](presentation-descriptors.md)
</dt> </dl>

 

 




