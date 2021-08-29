---
title: Интерполяция кадров
description: Интерполяция кадров
ms.assetid: 74dbe855-361c-42ba-b21b-322ccd1c91d0
keywords:
- Windows Пакет SDK для формата мультимедиа, интерполяция кадров
- кодеки, интерполяция кадров
- Интерполяция кадров
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 9b10691bd2a1f3e6257810efd1e243d099cd4cfa85f0b2522369786602792614
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120007014"
---
# <a name="frame-interpolation"></a>Интерполяция кадров

Интерполяция кадров — это процесс создания промежуточных видеокадров на основе данных в двух последовательных кадрах закодированного видео. Фактически интерполяция кадров увеличивает [*частоту кадров*](wmformat-glossary.md) закодированного видео во время декодирования. Интерполяцию кадров можно использовать для повышения гладкости воспроизведения видеопотоков с низкой частотой кадров.

Поскольку это функция декодирования, она не включает специальные параметры кодирования и не требует дополнительной нагрузки на содержимое. Интерполяция кадров указывается в качестве выходного параметра в объекте Reader.

только Windows кодек Media Video 9 поддерживает интерполяцию кадров.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Функции кодеков**](codec-features.md)
</dt> <dt>

[**IWMReaderAdvanced2:: Сетаутпутсеттинг**](/previous-versions/windows/desktop/api/Wmsdkidl/nf-wmsdkidl-iwmreaderadvanced2-setoutputsetting)
</dt> <dt>

[**Параметры вывода**](output-settings.md)
</dt> </dl>

 

 




