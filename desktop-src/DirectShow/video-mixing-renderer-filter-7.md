---
description: Фильтр визуализации 7 для микширования видео
ms.assetid: c83e6c50-76f2-4aeb-944b-5b244c6bf776
title: Фильтр визуализации 7 для микширования видео
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 988af74dc2e4abac06215f283a496bb719384891
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127272947"
---
# <a name="video-mixing-renderer-filter-7"></a>Фильтр визуализации 7 для микширования видео

этот раздел относится к Windows XP и более поздних версий.

в Windows XP и более поздних версиях модуль подготовки видео (VMR-7) является модулем обработки видео по умолчанию. Он называется VMR-7, так как на внутреннем уровне используется DirectDraw 7. В DirectX 9 аналогичный, но отдельный фильтр VMR-9 доступен для распространения в системах, не использующих XP. VMR-9 использует Direct3D 9.

> [!Note]  
> фильтр VMR доступен в Windows XP и более поздних версиях. Он недоступен через распространяемый пакет DirectX или в предыдущих версиях Windows. В большинстве случаев приложения должны использовать [устройство микширования видео 9](video-mixing-renderer-filter-9.md).

 

К свойствам VMR относятся:

-   True альфа-смешение до 16 входных потоков
-   Доступ к составному изображению до его подготовки к просмотру
-   Модель подключаемых модулей, которая позволяет сторонним разработчикам реализовать пользовательские видеоэффекты.
-   Поддержка до 15 мониторов.

во время построения графа на Windows XP и более поздних версиях диспетчер Graph фильтров не будет использовать старый модуль подготовки отчетов или наложение Mixer фильтры, если только приложение не создаст их и не добавит их в граф.

Дополнительные сведения см. [в разделе Использование модуля подготовки видео для микширования](using-the-video-mixing-renderer.md).




| Метка | Значение |
|--------|-------|
| Интерфейсы фильтра | Все режимы:<ul><li><a href="/windows/desktop/api/Strmif/nn-strmif-iamcertifiedoutputprotection"><strong>иамцертифиедаутпутпротектион</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-iamfiltermiscflags"><strong>иамфилтермискфлагс</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-ibasefilter"><strong>ибасефилтер</strong></a></li><li><a href="ikspropertyset.md"><strong>икспропертисет</strong></a></li><li><a href="/windows/desktop/api/Control/nn-control-imediaposition"><strong>имедиапоситион</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-imediaseeking"><strong>имедиасикинг</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"><strong>икуалитиконтрол</strong></a></li><li><a href="/previous-versions/windows/desktop/api/Amvideo/nn-amvideo-iqualprop"><strong>икуалпроп</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-ivmraspectratiocontrol"><strong>ивмраспектратиоконтрол</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-ivmrdeinterlacecontrol"><strong>ивмрдеинтерлацеконтрол</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-ivmrfilterconfig"><strong>ивмрфилтерконфиг</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-ivmrmixerbitmap"><strong>ивмрмиксербитмап</strong></a></li></ul>Режим с окнами:<br /><ul><li><a href="/windows/desktop/api/Control/nn-control-ibasicvideo"><strong>ибасиквидео</strong></a></li><li><a href="/windows/desktop/api/Control/nn-control-ibasicvideo2"><strong>IBasicVideo2</strong></a></li><li><a href="/windows/desktop/api/Control/nn-control-ivideowindow"><strong>ивидеовиндов</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-ivmrmonitorconfig"><strong>ивмрмониторконфиг</strong></a></li></ul>Режим без окон:<br /><ul><li><a href="/windows/desktop/api/Strmif/nn-strmif-ivmrwindowlesscontrol"><strong>ивмрвиндовлессконтрол</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-ivmrmonitorconfig"><strong>ивмрмониторконфиг</strong></a></li></ul>Режим безрендеринга:<br /><ul><li><a href="/windows/desktop/api/Strmif/nn-strmif-ivmrsurfaceallocatornotify"><strong>ивмрсурфацеаллокаторнотифи</strong></a></li></ul>режим Mixer:<br /><ul><li><a href="/windows/desktop/api/Strmif/nn-strmif-ivmrmixercontrol"><strong>ивмрмиксерконтрол</strong></a></li></ul>Сведения о различных режимах VMR-7 см. в разделе <a href="vmr-modes-of-operation.md">режимы VMR в операции</a>.<br /> | 
| Типы носителей входных закрепления | Основной тип: MEDIATYPE_VideoSubtype: зависит от графического оборудования. Должно быть несжатым видео.<br /> | 
| Интерфейсы входных закрепления | <ul><li><a href="/previous-versions/windows/desktop/api/videoacc/nn-videoacc-iamvideoaccelerator"><strong>иамвидеоакцелератор</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-imeminputpin"><strong>имеминпутпин</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-ioverlay"><strong>Иоверлай</strong></a> (см. примечания)</li><li><a href="/windows/desktop/api/Strmif/nn-strmif-ipin"><strong>ипин</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-ipinconnection"><strong>ипинконнектион</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-iqualitycontrol"><strong>икуалитиконтрол</strong></a></li><li><a href="/windows/desktop/api/Strmif/nn-strmif-ivmrvideostreamcontrol"><strong>ивмрвидеостреамконтрол</strong></a></li></ul> | 
| Типы носителей для выходного ПИН-кода | Неприменимо. | 
| Интерфейсы выходного ПИН-кода | Неприменимо. | 
| Фильтровать CLSID | С этим фильтром связано два идентификатора CLSID:<ul><li>CLSID_VideoMixingRenderer: создает VMR-7. Если для создания VMR-7 недостаточно системных ресурсов, вызов <strong>CoCreateInstance</strong> завершается ошибкой.</li><li>CLSID_VideoRendererDefault: создает VMR-7, если доступны системные ресурсы, или, в противном случае, создает старый фильтр модуля <a href="video-renderer-filter.md">подготовки</a> отчетов.</li></ul>Используйте CLSID_VideoMixingRenderer, если требуются специальные возможности VMR-7. В противном случае используйте CLSID_VideoRendererDefault, который почти не может завершиться сбоем, так как он возвращается к старому фильтру модуля подготовки отчетов.<br /> | 
| CLSID страницы свойств | Неприменимо. | 
| Исполняемый объект | Quartz.dll | 
| <a href="merit.md">Заслуживают</a> | MERIT_PREFERRED + 1 | 
| <a href="filter-categories.md">Категория фильтра</a> | CLSID_LegacyAmFilterCategory | 




 

