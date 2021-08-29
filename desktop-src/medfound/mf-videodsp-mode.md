---
description: Задает режим обработки Стабилизация видео MFT.
ms.assetid: 0D49892A-8628-4F2B-B41B-51160A19DC9B
title: Атрибут MF_VIDEODSP_MODE (Вмкодекдсп. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 29cb1aff27fb0c4077e26ef47b1cb19804e12d968158e39c34a7b3aa131bbe50
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119955034"
---
# <a name="mf_videodsp_mode-attribute"></a>\_ \_ Атрибут режима видеодсп MF

Задает режим обработки [**стабилизация видео MFT**](video-stabilization-mft.md).

## <a name="data-type"></a>Тип данных

**Мфвидеодспмоде** хранится в виде **UIINT32**

## <a name="remarks"></a>Remarks

Значением этого атрибута является значение перечисления [**мфвидеодспмоде**](/windows/desktop/api/wmcodecdsp/ne-wmcodecdsp-mfvideodspmode) . Этот атрибут можно использовать для включения или отключения образа стабилизации и может быть обновлен для каждого образца выходных данных.

Чтобы задать этот атрибут, сделайте следующее:

1.  Вызовите [**имфтрансформ:: OutAttribute**](/windows/desktop/api/mftransform/nf-mftransform-imftransform-getattributes) в файле MFT видео стабилизации, чтобы получить указатель [**имфаттрибутес**](/windows/desktop/api/mfobjects/nn-mfobjects-imfattributes) .
2.  Вызовите метод [**имфаттрибутес:: SetUINT32**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-setuint32) , чтобы задать атрибут.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                              |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                    |
| Заголовок<br/>                   | <dl> <dt>Вмкодекдсп. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[**Стабилизация видео MFT**](video-stabilization-mft.md)
</dt> </dl>

 

 




