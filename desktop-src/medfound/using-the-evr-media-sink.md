---
description: Использование приемника мультимедиа Евр
ms.assetid: cd98266a-bc62-43da-b4d7-3561447d634f
title: Использование приемника мультимедиа Евр
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 84f8c666e88b495ad2d2e53fb1de10364f91636f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127579790"
---
# <a name="using-the-evr-media-sink"></a>Использование приемника мультимедиа Евр

Расширенный приемник мультимедиа модуля подготовки видео (Евр) можно использовать в качестве отдельного компонента. Тем не менее часто приложение создает приемник мультимедиа Евр в топологии, а затем использует сеанс мультимедиа для управления воспроизведением.

Существует два способа создания приемника мультимедиа Евр.

-   Функция [**мфкреатевидеорендерер**](/windows/desktop/api/evr/nc-evr-mfcreatevideorenderer) создает приемник мультимедиа.

-   Функция [**мфкреатевидеорендерерактивате**](/windows/desktop/api/mfidl/nf-mfidl-mfcreatevideorendereractivate) создает объект активации для приемника мультимедиа.

Приемник носителя Евр изначально имеет один приемник потока, который соответствует потоку ссылок. Чтобы добавить новые приемники потока, вызовите метод [**имфмедиасинк:: аддстреамсинк**](/windows/desktop/api/mfidl/nf-mfidl-imfmediasink-addstreamsink).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Улучшенный модуль подготовки видео](enhanced-video-renderer.md)
</dt> <dt>

[Приемники носителей](media-sinks.md)
</dt> </dl>

 

 



