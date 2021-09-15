---
title: Константы WINBIO_INDICATOR_STATUS (Винбио \_ types. h)
description: Установите индикатор индикатора.
ms.assetid: 1e00ff9d-6693-4763-8ac3-b42d2a3e987d
topic_type:
- apiref
api_name:
- WINBIO_INDICATOR_ON
- WINBIO_INDICATOR_OFF
api_location:
- Winbio_types.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7693fbd2b9b37067738774d172f4bb482edb06e6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127469989"
---
# <a name="winbio_indicator_status-constants"></a>\_ \_ Константы состояния индикатора винбио

Чтобы задать индикатор индикатора, можно использовать следующие значения. По умолчанию датчики не имеют источника света, но приложения могут использовать эти значения для включения или отключения индикаторов индикатора. Значение **\_ \_ состояния датчика винбио** содержит более подробные сведения о состоянии индикатора индикаторов на. Дополнительные сведения см. в следующих функциях:

-   [**сенсорадаптерсетиндикаторстатус**](/windows/desktop/api/Winbio_adapter/nc-winbio_adapter-pibio_sensor_set_indicator_status_fn)
-   [**сенсорадаптержетиндикаторстатус**](/windows/desktop/api/Winbio_adapter/nc-winbio_adapter-pibio_sensor_get_indicator_status_fn)
-   [**сенсорадаптеркуеристатус**](/windows/desktop/api/Winbio_adapter/nc-winbio_adapter-pibio_sensor_query_status_fn)



| Константа                                                                                                                                                                            | Описание                                   |
|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------|
| <span id="WINBIO_INDICATOR_ON"></span><span id="winbio_indicator_on"></span><dl> <dt>**\_индикатор винбио \_ на**</dt> </dl>    | Индикатор датчика горит.<br/>  |
| <span id="WINBIO_INDICATOR_OFF"></span><span id="winbio_indicator_off"></span><dl> <dt>**\_индикатор винбио \_**</dt> </dl> | Индикатор датчика горит.<br/> |



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>                                                                    |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/>                                                       |
| Заголовок<br/>                   | <dl> <dt>Винбио \_ types. h (include винбио. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Константы клиентского приложения](client-application-constants.md)
</dt> </dl>

 

 





