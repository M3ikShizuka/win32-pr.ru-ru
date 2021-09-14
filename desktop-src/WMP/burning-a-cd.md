---
title: Запись компакт-диска
description: Запись компакт-диска
ms.assetid: df55479e-d8a7-443d-bf2c-c988bfd0b1be
keywords:
- проигрыватель Windows Media, запись компакт-дисков
- проигрыватель Windows Media объектной модели, запись компакт-диска
- Объектная модель, запись компакт-диска
- проигрыватель Windows Media ActiveX управления, запись компакт-дисков
- ActiveX управления, запись компакт-дисков
- проигрыватель Windows Media мобильный ActiveX элемент управления, запись компакт-дисков
- проигрыватель Windows Media Мобильные устройства, запись компакт-дисков
- Запись компакт-дисков, о программе
- запись компакт-дисков, сведения
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 007b7808ff375ab0673592d0d016f8e713321d1a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126889536"
---
# <a name="burning-a-cd"></a>Запись компакт-диска

В этом разделе описывается, как использовать интерфейс [ивмпкдромбурн](/previous-versions/windows/desktop/api/wmp/nn-wmp-iwmpcdromburn) для записи музыки на компакт-диск. Интерфейс **ивмпкдромбурн** предоставляет функциональные возможности для записи списков воспроизведения на компакт-диски в виде данных или звуковых дорожек, а также для стирания CD RWS.

Использование кода

В примерах кода в этом разделе используются классы библиотеки активных шаблонов (ATL), такие как **CComPtr**.

Включаемые заголовки

Чтобы использовать код в этом разделе, включите следующие заголовки:


```C++
#include <atlbase.h>
#include <atlcom.h>
#include <atlwin.h>
#include <commctrl.h>
#include "wmp.h"
#include "wmpids.h"

```



Указатели интерфейса

интерфейсы для проигрыватель Windows Media хранятся в следующих переменных члена:


```C++
// Player interface.
CComPtr<IWMPPlayer>             m_spPlayer;

// CDROM interfaces.
CComPtr<IWMPCdromCollection>    m_spCdromCollection;
CComPtr<IWMPCdrom>              m_spCdrom;
CComPtr<IWMPCdromBurn>          m_spCdromBurn;
CComPtr<IWMPPlaylist>           m_spPlaylist;

```



В следующих разделах описывается использование API записи компакт-дисков.

-   [Получение интерфейса записи компакт-дисков](retrieving-the-cd-burning-interface.md)
-   [Запуск процесса записи](starting-the-burn-process.md)
-   [Стирание перезаписываемого компакт-диска](erasing-a-rewritable-cd.md)
-   [Получение состояния диска и диска](retrieving-the-drive-and-disc-status.md)
-   [Получение состояния записи](retrieving-the-burn-status.md)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Управление проигрывателем**](player-control-guide.md)
</dt> </dl>

 

 




