---
description: После создания расширения оснастки вложения необходимо зарегистрировать его, чтобы оснастки MMC и настройки безопасности могли их искать и использовать.
ms.assetid: 176a658c-b1fd-40c5-a2ac-c9a2b7060c55
title: Регистрация расширения оснастки "вложение"
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 7726131325433aa920ff22c9b71a4f7184000a69
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064590"
---
# <a name="registering-an-attachment-snap-in-extension"></a>Регистрация расширения оснастки "вложение"

После создания расширения оснастки вложения необходимо зарегистрировать его, чтобы оснастки MMC и настройки безопасности могли их искать и использовать.

Оснастка "вложение" должна расширить пространство имен оснастки "Настройка безопасности", добавив собственный узел, как описано в следующей процедуре.

**Установка и регистрация расширения оснастки «вложение»**

1.  Зарегистрируйте расширение оснастки в следующем разделе реестра. Не создавайте автономный ключ в оснастке. расширения оснасток вложения должны быть только расширениями.

    ```
    HKEY_LOCAL_MACHINE
       SOFTWARE
          Microsoft
             MMC
                SnapIns
    ```

2.  Зарегистрируйте расширение оснастки вложений в следующих подразделах. Это можно сделать в рамках реализации функций **DllRegisterServer** и **DllUnregisterServer** .

    Пространство имен [шаблонов безопасности](security-templates.md) :

    ```
    HKLM
       SOFTWARE
          Microsoft
             MMC
                NodeTypes
                   24a7f717-1f0c-11d1-affb-00c04fb984f9
                      Extensions
                         NameSpace
    ```

    Пространство имен [настройки и анализа безопасности](security-configuration-and-analysis.md) :

    ```
    HKLM
       SOFTWARE
          Microsoft
             MMC
                NodeTypes
                   678050c7-1ff8-11d1-affb-00c04fb984f9
                      Extensions
                         NameSpace
    ```

 

 



