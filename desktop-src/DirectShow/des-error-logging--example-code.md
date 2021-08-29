---
description: 'Ведение журнала ошибок DES: пример кода'
ms.assetid: e734daed-9230-4376-839f-7e09da7bc275
title: 'Ведение журнала ошибок DES: пример кода'
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2919e8214a247be77c5d706bbbf5a043751791b26ecb59f95e2e1bc69ce9f070
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118952963"
---
# <a name="des-error-logging-example-code"></a>Ведение журнала ошибок DES: пример кода

\[Этот API не поддерживается и может быть изменен или недоступен в будущем.\]

в следующем примере кода представлено полноценное консольное приложение, которое загружает и предварительно просматривает файл XML-проекта [служб DirectShow editing Services](directshow-editing-services.md) , используя класс ведения журнала ошибок, описанный в этом разделе. (См. раздел [ошибки ведения журнала](logging-errors.md).) Имя файла проекта жестко закодировано в приложении.

Чтобы сделать код короче, консольное приложение использует интеллектуальные указатели ATL, что устраняет необходимость вызывать **QueryInterface** и **Release**. При желании можно изменить образец приложения при [загрузке и предварительном просмотре Project](loading-and-previewing-a-project.md). Просто добавьте код, показанный в предыдущем разделе.


```C++
#include <atlbase.h>
#include <dshow.h>
#include <qedit.h>
#include <stdio.h>

// Declare error logging class.
class CErrReporter;

// (The implementation of CErrReporter was given previously.)

void __cdecl main(void)
{
    HRESULT hr = CoInitialize(NULL);

    if (FAILED(hr))
    {
        // Error handling is omitted for clarity.
    }

    { // Scope for smart pointers.

    CComPtr<IAMTimeline>   pTL;
    CComPtr<IRenderEngine> pRenderEngine; 
    CComPtr<IXml2Dex>      pXML; 
    CComPtr<IGraphBuilder> pGraph;

    hr = CoCreateInstance(CLSID_AMTimeline, NULL, CLSCTX_INPROC_SERVER, 
                IID_IAMTimeline, (void**) &pTL);
    hr = CoCreateInstance(CLSID_Xml2Dex, NULL, CLSCTX_INPROC_SERVER, 
                IID_IXml2Dex, (void**) &pXML);
    hr = CoCreateInstance(CLSID_RenderEngine, NULL, CLSCTX_INPROC_SERVER,
                IID_IRenderEngine, (void**) &pRenderEngine);

    // Set the error log.
    CComQIPtr<IAMSetErrorLog, &IID_IAMSetErrorLog> pSetLog(pTL);
    if (pSetLog)
    {
        IAMErrorLog *pLog = new CErrReporter;    
        pSetLog->put_ErrorLog(pLog);
    }
   
    // Load and preview the project.
    CComBSTR bstrFile(OLESTR("C:\\example.xtl"));
    hr = pXML->ReadXMLFile(pTL, bstrFile); 
    if (SUCCEEDED(hr))
    {
        hr = pRenderEngine->SetTimelineObject(pTL);
        hr = pRenderEngine->ConnectFrontEnd( );
        hr = pRenderEngine->RenderOutputPins( );
        hr = pRenderEngine->GetFilterGraph(&pGraph);

        CComQIPtr<IMediaControl, &IID_IMediaControl> pControl(pGraph);
        CComQIPtr<IMediaEvent, &IID_IMediaEvent> pEvent(pGraph);
        pControl->Run();

        long evCode;
        hr = pEvent->WaitForCompletion(INFINITE, &evCode);
        pControl->Stop();
    }
    // Clean up.
    pRenderEngine->ScrapIt();
    }
    CoUninitialize();
}
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Регистрация ошибок](logging-errors.md)
</dt> </dl>

 

 



