---
description: Отключает использование преобразований Media Foundation на основе оборудования (МФТС) в подсистеме записи.
ms.assetid: 1C687FEC-276D-4759-A3B8-9A2A31CB0DE1
title: Атрибут MF_CAPTURE_ENGINE_DISABLE_HARDWARE_TRANSFORMS (Mfcaptureengine. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d9631804c61fab953793c3f89d1eac3dc2e8f4dc
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127580411"
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

 

 




