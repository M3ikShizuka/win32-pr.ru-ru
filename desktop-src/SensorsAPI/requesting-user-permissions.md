---
description: В этом разделе описывается, как запросить у пользователя разрешения на использование датчиков. Общие сведения о разрешениях в API датчика см. в разделе Управление разрешениями пользователей.
ms.assetid: e43ad497-86f1-4804-a67a-0aeb56b80d7f
title: Запрос разрешений пользователя
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b2bb6c977306ff68f40fb8d3a77b598114cb6f77feeb35d4beca96c05fbce224
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119992684"
---
# <a name="requesting-user-permissions"></a>Запрос разрешений пользователя

В этом разделе описывается, как запросить у пользователя разрешения на использование датчиков. Общие сведения о разрешениях в API датчика см. в разделе [Управление разрешениями пользователей](managing-user-permissions.md).

В следующих примерах показаны некоторые распространенные сценариаус, в которых можно запросить разрешения пользователя.

В следующем примере кода просто запрашиваются разрешения для всех датчиков, полученных от диспетчера датчиков, по типу с помощью асинхронного вызова метода. Платформа откроет диалоговое окно, в котором пользователю будет предложено только включить датчики, которые еще не включены. Чтобы определить, включил ли пользователь какие либо датчики в этом случае, необходимо выполнить обработку события [**исенсоревентс:: онстатечанжед**](/windows/win32/api/sensorsapi/nf-sensorsapi-isensorevents-onstatechanged) .


```C++
// Get the sensor collection.
hr = pSensorManager->GetSensorsByType(SAMPLE_SENSOR_TYPE_TIME, &pSensorColl);

if(SUCCEEDED(hr))
{
    // Request permissions for all sensors
    // in the collection.
    hr = pSensorManager->RequestPermissions(0, pSensorColl, FALSE);
}

```



Вы можете проверить состояние датчика в синхронном режиме, прежде чем пытаться получить данные. Этот метод показан в следующем примере кода.


```C++
if(SUCCEEDED(hr))
{
   // Check the current sensor state.
   SensorState state = SENSOR_STATE_NOT_AVAILABLE;

   hr = pSensor->GetState(&state);

   if(SUCCEEDED(hr))
   {
       if(state == SENSOR_STATE_ACCESS_DENIED)
       {
           wprintf_s(L"\nSensor not enabled, requesting permissions...\n");
           hr = pSensorManager->RequestPermissions(0, pSensorColl, TRUE);

           if(hr == HRESULT_FROM_WIN32(ERROR_ACCESS_DENIED) ||
              hr == HRESULT_FROM_WIN32(ERROR_CANCELLED)) 
           {
               wprintf_s(L"\nYou have previously denied access to this sensor.\n");
               wprintf_s(L"Please use the Location and Other Sensors control panel\n");
               wprintf_s(L"to enable the WDK Time Sensor and run this program again.\n");
           }
       }
   }
}

if(SUCCEEDED(hr))
{
    // Get the data report.
    hr = pSensor->GetData(&pReport);
}
```



В следующем примере кода пользователю предлагается разрешение датчика, если попытка извлечь отчет данных с определенного датчика завершается ошибкой.


```C++
if(SUCCEEDED(hr))
{
    // Get the data report.
    hr = pSensor->GetData(&pReport);

    if(E_ACCESSDENIED == hr)
    {
       wprintf_s(L"\nSensor not enabled, requesting permissions...\n");
       hr = pSensorManager->RequestPermissions(0, pSensorColl, TRUE);

       if(hr == HRESULT_FROM_WIN32(ERROR_ACCESS_DENIED) ||
          hr == HRESULT_FROM_WIN32(ERROR_CANCELLED)) 
       {
           wprintf_s(L"\nYou have previously denied access to this sensor.\n");
           wprintf_s(L"Please use the Location and Other Sensors control panel\n");
           wprintf_s(L"to enable the WDK Time Sensor and run this program again.\n");
       }
    }
}
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**исенсорманажер**](/windows/desktop/api/sensorsapi/nn-sensorsapi-isensormanager)
</dt> <dt>

[Управление разрешениями пользователей](managing-user-permissions.md)
</dt> </dl>

 

 
