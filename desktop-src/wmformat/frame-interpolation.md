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
ms.openlocfilehash: 5c62f95322920576eec0f10f3e4d61a279fdc4cf
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127267123"
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

 

 




