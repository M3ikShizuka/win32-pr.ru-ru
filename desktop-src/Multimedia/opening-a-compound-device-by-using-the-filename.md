---
title: Открытие составного устройства с помощью имени файла
description: Открытие составного устройства с помощью имени файла
ms.assetid: 5199bb68-44be-4fad-af5b-8fe89f27caee
keywords:
- Функция МЦисендкомманд
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 20eb271658f77c5af4d35db96dd7bdbe6753af08
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371718"
---
# <a name="opening-a-compound-device-by-using-the-filename"></a>Открытие составного устройства с помощью имени файла

В следующем примере показано, как открыть устройство аудио-сигнала, указав звуковой файл с именем "ЛИТАВРЕ". WAV "с помощью функции [**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85)) .


```C++
UINT wDeviceID;
DWORD dwReturn;
MCI_OPEN_PARMS mciOpenParms;
 
// Opens a waveform-audio device by specifying the device and 
// file name.

mciOpenParms.lpstrDeviceType = "waveaudio";
mciOpenParms.lpstrElementName = "timpani.wav";

if (dwReturn = mciSendCommand(NULL, MCI_OPEN,
    MCI_OPEN_TYPE | MCI_OPEN_ELEMENT, (DWORD)(LPVOID) &mciOpenParms))
{
    
    // Error, unable to open device.
    
}

// The device opened successfully; get the device ID.
wDeviceID = mciOpenParms.wDeviceID;
```



 

 