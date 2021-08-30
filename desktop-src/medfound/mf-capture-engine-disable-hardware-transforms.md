---
description: Отключает использование преобразований Media Foundation на основе оборудования (МФТС) в подсистеме записи.
ms.assetid: 1C687FEC-276D-4759-A3B8-9A2A31CB0DE1
title: Атрибут MF_CAPTURE_ENGINE_DISABLE_HARDWARE_TRANSFORMS (Mfcaptureengine. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7818e79a78ab346ffb8a1967569fdd8711e2b948e0eb656f032770487d8820ef
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119956814"
---
# <a name="mf_capture_engine_disable_hardware_transforms-attribute"></a>\_Атрибут MF \_ \_ Отключить \_ аппаратные \_ преобразования для ядра записи

Отключает использование преобразований Media Foundation на основе оборудования (МФТС) в подсистеме записи.

## <a name="data-type"></a>Тип данных

**Bool** , сохраненный как **UINT32**

## <a name="remarks"></a>Remarks

По умолчанию подсистема отслеживания использует аппаратные декодеры или кодировщики. Чтобы отключить использование оборудования МФТС, установите для этого атрибута значение **true** при создании подсистемы захвата.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                                   |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                         |
| Заголовок<br/>                   | <dl> <dt>Mfcaptureengine. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Атрибуты подсистемы захвата](capture-engine-attributes.md)
</dt> <dt>

[**Имфкаптурингине:: Initialize**](/windows/desktop/api/mfcaptureengine/nf-mfcaptureengine-imfcaptureengine-initialize)
</dt> </dl>

 

 




