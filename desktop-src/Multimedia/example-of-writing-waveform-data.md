---
title: Пример записи данных волны
description: Пример записи данных волны
ms.assetid: 8078e5b4-340b-409a-88f9-143b02efebc1
keywords:
- звуковая волна, запись данных волны
- вспомогательный звук, запись данных волны
- запись данных волны
- Структура ВАВЕХДР
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f3ea78101c33ae7701bc30d70e55c788d826d5a4
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371316"
---
# <a name="example-of-writing-waveform-data"></a>Пример записи данных волны

В следующем примере показаны шаги, необходимые для выделения и настройки структуры [**вавехдр**](/windows/win32/api/mmeapi/ns-mmeapi-wavehdr) и записи блока данных на выходное устройство звуковой волны.


```C++
// Global variables. 

HANDLE hData  = NULL;  // handle of waveform data memory 
HPSTR  lpData = NULL;  // pointer to waveform data memory 
 
void WriteWaveData(void) 
{ 
    HWAVEOUT    hWaveOut; 
    HGLOBAL     hWaveHdr; 
    LPWAVEHDR   lpWaveHdr; 
    HMMIO       hmmio; 
    UINT        wResult; 
    HANDLE      hFormat; 
    WAVEFORMAT  *pFormat; 
    DWORD       dwDataSize; 

    // Open a waveform device for output using window callback. 

    if (waveOutOpen((LPHWAVEOUT)&hWaveOut, WAVE_MAPPER, 
                    (LPWAVEFORMAT)pFormat, 
                    (LONG)hwndApp, 0L, CALLBACK_WINDOW)) 
    { 
        MessageBox(hwndApp, 
                   "Failed to open waveform output device.", 
                   NULL, MB_OK | MB_ICONEXCLAMATION); 
        LocalUnlock(hFormat); 
        LocalFree(hFormat); 
        mmioClose(hmmio, 0); 
        return; 
    } 
 
    // Allocate and lock memory for the waveform data. 
 
    hData = GlobalAlloc(GMEM_MOVEABLE | GMEM_SHARE, dwDataSize ); 
    if (!hData) 
    { 
        MessageBox(hwndApp, "Out of memory.", 
                   NULL, MB_OK | MB_ICONEXCLAMATION); 
        mmioClose(hmmio, 0); 
        return; 
    } 
    if ((lpData = GlobalLock(hData)) == NULL) 
    { 
        MessageBox(hwndApp, "Failed to lock memory for data chunk.", 
                   NULL, MB_OK | MB_ICONEXCLAMATION); 
        GlobalFree(hData); 
        mmioClose(hmmio, 0); 
        return; 
    } 
 
    // Read the waveform data subchunk. 
 
    if(mmioRead(hmmio, (HPSTR) lpData, dwDataSize) != (LRESULT)dwDataSize) 
    { 
        MessageBox(hwndApp, "Failed to read data chunk.", 
                   NULL, MB_OK | MB_ICONEXCLAMATION); 
        GlobalUnlock(hData); 
        GlobalFree(hData); 
        mmioClose(hmmio, 0); 
        return; 
    } 
 
    // Allocate and lock memory for the header. 

    hWaveHdr = GlobalAlloc(GMEM_MOVEABLE | GMEM_SHARE, 
        (DWORD) sizeof(WAVEHDR)); 
    if (hWaveHdr == NULL) 
    { 
        GlobalUnlock(hData); 
        GlobalFree(hData); 
        MessageBox(hwndApp, "Not enough memory for header.", 
            NULL, MB_OK | MB_ICONEXCLAMATION); 
        return; 
    } 
 
    lpWaveHdr = (LPWAVEHDR) GlobalLock(hWaveHdr); 
    if (lpWaveHdr == NULL) 
    { 
        GlobalUnlock(hData); 
        GlobalFree(hData); 
        MessageBox(hwndApp, 
            "Failed to lock memory for header.", 
            NULL, MB_OK | MB_ICONEXCLAMATION); 
        return; 
    } 
 
    // After allocation, set up and prepare header. 
 
    lpWaveHdr->lpData = lpData; 
    lpWaveHdr->dwBufferLength = dwDataSize; 
    lpWaveHdr->dwFlags = 0L; 
    lpWaveHdr->dwLoops = 0L; 
    waveOutPrepareHeader(hWaveOut, lpWaveHdr, sizeof(WAVEHDR)); 
 
    // Now the data block can be sent to the output device. The 
    // waveOutWrite function returns immediately and waveform 
    // data is sent to the output device in the background. 
 
    wResult = waveOutWrite(hWaveOut, lpWaveHdr, sizeof(WAVEHDR)); 
    if (wResult != 0) 
    { 
        waveOutUnprepareHeader(hWaveOut, lpWaveHdr, 
                               sizeof(WAVEHDR)); 
        GlobalUnlock( hData); 
        GlobalFree(hData); 
        MessageBox(hwndApp, "Failed to write block to device", 
                   NULL, MB_OK | MB_ICONEXCLAMATION); 
        return; 
    } 
} 
```



 

 