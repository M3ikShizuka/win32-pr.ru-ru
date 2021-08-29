---
description: Определяет тип уведомления, передаваемого \_ \_ \_ \_ функции обратного вызова уведомления приемника WFD.
ms.assetid: C0AFF80E-A4D2-4FF1-B111-D628AF8755A8
title: Перечисление WFD_DISPLAY_SINK_NOTIFICATION_TYPE (Вфдсинк. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- WFD_DISPLAY_SINK_NOTIFICATION_TYPE
api_type:
- HeaderDef
api_location:
- wfdsink.h
ms.openlocfilehash: ca16197da0137e40c25a75c139773b02674b6bf7c90bcae2b94ae0845d201e71
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119800614"
---
# <a name="wfd_display_sink_notification_type-enumeration"></a>\_ \_ \_ Перечисление типов уведомлений приемника для дисплея WFD \_

Тип **\_ \_ \_ уведомления \_ sink дисплея WFD** определяет тип уведомления, передаваемого функции [**\_ \_ \_ \_ обратного вызова уведомления приемника WFD**](wfd-display-sink-notification-callback.md) .

## <a name="syntax"></a>Синтаксис


```C++
typedef enum _WFD_DISPLAY_SINK_NOTIFICATION_TYPE { 
  ProvisioningRequestNotification,
  ReconnectRequestNotification,
  ConnectedNotification,
  DisconnectedNotification
} WFD_DISPLAY_SINK_NOTIFICATION_TYPE, *PWFD_DISPLAY_SINK_NOTIFICATION_TYPE;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="ProvisioningRequestNotification"></span><span id="provisioningrequestnotification"></span><span id="PROVISIONINGREQUESTNOTIFICATION"></span>**провисионингрекуестнотификатион**
</dt> <dd>

Уведомление — это запрос на подготовку.

</dd> <dt>

<span id="ReconnectRequestNotification"></span><span id="reconnectrequestnotification"></span><span id="RECONNECTREQUESTNOTIFICATION"></span>**реконнектрекуестнотификатион**
</dt> <dd>

Уведомление является запросом на повторное подключение.

</dd> <dt>

<span id="ConnectedNotification"></span><span id="connectednotification"></span><span id="CONNECTEDNOTIFICATION"></span>**коннектеднотификатион**
</dt> <dd>

Уведомление является подключенным уведомлением.

</dd> <dt>

<span id="DisconnectedNotification"></span><span id="disconnectednotification"></span><span id="DISCONNECTEDNOTIFICATION"></span>**дисконнектеднотификатион**
</dt> <dd>

Уведомление является отключенным уведомлением.

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ только классические приложения\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows Server 2012 \[Только классические приложения R2\]<br/>                              |
| Заголовок<br/>                   | <dl> <dt>Вфдсинк. h</dt> </dl> |



 

 