## <a name="remarks"></a>Комментарии

Закрепление ввода предоставляет интерфейс **иоверлай** только в том случае, если фильтр VMR-7 находится в оконном режиме. Единственным методом **иоверлай** , который реализует ПИН-код, является **жетвиндовхандле**, который позволяет приложению получить маркер окна видео фильтра. Все остальные методы **иоверлай** возвращают E \_ нотимпл. В режиме без окон фильтр не создает окно видео, поэтому ПИН-код не предоставляет интерфейс.

Приложение может предоставить пользовательский объект распределителя-Presenter, который предоставляет следующие интерфейсы:

-   [**ивмримажепресентер**](/windows/desktop/api/Strmif/nn-strmif-ivmrimagepresenter)
-   [**Ивмримажепресентерконфиг**](/windows/desktop/api/Strmif/nn-strmif-ivmrimagepresenterconfig) (необязательно)
-   [**Ивмрмониторконфиг**](/windows/desktop/api/Strmif/nn-strmif-ivmrmonitorconfig) (необязательно)
-   [**ивмрсурфацеаллокатор**](/windows/desktop/api/Strmif/nn-strmif-ivmrsurfaceallocator)
-   [**Ивмрвиндовлессконтрол**](/windows/desktop/api/Strmif/nn-strmif-ivmrwindowlesscontrol) (необязательно)

Дополнительные сведения о пользовательских распределительных выступающих см. [в разделе предоставление настраиваемого Allocator-Presenter для VMR-7](supplying-a-custom-allocator-presenter-for-vmr-7.md).

Приложение также может предоставить пользовательский компоновщик подключаемых модулей, который предоставляет следующий интерфейс:

-   [**ивмримажекомпоситор**](/windows/desktop/api/Strmif/nn-strmif-ivmrimagecompositor)

Чтобы настроить VMR с помощью пользовательского компоновщика, вызовите [**ивмрфилтерконфиг:: сетимажекомпоситор**](/windows/desktop/api/Strmif/nf-strmif-ivmrfilterconfig-setimagecompositor).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[DirectShow Фильтрующ](directshow-filters.md)
</dt> </dl>

 

 




