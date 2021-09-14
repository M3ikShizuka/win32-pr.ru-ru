---
description: Показывает, как использовать Microsoft Media Foundation для декодирования звука из файла мультимедиа.
ms.assetid: 29822e6b-8598-4133-b181-7fb0854553b7
title: Пример аудиоклипа
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 9c0e4a3e515d08e2cafd2ab2ba451a528f3d5677
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127269395"
---
# <a name="audio-clip-sample"></a>Пример аудиоклипа

Показывает, как использовать Microsoft Media Foundation для декодирования звука из файла мультимедиа.

Пример приложения для аудио-клипа считывает звуковые данные из файла мультимедиа и записывает несжатое аудио в ВОЛНовый файл.

## <a name="apis-demonstrated"></a>Продемонстрированные API

В этом образце демонстрируются следующие интерфейсы Media Foundation:

-   [**имфсаурцереадер**](/windows/desktop/api/mfreadwrite/nn-mfreadwrite-imfsourcereader)

## <a name="usage"></a>Использование

Этот пример представляет собой приложение командной строки. Он использует следующие аргументы командной строки:

``` syntax
audioclip.exe inputfile outputfile.wav
```

-   inputFile: имя файла, содержащего аудиопоток.
-   выходной_файл. WAV: Имя записываемого файла звукозаписи.

## <a name="requirements"></a>Требования



| Продукт                                                        | Version   |
|----------------------------------------------------------------|-----------|
| [Windows SDK](https://msdn.microsoft.com/windowsvista/bb980924.aspx) | Windows 7 |



 

## <a name="downloading-the-sample"></a>Загрузка образца

этот пример доступен в [репозитории github для классических примеров Windows](https://github.com/Microsoft/Windows-classic-samples/tree/master/Samples/Win7Samples/multimedia/mediafoundation/AudioClip).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Примеры пакетов SDK Media Foundation](media-foundation-sdk-samples.md)
</dt> <dt>

[Модуль чтения исходного кода](source-reader.md)
</dt> <dt>

[Учебник. декодирование аудио](tutorial--decoding-audio.md)
</dt> </dl>

 

 



