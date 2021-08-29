---
description: Некоторые свойства и поля данных содержат массивы данных.
ms.assetid: 85e3b953-be36-4d60-b04e-4f572d0b9564
title: Получение типов векторов
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d15579d7067d0eafba0d181d8e8845dfa1bd78b060fb5fba8b08f196d2107d3e
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119739464"
---
# <a name="retrieving-vector-types"></a>Получение типов векторов

Некоторые свойства и поля данных содержат массивы данных. Например, \_ \_ свойство "Кривое" светлого ответа Свойства датчика \_ \_ содержит массив из 4-байтных целых чисел без знака. Однако при получении таких массивов через API датчика они всегда представляются как тип VT \_ vector \| UI1, массив однобайтовых символов, независимо от фактического типа данных в массиве. Для этих типов необходимо соблюдать осторожность при приведении переменных массива к правильному типу данных для свойства или поля данных.

Сведения о свойствах, полях данных и их типах см. в разделе [константы](constants.md).

В следующем примере кода показано, как выполнить приведение данных, полученных \_ с \_ помощью кривой светлого ответа Свойства датчика, \_ \_ к правильному типу.


```C++
PROPVARIANT pvCurve;
PropVariantInit(&pvCurve);

// Retrieve the property value.
hr = pSensor->GetProperty(SENSOR_PROPERTY_LIGHT_RESPONSE_CURVE, &pvCurve);
if (SUCCEEDED(hr))
{
    if ((VT_UI1|VT_VECTOR) == V_VT(pvCurve)) // Note actual type of UI1
    {
        // Cast the array to UINT, a 4-byte unsigned integer.

        // Item count for the array.
        UINT  cElement = pvCurve.caub.cElems/sizeof(UINT);
        // Array pointer.
        UINT* pElement = (UINT*)(pvCurve.caub.pElems);

        // Use the array.
    }
}

// Remember to free the PROPVARIANT when done.
PropVariantClear(&pvCurve);
```



 

 



