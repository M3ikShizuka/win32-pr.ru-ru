---
title: Получение сообщений Running-Status
description: Получение сообщений Running-Status
ms.assetid: 4f2e8e41-89f6-45e3-ae16-47b856f0e63e
keywords:
- Цифровой интерфейс музыкального инструмента (MIDI), состояние выполнения
- MIDI (цифровой интерфейс музыкального инструмента), состояние выполнения
- запись звука MIDI, состояние выполнения
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a0a4d12a19f525a6fa673747063774bf4507d65b
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370920"
---
# <a name="receiving-running-status-messages"></a>Получение сообщений Running-Status

*Стандартная спецификация файлов MIDI 1,0* позволяет использовать *состояние выполнения* , если сообщение имеет тот же самый байт состояния, что и предыдущее сообщение. Если используется состояние выполнения, то байт состояния последующих сообщений можно опустить. Все драйверы устройств ввода MIDI необходимы для расширения сообщений, использующих состояние выполнения, в полные сообщения, чтобы всегда отправлять сообщения MIDI от драйвера устройства ввода MIDI.

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Запись звука MIDI](recording-midi-audio.md)
</dt> </dl>

 

 




