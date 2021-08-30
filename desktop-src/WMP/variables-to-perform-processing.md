---
title: Переменные для выполнения обработки
description: Переменные для выполнения обработки
ms.assetid: 02f194ea-cac0-410f-886f-2894dd6971c8
keywords:
- проигрыватель Windows Media подключаемые модули, метод Echo sample допроцессаутпут
- подключаемые модули, метод Echo Sample Допроцессаутпут
- подключаемые модули обработки цифровых сигналов, метод Echo Sample Допроцессаутпут
- Подключаемые модули DSP, метод Echo Sample Допроцессаутпут
- Пример подключаемого модуля Echo DSP, метод Допроцессаутпут
- Пример подключаемого модуля Echo DSP, обработка переменных
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e2f856808c1e9a00602fe3d2fe03d4255fd79bcfeb44c2021f2434ea670706cf
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120001344"
---
# <a name="variables-to-perform-processing"></a>Переменные для выполнения обработки

Переменные члена для обработки буфера задержки с количеством **байтов** ; они представляют собой **байтовые** указатели и целое число, в котором хранится число байтов. Это идеальный вариант для обработки 8-разрядного звука, так как 8-разрядный пример хорошо помещается в один байт памяти. Однако при обработке 16-разрядного звука удобнее преобразовать их в **короткие** указатели, поэтому обработка может происходить по два байта за раз.

Следующий пример кода выделяет новые 16-разрядные указатели и добавляет переменную указателя, в которой хранится адрес конца буфера задержки. Вставьте его в раздел "Case 16" непосредственно перед точкой входа цикла:


```C++
// Store local pointers to the delay buffer.
short    *pwDelayPointer = (short *)m_pbDelayPointer;
short    *pwDelayBuffer = (short *) m_pbDelayBuffer;
// Store the address of the last word of the delay buffer.
short    *pwEOFDelayBuffer = (short *)(m_pbDelayBuffer + m_cbDelayBuffer - sizeof(short)); 

```



Код для 8-разрядной обработки также выделяет переменную, в которой хранится адрес конца буфера задержки. Сохранение этого значения позволяет легко проверить, достигнут ли перемещаемый указатель буфера задержки на конец буфера задержки. В следующем примере кода вычисляется значение:


```C++
// Store the address of the end of the delay buffer.
BYTE * pbEOFDelayBuffer = (m_pbDelayBuffer + m_cbDelayBuffer - sizeof(BYTE));

```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Реализация Цечо::D Опроцессаутпут**](implementing-cecho--doprocessoutput.md)
</dt> </dl>

 

 




