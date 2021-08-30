---
description: Происходит при формировании нового отчета широты/долготы.
ms.assetid: 2b1a25a1-ccd6-43f8-979b-c2d414d666a2
title: Событие Невлатлонгрепорт
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- NewLatLongReport
api_type:
- COM
api_location: ''
ms.openlocfilehash: 3cc8a46267927aaf7bf3011acbd05a32244fd0dcd8cc354a2bde1a299aaca624
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120129804"
---
# <a name="newlatlongreport-event"></a>Событие Невлатлонгрепорт

\[Объектная модель API расположения доступна для использования в операционных системах, указанных в разделе требования. В последующих версиях он может быть изменен или недоступен. Вместо этого для доступа к расположению с веб-сайта используйте [API географического расположения W3C](/previous-versions/windows/internet-explorer/ie-developer/samples/gg589513(v=vs.85)). Чтобы получить доступ к расположению из классического приложения, используйте [**Windows. API Devices. Географическое расположение**](/uwp/api/Windows.Devices.Geolocation) .\]

Происходит при формировании нового отчета широты/долготы.

## <a name="syntax"></a>Синтаксис


```JScript
.NewLatLongReport(
  newReport
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*неврепорт* 
</dt> <dd>

Новый объект [**локатиондисп. дисплатлонгрепорт**](locationdisp-displatlongreport.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="examples"></a>Примеры

Пример использования этого события см. в разделе [Listening for LatLong Reports Events](/uwp/api/Windows.Devices.Geolocation).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/> |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                  |



 

