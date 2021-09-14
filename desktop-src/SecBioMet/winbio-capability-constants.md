---
title: Константы WINBIO_CAPABILITY (Винбио \_ types. h)
description: Подтипы датчика отпечатков пальцев.
ms.assetid: D447273E-2A02-484E-B0E4-69FEADD15797
topic_type:
- apiref
api_name:
- WINBIO_CAPABILITY_SENSOR
- WINBIO_CAPABILITY_MATCHING
- WINBIO_CAPABILITY_DATABASE
- WINBIO_CAPABILITY_PROCESSING
- WINBIO_CAPABILITY_ENCRYPTION
- WINBIO_CAPABILITY_NAVIGATION
- WINBIO_CAPABILITY_INDICATOR
- WINBIO_CAPABILITY_VIRTUAL_SENSOR
api_location:
- winbio_types.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: bfd98b4831d5e3dfa13aea365d6ed9ddd30960ee
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064617"
---
# <a name="winbio_capability-constants"></a>\_Константы возможностей винбио

Следующие подтипы датчика отпечатков пальцев — это значения **\_ возможностей винбио** , которые можно использовать в качестве битовой маски для параметра *CAPABILITIES* структуры [**\_ \_ схемы единицы винбио**](winbio-unit-schema.md) . Они относятся к возможностям встроенного датчика.




| Константа/значение | Описание | 
|----------------|-------------|
| <span id="WINBIO_CAPABILITY_SENSOR"></span><span id="winbio_capability_sensor"></span><dl><dt><strong>WINBIO_CAPABILITY_SENSOR</strong></dt><dt>0x00000001</dt></dl> | Датчик может записывать биометрические данные.<br /> | 
| <span id="WINBIO_CAPABILITY_MATCHING"></span><span id="winbio_capability_matching"></span><dl><dt><strong>WINBIO_CAPABILITY_MATCHING</strong></dt><dt>0x00000002</dt></dl> | Датчик может сопоставлять биометрические данные с удостоверением.<br /> | 
| <span id="WINBIO_CAPABILITY_DATABASE"></span><span id="winbio_capability_database"></span><dl><dt><strong>WINBIO_CAPABILITY_DATABASE</strong></dt><dt>0x00000004</dt></dl> | Датчик содержит встроенную базу данных.<br /> | 
| <span id="WINBIO_CAPABILITY_PROCESSING"></span><span id="winbio_capability_processing"></span><dl><dt><strong>WINBIO_CAPABILITY_PROCESSING</strong></dt><dt>0x00000008</dt></dl> | Датчик может выполнять биометрическую обработку.<br /> | 
| <span id="WINBIO_CAPABILITY_ENCRYPTION"></span><span id="winbio_capability_encryption"></span><dl><dt><strong>WINBIO_CAPABILITY_ENCRYPTION</strong></dt><dt>0x00000010</dt></dl> | Датчик может шифровать биометрические данные.<br /> | 
| <span id="WINBIO_CAPABILITY_NAVIGATION"></span><span id="winbio_capability_navigation"></span><dl><dt><strong>WINBIO_CAPABILITY_NAVIGATION</strong></dt><dt>0x00000020</dt></dl> | Датчик может работать как клавиатура мыши. В настоящее время это не поддерживается.<br /> | 
| <span id="WINBIO_CAPABILITY_INDICATOR"></span><span id="winbio_capability_indicator"></span><dl><dt><strong>WINBIO_CAPABILITY_INDICATOR</strong></dt><dt>0x00000040</dt></dl> | Датчик содержит индикатор индикатора.<br /> | 
| <span id="WINBIO_CAPABILITY_VIRTUAL_SENSOR"></span><span id="winbio_capability_virtual_sensor"></span><dl><dt><strong>WINBIO_CAPABILITY_VIRTUAL_SENSOR</strong></dt><dt>0x00000080</dt></dl> | Адаптер датчика управляет собственным подключением к биометрической оборудованию.<br /><blockquote>[!Note]<br />эта константа применяется только для Windows 10 и более поздних версий.</blockquote><br /> | 




## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                                                                                                               |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/>                                                                                                                  |
| Заголовок<br/>                   | <dl> <dt>Винбио \_ types. h (включите винбио. h для клиентских приложений или винбио \_ Adapters. h для адаптеров).</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Константы клиентского приложения](client-application-constants.md)
</dt> <dt>

[**\_схема единицы \_ винбио**](winbio-unit-schema.md)
</dt> </dl>

 

 





