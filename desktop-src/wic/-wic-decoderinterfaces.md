---
description: Интерфейсы декодера
ms.assetid: b88517cc-06fe-4d83-a6a9-76e1f34293f4
title: Интерфейсы декодера
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ef90ca2dd521c15460295505a6d5b7ea451c4dba
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570322"
---
# <a name="decoder-interfaces"></a>Интерфейсы декодера

в следующих таблицах показаны интерфейсы, реализованные с помощью декодеров Windows imaging Component (WIC), а на схеме классов показана иерархия наследования.

Интерфейсы декодера Container-Level



| Интерфейс                                                                                       | Обязанности                             | Реализация                                                             |
|-------------------------------------------------------------------------------------------------|----------------------------------------------|----------------------------------------------------------------------------|
| [ивикбитмапдекодер](-wic-imp-iwicbitmapdecoder.md)                                             | Службы уровня контейнера                     | Обязательно                                                                   |
| [ивикбитмапкодекпрогресснотификатион](-wic-imp-iwicbitmapcodecprogressnotification-decoder.md) | Уведомление о ходе выполнения & поддержка отмены | Рекомендуется                                                                |
| [ивикметадатаблоккреадер](-wic-imp-iwicmetadatablockreader.md)                                 | Перечисление метаданных                         | Необязательный (требуется только для форматов, поддерживающих метаданные уровня контейнера) |



 

Интерфейсы декодера Frame-Level



| Интерфейс                                                           | Обязанности          | Реализация                |
|---------------------------------------------------------------------|---------------------------|-------------------------------|
| [IWICBitmapFrameDecode](-wic-imp-iwicbitmapframedecode.md)         | Службы уровня кадров      | Обязательно                      |
| [ивикметадатаблоккреадер](-wic-imp-iwicmetadatablockreader.md)     | Перечисление метаданных      | Обязательно                      |
| [ивикбитмапсаурцетрансформ](-wic-imp-iwicbitmapsourcetransform.md) | Встроенные преобразования декодера | Рекомендуется                   |
| [ивикдевелоправ](-wic-imp-iwicdevelopraw.md)                       | Службы обработки RAW   | Требуется только для необработанных форматов |



 

![Иерархия наследования интерфейса WIC](graphics/wicinterfaces.png)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

**Основные понятия**
</dt> <dt>

[Реализация декодера WIC-Enabled](-wic-implementingwicdecoder.md)
</dt> <dt>

[Реализация Ивикбитмапдекодер](-wic-imp-iwicbitmapdecoder.md)
</dt> <dt>

[Написание WIC-Enabled КОДЕка](-wic-howtowriteacodec.md)
</dt> <dt>

[Windows Общие сведения о компонентах обработки изображений](-wic-about-windows-imaging-codec.md)
</dt> </dl>

 

 



