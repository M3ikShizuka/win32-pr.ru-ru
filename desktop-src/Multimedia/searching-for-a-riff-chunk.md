---
title: Поиск фрагмента Metallica
description: Поиск фрагмента Metallica
ms.assetid: ce974fb3-3af0-4400-8f55-65d63627592a
keywords:
- файловый ввод-вывод для мультимедиа, Поиск фрагмента Metallica
- Ввод-вывод файлов, Поиск фрагмента Metallica
- входные и выходные данные (ввод-вывод), Поиск фрагмента Metallica
- Ввод-вывод (входные и выходные данные), Поиск фрагмента Metallica
- Поиск фрагмента Metallica
- формат файла обмена ресурсами (Metallica)
- Metallica (формат файла обмена ресурсами)
- ВВОД-ВЫВОД METALLICA
- Фрагмент Metallica
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 9b45b2182e44ac84423c29a79fe29e96820d5bf2
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371826"
---
# <a name="searching-for-a-riff-chunk"></a>Поиск фрагмента Metallica

В следующем примере функция [**ммиодесценд**](/windows/win32/api/mmiscapi/nf-mmiscapi-mmiodescend) используется для поиска фрагмента "Metallica" с типом формы "Wave", чтобы убедиться, что файл, который только что открыт, является файлом аудио-файла.


```C++
HMMIO    hmmio; 
MMCKINFO mmckinfoParent; 
MMCKINFO mmckinfoSubchunk; 
. 
. 
. 
// Locate a "RIFF" chunk with a "WAVE" form type to make 
// sure the file is a waveform-audio file. 
mmckinfoParent.fccType = mmioFOURCC('W', 'A', 'V', 'E'); 
if (mmioDescend(hmmio, (LPMMCKINFO) &mmckinfoParent, NULL, 
    MMIO_FINDRIFF)) 
    // The file is not a waveform-audio file. 
else 
    // The file is a waveform-audio file 

```



 

 