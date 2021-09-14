---
title: Получение Time-Stamped сообщений MIDI
description: Получение Time-Stamped сообщений MIDI
ms.assetid: a91c85fe-f9c4-4cf6-b0bb-49aa8ed45644
keywords:
- Цифровой интерфейс MIDI, сообщения с отметкой времени
- MIDI (цифровой интерфейс музыкального инструмента), сообщения с штампом времени
- запись аудио MIDI, сообщений с штампом времени
- сообщения MIDI с отметкой времени
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f7ead268c6d022f67a3607bb8a43a3d773bd7325
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171568"
---
# <a name="receiving-time-stamped-midi-messages"></a>Получение Time-Stamped сообщений MIDI

Из-за задержки между тем, когда драйвер устройства получает сообщение MIDI и время, когда приложение получает сообщение, драйвер MIDI input Devices Time отмечает сообщение MIDI на время получения сообщения. Метки времени MIDI, которые определяются как время получения первого байта сообщения, указываются в миллисекундах. Функция [**мидиинстарт**](/windows/win32/api/mmeapi/nf-mmeapi-midiinstart) сбрасывает отметки времени для устройства в ноль.

Как упоминалось ранее, для получения меток времени с помощью ввода MIDI необходимо использовать функцию обратного вызова. параметр *dwParam2* функции обратного вызова задает отметку времени для данных, связанных с [**MIMными \_ данными**](mim-data.md) и [**MIM \_**](mim-longdata.md) сообщениями лонгдата.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Запись звука MIDI](recording-midi-audio.md)
</dt> </dl>

 

 