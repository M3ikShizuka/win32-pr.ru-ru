---
description: в этом разделе рассматриваются разработчики с рекомендациями по внедрению кодеков формата файлов изображений, которые будут работать в инфраструктуре Windowsного компонента обработки изображений (WIC).
ms.assetid: 58f03dc2-cc31-4d76-b75a-f332da1f900f
title: Написание WIC-Enabled кодека
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ee694d9a857781e97a31cb37f5ef18c518dae964
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127343475"
---
# <a name="how-to-write-a-wic-enabled-codec"></a>Написание WIC-Enabled кодека

в этом разделе рассматриваются разработчики с рекомендациями по внедрению кодеков формата файлов изображений, которые будут работать в инфраструктуре Windowsного компонента обработки изображений (WIC).

<dl>

[Введение](-wic-howtowriteacodec-intro.md)  
[принцип работы компонента обработки изображений Windows (WIC)](-wic-howwicworks.md)  
<dl>

[Обнаружение и арбитраж](-wic-howwicworks.md)  
[Декодирование](-wic-howwicworks.md)  
[Кодирование](-wic-howwicworks.md)  
[Время существования кодека](-wic-howwicworks.md)  
[Как WIC — включение кодека](-wic-howwicworks.md)  
[Поддержка многопоточных подразделений в WIC](-wic-howwicworks.md)  
</dl> </dd> <a href="-wic-implementingwicdecoder.md">Реализация декодера WIC-Enabled</a><dl>

[Интерфейсы декодера](-wic-decoderinterfaces.md)<dl>

[ивикбитмапдекодер](-wic-imp-iwicbitmapdecoder.md)  
[ивикбитмапкодекпрогресснотификатион](-wic-imp-iwicbitmapcodecprogressnotification-decoder.md)  
[IWICBitmapSource](-wic-imp-iwicbitmapsource.md)  
[IWICBitmapFrameDecode](-wic-imp-iwicbitmapframedecode.md)  
[ивикметадатаблоккреадер](-wic-imp-iwicmetadatablockreader.md)  
[ивикбитмапсаурцетрансформ](-wic-imp-iwicbitmapsourcetransform.md)  
[ивикдевелоправ](-wic-imp-iwicdevelopraw.md)  
</dl> </dd> </dl> </dd> <a href="-wic-implementingwicencoder.md">Реализация кодировщика WIC-Enabled</a>  
<dl>

[Интерфейсы кодировщика](-wic-encoderinterfaces.md)  
<dl>

[ивикбитмапенкодер](-wic-imp-iwicbitmapencoder.md)  
[ивикбитмапкодекпрогресснотификатион](-wic-imp-iwicbitmapcodecprogressnotification-encoder.md)  
[ивикбитмапфраминкоде](-wic-imp-iwicbitmapframeencode.md)  
[ивикметадатаблокквритер](-wic-imp-iwicmetadatablockwriter.md)  
</dl> </dd> </dl> </dd> <a href="-wic-codecinstallandreg.md">Установка и регистрация кодека</a>  
<dl>

[Регистрация кодека](-wic-codecinstallandreg.md)  
<dl>

[Общие записи регистров](-wic-generalregentries.md)  
[Записи реестра, относящиеся к кодировщику](-wic-encoderregentries.md)  
<dl>

[Регистрация формата контейнера с помощью модулей записи метаданных](-wic-encoderregentries.md)  
</dl> </dd> <a href="-wic-decoderregentries.md">Записи реестра, относящиеся к кодировщику</a>  
<dl>

[Регистрация нового формата контейнера с помощью средств чтения метаданных](-wic-decoderregentries.md)  
</dl> </dd> <a href="-wic-integrationregentries.md">интеграция с Windows Vista фотогаллери и проводником</a>  
<dl>

[Windows Хранилище свойств](-wic-integrationregentries.md)  
[Windows Галерея фотографий Vista](-wic-integrationregentries.md)  
[Windows Кэш эскизов Vista](-wic-integrationregentries.md)  
</dl> </dd> </dl> </dd> <a href="-wic-codecinstallandreg.md">Обновление кэша эскизов при установке кодека,</a> [делающей WIC-Enabled кодек, доступный для пользователей](-wic-codecinstallandreg.md) </dl> </dd> <a href="-wic-howtowriteacodec-conclusion.md"></a>  
</dl>

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

**Основные понятия**
</dt> <dt>

[Введение (написание WIC-Enabled КОДЕка)](-wic-howtowriteacodec-intro.md)
</dt> <dt>

[Windows Общие сведения о компонентах обработки изображений](-wic-about-windows-imaging-codec.md)
</dt> </dl>

 

 



