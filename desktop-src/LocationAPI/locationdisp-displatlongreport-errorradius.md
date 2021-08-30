---
description: Расстояние от сообщаемого места в метрах. В сочетании с исходным расположением в качестве источника этот радиус описывает круг, в котором может находиться фактическое расположение.
ms.assetid: a9565bd5-d1e0-45f8-abeb-3191b16480fa
title: Локатиондисп. Дисплатлонгрепорт. Ерроррадиус, свойство
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- LocationDisp.DispLatLongReport.ErrorRadius
api_type:
- COM
api_location: ''
ms.openlocfilehash: 6e331d6001acbdbb7aa97689fdda272a55227f202e8a28c6ba77b56357465dba
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120130004"
---
# <a name="locationdispdisplatlongreporterrorradius-property"></a>Локатиондисп. Дисплатлонгрепорт. Ерроррадиус, свойство

\[Объектная модель API расположения доступна для использования в операционных системах, указанных в разделе требования. В последующих версиях он может быть изменен или недоступен. Вместо этого для доступа к расположению с веб-сайта используйте [API географического расположения W3C](/previous-versions/windows/internet-explorer/ie-developer/samples/gg589513(v=vs.85)). Чтобы получить доступ к расположению из классического приложения, используйте [**Windows. API Devices. Географическое расположение**](/uwp/api/Windows.Devices.Geolocation) .\]

Расстояние от сообщаемого места в метрах. В сочетании с исходным расположением в качестве источника этот радиус описывает круг, в котором может находиться фактическое расположение.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
ErrorRadius = LocationDisp.DispLatLongReport.ErrorRadius
```



## <a name="property-value"></a>Значение свойства

Это свойство доступно только для чтения ( **число** с плавающей запятой двойной точности).

## <a name="examples"></a>Примеры

Пример использования этого свойства см. [в примере простого отчета LatLong](/uwp/api/Windows.Devices.Geolocation).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/> |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                  |



 

