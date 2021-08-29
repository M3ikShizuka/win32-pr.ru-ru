---
description: запись Windowsного файла мультимедиа в DES
ms.assetid: 741ebcbc-62fb-4c7f-845f-a361f5b63f8c
title: запись Windowsного файла мультимедиа в DES
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d05b954ae6046bb61027bd3e7f63bcd2fcaafa35020bc0a8a1bed278b99731ea
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119650494"
---
# <a name="writing-a-windows-media-file-in-des"></a>запись Windowsного файла мультимедиа в DES

\[Этот API не поддерживается и может быть изменен или недоступен в будущем.\]

в этом разделе описано, как записать Windows файл мультимедиа с помощью [служб DirectShow editing Services](directshow-editing-services.md) (DES).

> [!IMPORTANT]
> не используйте модуль интеллектуального просмотра для записи Windows файлов мультимедиа. Всегда используйте базовый механизм визуализации (CLSID \_ рендеренгине).

 

чтобы записать Windows файл мультимедиа, выполните следующие действия.

1.  Вызовите **SetSite** в подсистеме визуализации, указав указатель на поставщика ключа.
2.  Создание внешнего интерфейса графа. (См. раздел [Подготовка к просмотру Project](rendering-a-project.md).)
3.  Создайте фильтр [модуля записи WM ASF](wm-asf-writer-filter.md) и добавьте его в граф.
4.  Чтобы задать имя файла, используйте интерфейс [**ифилесинкфилтер**](/windows/desktop/api/Strmif/nn-strmif-ifilesinkfilter) в фильтре модуля записи WM ASF.
5.  настройка модуля записи WM ASF для использования Windowsного профиля носителя. Каждый профиль имеет предопределенное количество потоков. Необходимо выбрать профиль, соответствующий группам в проекте.

    Интерфейс [**иконфигасфвритер**](/previous-versions/windows/desktop/api/Dshowasf/nn-dshowasf-iconfigasfwriter) содержит несколько различных методов настройки профиля. Например, метод **конфигурефилтерусингпрофилегуид** указывает системный профиль в виде идентификатора GUID. или можно использовать Windows методы формата мультимедиа, чтобы получить указатель **ивмпрофиле** , а затем вызвать [**иконфигасфвритер:: конфигурефилтерусингпрофиле**](/previous-versions/windows/desktop/api/Dshowasf/nf-dshowasf-iconfigasfwriter-configurefilterusingprofile). Дополнительные сведения см. [в разделе Настройка модуля записи ASF](configuring-the-asf-writer.md).

6.  Подключение внешний интерфейс в модуль записи ASF. Внешний интерфейс графа содержит один выходной ПИН-код для каждой группы. Если вы указали совместимый профиль, модуль записи ASF должен иметь соответствующий набор входных ПИН-кодов. Подключение каждый выходной закрепление в соответствующий входной пин-код. Проще всего это сделать с помощью метода [**ICaptureGraphBuilder2:: RenderStream**](/windows/desktop/api/Strmif/nf-strmif-icapturegraphbuilder2-renderstream) . сначала создайте новый экземпляр [построителя Graph Capture](capture-graph-builder.md) и инициализируйте его с помощью указателя на фильтр Graph Manager:

    ```C++
    ICaptureGraphBuilder2 *pBuild = 0;
    hr = CoCreateInstance(CLSID_CaptureGraphBuilder2, 0, CLSCTX_INPROC_SERVER,
        IID_ICaptureGraphBuilder2, (void**)&pBuild);
    pBuild->SetFiltergraph(pGraph); 
    ```

    

    Затем извлеките выходной ПИН-код для каждой группы, вызвав метод [**ирендеренгине:: жетграупаутпутпин**](irenderengine-getgroupoutputpin.md) . Вызовите **RenderStream** , чтобы подключить ПИН-код к модулю записи ASF:

    ```C++
    long cGroups = 0;
    hr = pTimeline->GetGroupCount(&cGroups);
    for (long i = 0; i < cGroups; i++)
    {
        IPin *pPin;
        hr = pRenderEngine->GetGroupOutputPin(i, &pPin);
        if (SUCCEEDED(hr))
        {
            hr = pBuild->RenderStream(0, 0, pPin, 0, pASF);
        }
        pPin->Release();
    }
    pBuild->Release
    ```

    

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[использование Windows Media с DirectShow служб редактирования](using-windows-media-with-directshow-editing-services.md)
</dt> </dl>

 

 



