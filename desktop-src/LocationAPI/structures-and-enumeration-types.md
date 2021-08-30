---
description: API расположения определяет следующие типы перечислений.
ms.assetid: a1d9d274-2861-4818-8fa1-d8d66edf27b3
title: Структуры и типы перечислений (API Location)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3e8cfea31e8822147cc33710239b31dcd4b982ca3b523dfb6f118d1969af703c
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120129814"
---
# <a name="structures-and-enumeration-types-location-api"></a>Структуры и типы перечислений (API Location)

\[API расположения Win32 доступен для использования в операционных системах, указанных в разделе требования. В последующих версиях он может быть изменен или недоступен. Вместо этого используйте [**Windows. API Devices. Географическое расположение**](/uwp/api/Windows.Devices.Geolocation) . \]

API расположения определяет следующие типы перечислений.



| Перечисление                                                                       | Описание                                                          |
|-----------------------------------------------------------------------------------|----------------------------------------------------------------------|
| [**\_Требуемая \_ точность расположения**](/previous-versions/windows/desktop/legacy/dd756639(v=vs.85))                  | Определяет возможные типы точности.                         |
| [**\_состояние отчета о расположении \_**](/windows/win32/api/locationapi/ne-locationapi-location_report_status) | Определяет возможное состояние для новых отчетов определенного типа отчета. |



 

## <a name="location-constants-from-the-sensor-api"></a>Константы расположения из API датчика

API датчика также определяет связанные с расположением ключи и константы свойств. Ключи свойств, определенные в sensors. h, можно использовать для получения данных о местоположении из отчета путем вызова [**илокатионрепорт:: GetValue**](/windows/win32/api/locationapi/nf-locationapi-ilocationreport-getvalue).

 

 
