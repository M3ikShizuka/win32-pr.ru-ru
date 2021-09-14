---
description: Фильтр модуля подготовки звука (звук)
ms.assetid: a3f2776b-974b-4886-82a3-38e00b607a07
title: Фильтр модуля подготовки звука (звук)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5d66d92357b41b6fa23018acf6d44b966eb77fab
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127162212"
---
# <a name="audio-renderer-waveout-filter"></a>Фильтр модуля подготовки звука (звук)

Этот фильтр использует \* API-интерфейс для вывода звуковых сигналов. Однако [Фильтр рендеринга DirectSound](directsound-renderer-filter.md) предоставляет те же функциональные возможности, что и DirectSound. по умолчанию фильтр Graph Manager использует модуль подготовки DirectSound вместо этого фильтра. Микширование звука отключено в модуле подготовки аудио, поэтому если во время воспроизведения необходимо смешивать несколько звуковых потоков, используйте модуль подготовки DirectSound.

Этот фильтр не проверяет подтип аудиопотока. Структура [**вавеформат**](/windows/win32/api/mmreg/ns-mmreg-waveformat) или [**вавеформатекс**](/previous-versions/dd757713(v=vs.85)) , переданная в формате, содержит сведения, необходимые для соединения.

Этот фильтр поддерживает ряд частот выборки, которые зависят от звукового драйвера.




| Метка | Значение |
|--------|-------|
| Интерфейсы фильтра | <ul><li><a href="/windows/desktop/api/Strmif/nn-strmif-iamaudiorendererstats"><strong>иамаудиорендерерстатс</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-iamclockslave"><strong>иамклоккславе</strong></a></li><li><a href="/previous-versions/windows/desktop/api/Amaudio/nn-amaudio-iamdirectsound"><strong>иамдиректсаунд</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-iamresourcecontrol"><strong>иамресаурцеконтрол</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-ibasefilter"><strong>ибасефилтер</strong></a></li><li><a href="/windows/desktop/api/Control/nn-control-ibasicaudio"><strong>ибасикаудио</strong></a></li><li><a href="/windows/desktop/api/Control/nn-control-imediaposition"><strong>имедиапоситион</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-imediaseeking"><strong>имедиасикинг</strong></a></li><li>IPersistPropertyBag</li><li>IPersistStream</li><li><a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"><strong>икуалитиконтрол</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-ireferenceclock"><strong>иреференцеклокк</strong></a></li></ul> | 
| Типы носителей входных закрепления | <strong>MEDIATYPE_Audio</strong> | 
| Интерфейсы входных закрепления | <ul><li><a href="/windows/desktop/api/Strmif/nn-strmif-imeminputpin"><strong>имеминпутпин</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>ипин</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"><strong>икуалитиконтрол</strong></a></li></ul> | 
| Типы носителей для выходного ПИН-кода | Неприменимо. | 
| Интерфейсы выходного ПИН-кода | Неприменимо. | 
| Фильтровать CLSID | <strong>CLSID_AudioRender</strong> | 
| CLSID страницы свойств | <strong>CLSID_AudioProperties</strong>, <strong>CLSID_AudioRendererAdvancedProperties</strong> | 
| Исполняемый объект | quartz.dll | 
| <a href="merit.md">Заслуживают</a> | <strong>MERIT_DO_NOT_USE</strong> | 
| <a href="filter-categories.md">Категория фильтра</a> | <strong>CLSID_AudioRendererCategory</strong> | 




 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[DirectShow Фильтрующ](directshow-filters.md)
</dt> </dl>

 

 
