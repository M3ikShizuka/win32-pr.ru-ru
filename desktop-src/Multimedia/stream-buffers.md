---
title: Буферы потока
description: Буферы потока
ms.assetid: d73209a3-4b9d-4405-9e62-8ecfb94c0bd5
keywords:
- Windows мультимедиа, буферы потоков
- мультимедиа, буферы потоков
- мультимедийные аудио, буферы потоков
- звук, буферы потоков
- Цифровой интерфейс музыкальных инструментов (MIDI), буферы потоков
- MIDI (цифровой интерфейс музыкального инструмента), буферы потоков
- буферы потоков, сведения
- Структура МИДИХДР
- Структура МИДИЕВЕНТ
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 8d4a01862a8a8e6b7846cbe445737bd13422cf0f
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371040"
---
# <a name="stream-buffers"></a>Буферы потока

Приложения могут использовать буферы потоков для отправки потоков событий MIDI на устройство. Каждый буфер потока — это блок памяти, на который указывает структура [**мидихдр**](/windows/win32/api/mmeapi/ns-mmeapi-midihdr) . Этот блок памяти содержит данные для одного или нескольких событий MIDI, каждое из которых определяется структурой [**мидиевент**](/windows/win32/api/mmeapi/ns-mmeapi-midievent) . Приложение управляет буфером путем вызова функций обработки потока, таких как [**мидистреамопен**](/windows/win32/api/mmeapi/nf-mmeapi-midistreamopen), [**мидистреамаут**](/windows/win32/api/mmeapi/nf-mmeapi-midistreamout)и [**мидистреамклосе**](/windows/win32/api/mmeapi/nf-mmeapi-midistreamclose).

-   [Формат буфера потока](stream-buffer-format.md)
-   [Сведения о времени](timing-information.md)
-   [Типы событий MIDI](midi-event-types.md)
-   [Потоки MIDI](midi-streams.md)

 

 