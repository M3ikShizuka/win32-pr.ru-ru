---
title: Запрос устройств ввода MIDI
description: Запрос устройств ввода MIDI
ms.assetid: 2da88418-f9cf-49da-b17f-8a26d357b5ab
keywords:
- Цифровой интерфейс MIDI, устройства ввода
- MIDI (цифровой интерфейс музыкального инструмента), устройства ввода
- запись аудио MIDI, устройств ввода
- Устройства ввода MIDI
- Цифровой интерфейс музыкальных инструментов (MIDI), запрос устройств ввода
- MIDI (цифровой интерфейс музыкального инструмента), запрос устройств ввода
- запись аудио MIDI, запрос устройств ввода
- запрос устройств ввода MIDI
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 7a92bec8733887e20c25f37d1de3dd493e555c8a
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370914"
---
# <a name="querying-midi-input-devices"></a>Запрос устройств ввода MIDI

Перед записью звука MIDI следует использовать функцию [**мидиинжетдевкапс**](/windows/win32/api/mmeapi/nf-mmeapi-midiingetdevcaps) для определения возможностей входного устройства MIDI, присутствующего в системе. Эта функция принимает адрес структуры [**мидиинкапс**](/windows/win32/api/mmeapi/ns-mmeapi-midiincaps) , которая заполняется сведениями о возможностях данного устройства. Эти сведения включают в себя изготовителя и идентификаторы продуктов, название продукта для устройства и номер версии драйвера устройства.

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Запись звука MIDI](recording-midi-audio.md)
</dt> </dl>

 

 