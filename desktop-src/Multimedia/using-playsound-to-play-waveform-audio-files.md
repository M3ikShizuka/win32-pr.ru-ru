---
title: Использование функции PlaySound для воспроизведения Waveform-Audio файлов
description: Использование функции PlaySound для воспроизведения Waveform-Audio файлов
ms.assetid: 8b7d191b-6b0c-4dff-84de-cb3a5c314b80
keywords:
- волна Audio, функция PlaySound
- звуковая волна, воспроизведение файлов
- звуковая волна, расширение имени файла WAV
- Функция PlaySound, воспроизведение аудио-файлов
- Воспроизведение аудио-файлов, функция PlaySound
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b9d5dde46827b7892217f760c749e75e19f368f5
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124372498"
---
# <a name="using-playsound-to-play-waveform-audio-files"></a>Использование функции PlaySound для воспроизведения Waveform-Audio файлов

В большинстве звуковых файлов с аудио-файлами используется. Расширение имени файла WAV.

Следующая инструкция воспроизводит сигналы C: \\ Sounds \\ . WAV файл:


```C++
PlaySound("C:\\SOUNDS\\BELLS.WAV", NULL, SND_SYNC); 
```



Если указанный файл не существует или файл не умещается в доступную память, то [**PlaySound**](/previous-versions//dd743680(v=vs.85)) воспроизводит системный звук по умолчанию. Если системный звук по умолчанию не определен, **PlaySound** завершается сбоем без какого бы то ни было звука. Если вы не хотите воспроизводить системный звук по умолчанию, укажите флаг "SND" \_ по умолчанию, как показано в следующем примере:


```C++
PlaySound("C:\\SOUNDS\\BELLS.WAV", NULL, SND_SYNC | SND_NODEFAULT); 
```



 

 