---
title: Удаление кода для обработки более чем 16 бит
description: Удаление кода для обработки более чем 16 бит
ms.assetid: 90c165e1-bc77-42a5-878d-056762c62991
keywords:
- проигрыватель Windows Media подключаемые модули, метод Echo sample допроцессаутпут
- подключаемые модули, метод Echo Sample Допроцессаутпут
- подключаемые модули обработки цифровых сигналов, метод Echo Sample Допроцессаутпут
- Подключаемые модули DSP, метод Echo Sample Допроцессаутпут
- Пример подключаемого модуля Echo DSP, метод Допроцессаутпут
- Пример подключаемого модуля Echo DSP с обработкой более 16 бит
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ec33332ee332d0ca7b615844ba8ad5cd7b00eb2f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064368"
---
# <a name="removing-the-code-to-process-greater-than-16-bits"></a>Удаление кода для обработки более чем 16 бит

поскольку в этом образце обрабатывается только 8-разрядный или 16-разрядный звук, необходимо изменить код в **цечо:: валидатемедиатипе** , чтобы возвращался \_ тип DMO E \_ \_ не \_ принят для типов мультимедиа, превышающих 16 бит. Для этого необходимо изменить код в блоке switch, который проверяет форматы типа "волна" в \_ \_ расширяемом формате. Замените код мастера следующим кодом:


```C++
case WAVE_FORMAT_EXTENSIBLE:
    {
         // Sample size is greater than 16-bit or is multichannel.
        WAVEFORMATEXTENSIBLE *pWaveXT = (WAVEFORMATEXTENSIBLE *) pWave;

        if (KSDATAFORMAT_SUBTYPE_PCM != pWaveXT->SubFormat)
        {
            return DMO_E_TYPE_NOT_ACCEPTED;
        }
    }
    break;

```



Затем удалите или закомментируйте разделы кода в **допроцессаутпут** , которые обрабатывали аудио с высоким битом разрешения. Ниже приведены разделы, которые начинаются с варианта 24 и регистра 32.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Реализация Цечо::D Опроцессаутпут**](implementing-cecho--doprocessoutput.md)
</dt> </dl>

 

 




