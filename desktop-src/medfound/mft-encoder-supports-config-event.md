---
description: Указывает, что кодировщик MFT поддерживает получение событий Минкодингпараметер во время потоковой передачи.
ms.assetid: 8DE04537-641C-4154-9C7F-A7D025CA4C39
title: Атрибут MFT_ENCODER_SUPPORTS_CONFIG_EVENT (Мфтрансформ. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c49c688abc4d372a463115c369e4616babe3bcaa
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127469106"
---
# <a name="mft_encoder_supports_config_event-attribute"></a>\_КОДИРОВЩИК MFT \_ поддерживает \_ \_ атрибут события конфигурации

Указывает, что кодировщик MFT поддерживает получение событий [минкодингпараметер](meencodingparameters.md) во время потоковой передачи.

## <a name="data-type"></a>Тип данных

**Bool** , сохраненный как **UINT32**

## <a name="remarks"></a>Remarks

Отправляется кодировщиком MFT через [**имфтрансформ::P роцессевент**](/windows/desktop/api/mftransform/nf-mftransform-imftransform-processevent).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ приложения UWP для классических приложений \|\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Server 2012 Приложения универсального \[ приложения UWP для настольных приложений \|\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>Мфтрансформ. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Мфтрансформ. idl</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Алфавитный список атрибутов Media Foundation](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[**Имфтрансформ::P Роцессевент**](/windows/desktop/api/mftransform/nf-mftransform-imftransform-processevent)
</dt> </dl>

 

 




