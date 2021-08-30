---
title: Запуск процесса копирования
description: Запуск процесса копирования
ms.assetid: 82ffc114-ddad-41be-af80-6c1bd29cb0d4
keywords:
- проигрыватель Windows Media, копирование компакт-дисков
- проигрыватель Windows Mediaная модель объектов, копирование компакт-дисков
- Объектная модель, копирование компакт-дисков
- проигрыватель Windows Media ActiveX управления, копирование компакт-дисков
- ActiveX управления, копирование компакт-дисков
- проигрыватель Windows Media мобильный ActiveX управление, копирование компакт-дисков
- проигрыватель Windows Media Мобильные устройства, копирование компакт-дисков
- Копирование компакт-дисков, запуск процесса копирования с диска
- Копирование компакт-дисков, запуск процесса копирования
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 47d6d4e7bac4de9fc82f26d7231020e002570553ecdd6447c55f981601e5830a
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120002164"
---
# <a name="starting-the-rip-process"></a>Запуск процесса копирования

После получения интерфейса копирования, как описано в предыдущем разделе, запустите процесс копирования, вызвав [ивмпкдромрип:: стартрип](/previous-versions/windows/desktop/api/wmp/nf-wmp-iwmpcdromrip-startrip).


```C++
// Start ripping.
HRESULT hr = m_spCdromRip->startRip();

```



Можно прерывать операцию копирования путем вызова [ивмпкдромрип:: стоприп](/previous-versions/windows/desktop/api/wmp/nf-wmp-iwmpcdromrip-stoprip).


```C++
// Stop ripping.
HRESULT hr = m_spCdromRip->stopRip();

```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Копирование компакт-диска**](ripping-a-cd.md)
</dt> <dt>

[**Получение интерфейса копирования данных с компакт-диска**](retrieving-the-ripping-interface.md)
</dt> <dt>

[**Получение состояния копирования**](retrieving-the-rip-status.md)
</dt> <dt>

[**Выбор элементов для копирования**](selecting-items-for-ripping.md)
</dt> </dl>

 

 




