---
title: Определение уровней серьезности
description: Уровни используются для группирования событий и обычно указывают на серьезность или уровень детализации события.
ms.assetid: dfa4e0a9-4d89-4f50-aef9-1dae0dc11726
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 1c8e2e979e75057a77cca267e540b3ec5469562f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126885536"
---
# <a name="defining-severity-levels"></a>Определение уровней серьезности

Уровни используются для группирования событий и обычно указывают на серьезность или уровень детализации события. Чтобы определить уровень, используйте элемент **Level** . Файл Winmeta.xml определяет следующие часто используемые уровни серьезности:

-   win:Critical
-   win:Error
-   win:Warning
-   win:Informational
-   win:Verbose

Потребители используют уровни для запроса событий, содержащих определенное значение уровня. Сеанс трассировки ETW также может использовать уровни для ограничения событий, записываемых в файл журнала трассировки событий. события со значением уровня, равным или меньшим указанного значения уровня, записываются в файл журнала. Например, если сеанс указал значение уровня для Win: Warning, файл журнала будет содержать предупреждения, ошибки и критические события.

В следующем примере показано, как определить уровень. Необходимо указать атрибуты **имени** и **значения** уровня. Значение атрибута **value** должно находиться в диапазоне от 16 до 255. Атрибуты **symbol** и **Message** являются необязательными.


```XML
<instrumentationManifest
    xmlns="http://schemas.microsoft.com/win/2004/08/events" 
    xmlns:win="http://manifests.microsoft.com/win/2004/08/windows/events"
    xmlns:xs="http://www.w3.org/2001/XMLSchema"
    >

    <instrumentation>
        <events>
            <provider name="Microsoft-Windows-SampleProvider"
                guid="{1db28f2e-8f80-4027-8c5a-a11f7f10f62d}"
                symbol="PROVIDER_GUID"
                resourceFileName="<path to the exe or dll that contains the metadata resources>"
                messageFileName="<path to the exe or dll that contains the string resources>"
                message="$(string.Provider.Name)">

                . . .

                <levels>
                    <level name="NotValid"
                           value="16"
                           symbol="LEVEL_SAMPLEPROVIDER_NOTVALID"
                           message="$(string.Level.NotValid)"/>
                    <level name="Valid"
                           value="17"
                           symbol="LEVEL_SAMPLEPROVIDER_VALID"
                           message="$(string.Level.Valid)"/>
                </levels>

                . . .

            </provider>
        </events>
    </instrumentation>

    <localization>
        <resources culture="en-US">
            <stringTable>
                <string id="Provider.Name" value="Sample Provider"/>
                <string id="Level.Valid" value="Valid"/>
                <string id="Level.NotValid" value="Not Valid"/>
            </stringTable>
        </resources>
    </localization>

</instrumentationManifest>
```
