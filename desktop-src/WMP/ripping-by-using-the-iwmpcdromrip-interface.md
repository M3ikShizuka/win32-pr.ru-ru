---
title: Копирование с помощью интерфейса Ивмпкдромрип
description: Копирование с помощью интерфейса Ивмпкдромрип
ms.assetid: 7622072e-82e1-4e31-ad80-ddc3473b5841
keywords:
- проигрыватель Windows Media, копирование компакт-дисков
- проигрыватель Windows Mediaная модель объектов, копирование компакт-дисков
- Объектная модель, копирование компакт-дисков
- проигрыватель Windows Media ActiveX управления, копирование компакт-дисков
- ActiveX управления, копирование компакт-дисков
- проигрыватель Windows Media мобильный ActiveX управление, копирование компакт-дисков
- проигрыватель Windows Media Мобильные устройства, копирование компакт-дисков
- Копирование компакт-дисков, интерфейс Ивмпкдромрип
- Копирование компакт-дисков, интерфейс Ивмпкдромрип
- Интерфейс Ивмпкдромрип
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4fcf2e959d10385365075bb20e1c04c2d796ad2e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127469641"
---
# <a name="ripping-by-using-the-iwmpcdromrip-interface"></a>Копирование с помощью интерфейса Ивмпкдромрип

В этом разделе описывается использование интерфейса [ивмпкдромрип](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmpcdromrip) для копирования музыки с компакт-диска.

копирование компакт-диска с помощью интерфейса **ивмпкдромрип** действует так же, как копирование музыки с помощью пользовательского интерфейса проигрыватель Windows Media. Скопированное содержимое автоматически добавляется в библиотеку в соответствии с предпочтениями пользователя. дополнительные сведения о копировании компакт-дисков см. в подразделе «копирование музыки с cd» раздела справка проигрыватель Windows Media.

В примерах кода в этом разделе используются классы библиотеки активных шаблонов (ATL), такие как **CComPtr**.

## <a name="included-headers"></a>Включаемые заголовки

Чтобы использовать код в этом разделе, включите следующие заголовки:


```C++
#include <atlbase.h>
#include <atlcom.h>
#include <atlwin.h>
#include <commctrl.h>
#include "wmp.h"
#include "wmpids.h"

```



## <a name="interface-pointers"></a>Указатели интерфейса

интерфейсы для проигрыватель Windows Media хранятся в следующих переменных члена.


```C++
// Player interface.
CComPtr<IWMPPlayer>             m_spPlayer;

// CDROM interfaces.
CComPtr<IWMPCdromCollection>    m_spCdromCollection;
CComPtr<IWMPCdrom>              m_spCdrom;
CComPtr<IWMPCdromRip>           m_spCdromRip;
CComPtr<IWMPPlaylist>           m_spPlaylist;

```



В следующих разделах описывается использование интерфейса Ивмпкдромрип

-   [Получение интерфейса копирования данных с компакт-диска](retrieving-the-ripping-interface.md)
-   [Запуск процесса копирования](starting-the-rip-process.md)
-   [Получение состояния копирования](retrieving-the-rip-status.md)
-   [Выбор элементов для копирования](selecting-items-for-ripping.md)

 

 




