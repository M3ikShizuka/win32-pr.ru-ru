---
description: Указывает список битовых ставок и соответствующих окон буфера для файла с переменным битом (VBR) расширенного формата системы (ASF).
ms.assetid: e45d055f-d404-47e9-b3c8-ac743b290138
title: Атрибут MF_PD_ASF_METADATA_LEAKY_BUCKET_PAIRS (Вмконтаинер. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7426d15a806a8c61c9a2ea1fdfb0565372c5f48f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127579874"
---
# <a name="mf_pd_asf_metadata_leaky_bucket_pairs-attribute"></a>\_ \_ \_ \_ \_ Атрибут пар контейнеров утечки метаданных MF PD ASF \_

Указывает список битовых ставок и соответствующих окон буфера для файла с переменным битом (VBR) расширенного формата системы (ASF).

## <a name="data-type"></a>Тип данных

массив байтов;

## <a name="remarks"></a>Remarks

Этот атрибут применяется к дескрипторам представления для содержимого ASF.

Метод [**имфасфконтентинфо:: женератепресентатиондескриптор**](/windows/desktop/api/wmcontainer/nf-wmcontainer-imfasfcontentinfo-generatepresentationdescriptor) создает этот атрибут, который применяется к дескриптору представления для содержимого ASF.

Значение атрибута имеет следующий формат:

``` syntax
struct {
    WORD wReserved;
    WM_LEAKY_BUCKET_PAIR bucket[2];
};
```

Структура **\_ \_ \_ пары контейнеров с утечками WM** определяется следующим образом:

``` syntax
typedef struct _WMLeakyBucketPair {
  DWORD  dwBitrate;
  DWORD  msBufferWindow;
} WM_LEAKY_BUCKET_PAIR;
```

Для каждой скорости потока элемент **мсбуффервиндов** указывает, сколько содержимого буферизовано до начала воспроизведения, в миллисекундах. Размер буфера в байтах равен **мсбуффервинов** x **двбитрате** /8000.

> [!Note]  
> этот атрибут соответствует атрибуту **асфлеакибуккетпаирс** в пакете SDK для Windows Media Format.

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                     |
| Заголовок<br/>                   | <dl> <dt>Вмконтаинер. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[**Имфаттрибутес:: BLOB**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getblob)
</dt> <dt>

[**Имфаттрибутес:: SetBlob**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setblob)
</dt> <dt>

[**имфпресентатиондескриптор**](/windows/desktop/api/mfidl/nn-mfidl-imfpresentationdescriptor)
</dt> <dt>

[Атрибуты дескриптора представления](presentation-descriptor-attributes.md)
</dt> <dt>

[Объект заголовка ASF](asf-file-structure.md)
</dt> <dt>

[Дескрипторы представления](presentation-descriptors.md)
</dt> </dl>

 

 




