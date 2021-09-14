---
description: 'В этом примере создается диаграмма предварительного просмотра видео с помощью метода ICaptureGraphBuilder2:: RenderStream в DirectShow.'
ms.assetid: 9b401de1-910a-41f7-bf80-dda73ee4a204
title: Предварительный просмотр видео (DirectShow)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 482fed2e164bbe867d848b05d417c89d0790256f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127254203"
---
# <a name="previewing-video-directshow"></a>Предварительный просмотр видео (DirectShow)

Чтобы создать диаграмму предварительного просмотра видео, вызовите метод [**ICaptureGraphBuilder2:: RenderStream**](/windows/desktop/api/Strmif/nf-strmif-icapturegraphbuilder2-renderstream) следующим образом:


```C++
ICaptureGraphBuilder2 *pBuild; // Capture Graph Builder
// Initialize pBuild (not shown).

IBaseFilter *pCap; // Video capture filter.

/* Initialize pCap and add it to the filter graph (not shown). */

hr = pBuild->RenderStream(&PIN_CATEGORY_PREVIEW, &MEDIATYPE_Video, 
    pCap, NULL, NULL);
```



В этом примере предполагается следующее:

-   *пбуилд* был инициализирован, как описано в [построителе Graph Capture](about-the-capture-graph-builder.md).
-   *ПКАП* был инициализирован путем создания экземпляра фильтра записи и его добавления в граф фильтра, как описано в разделе [Выбор устройства записи](selecting-a-capture-device.md).

Первый параметр метода [**ICaptureGraphBuilder2:: RenderStream**](/windows/desktop/api/Strmif/nf-strmif-icapturegraphbuilder2-renderstream) задает категорию закрепления. для предварительного просмотра диаграммы используйте **\_ \_ Предварительный просмотр категории закрепления**. Второй параметр указывает тип носителя, в качестве основного GUID типа. Для видео используйте **\_ Формат MEDIATYPE**. DV-устройства доставляют аудио и видео с чередованием, для которых используется тип носителя с **\_ чередованием**. (Дополнительные сведения о записи DV см. [в разделе Digital Video в DirectShow](digital-video-in-directshow.md).)

Третий параметр является указателем на интерфейс [**ибасефилтер**](/windows/desktop/api/Strmif/nn-strmif-ibasefilter) фильтра захвата. В этом примере следующие два параметра не требуются. Они используются для указания дополнительных фильтров, которые могут потребоваться для визуализации потока. установка последнего параметра в **значение NULL** приводит к тому, что построитель Graph отслеживания выбирает для потока модуль подготовки по умолчанию в зависимости от типа носителя. для видео Graph построитель записи всегда использует фильтр модуля [подготовки](video-renderer-filter.md) отчетов в качестве модуля подготовки отчетов по умолчанию.

> [!Note]  
> в Windows XP и более поздних версиях, хотя модуль подготовки видео (VMR) является модулем подготовки видео по умолчанию для методов [**играфбуилдер**](/windows/desktop/api/Strmif/nn-strmif-igraphbuilder) , он не является модулем подготовки отчетов по умолчанию для метода [**RenderStream**](/windows/desktop/api/Strmif/nf-strmif-icapturegraphbuilder2-renderstream) . на любой платформе Graph построитель записи всегда использует старый фильтр модуля подготовки отчетов, если не указано иное.

 

Хотя Категория PIN-кодов указана **как \_ \_ Предварительная версия категории ПИН**-кода, она не имеет значения, имеет ли фильтр предварительный ПИН-код, он может иметь ПИН-код видеопорта или просто ПИН-код захвата. в любом случае построитель Graph отслеживания автоматически создает правильный граф.

На следующей диаграмме показана самая простая диаграмма для предварительного просмотра видео.

![Диаграмма предварительного просмотра видео](images/vidcap01.png)

На этой схеме фильтр записи имеет предварительный ПИН-код для предварительного просмотра, который подключается непосредственно к модулю подготовки видео.

если фильтр записи имеет только пин-код записи, то построитель Graph записи добавляет фильтр [Smart Tee](smart-tee-filter.md) , который разделяет поток на поток записи и предварительный просмотр потока. Это описано более подробно в статье [объединение видеороликов и предварительной версии](combining-video-capture-and-preview.md).

в некоторых случаях поток видео должен проходить через наложение Mixer фильтр. Если это так, метод [**RenderStream**](/windows/desktop/api/Strmif/nf-strmif-icapturegraphbuilder2-renderstream) автоматически добавит его в граф.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Объединение видеозаписей и предварительной версии](combining-video-capture-and-preview.md)
</dt> <dt>

[Видеозапись](video-capture.md)
</dt> </dl>

 

 



