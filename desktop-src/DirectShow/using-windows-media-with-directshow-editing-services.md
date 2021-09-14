---
description: использование Windows Media с DirectShow служб редактирования
ms.assetid: 26a88197-ec80-4443-9d50-e11df40dd1eb
title: использование Windows Media с DirectShow служб редактирования
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 18fbfe715495834217b695f887305f1ecb21cb6f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127144882"
---
# <a name="using-windows-media-with-directshow-editing-services"></a>использование Windows Media с DirectShow служб редактирования

\[Этот API не поддерживается и может быть изменен или недоступен в будущем.\]

в этом разделе описывается использование Windows содержимого на основе носителя в приложении [DirectShow editing Services](directshow-editing-services.md) (DES). Существует два основных сценария.

-   Исходные клипы. проект DES может содержать аудио-и видеоклипы из Windows файлов мультимедиа.
-   Конечный формат. Windows Носитель — это идеальный формат для окончательных выходных данных проекта редактирования видео.

для работы с Windows файлами мультимедиа приложение должно предоставить сертификат программного обеспечения, который также называется ключом. Для этого реализуется объект поставщика ключа. Поставщик ключей — это COM-объект, предоставляющий интерфейс **IServiceProvider** . дополнительные сведения о реализации поставщика ключей см. [в разделе разблокировка пакета SDK для Windows Media Format](unlocking-the-windows-media-format-sdk.md).

чтобы использовать DES с Windows файлами мультимедиа, для следующих объектов des требуется программный ключ:

-   Модуль подготовки отчетов для предварительного просмотра или записи файлов.
-   Объект Медиадет для получения видеокадров или типов мультимедиа из файлов ASF.
-   \[! Существенно\]  
    > не используйте интеллектуальный модуль визуализации для чтения или записи Windows файлов мультимедиа. Всегда используйте базовый механизм визуализации (CLSID \_ рендеренгине).

     

Чтобы предоставить объекту программный ключ, запросите этот объект для интерфейса **IObjectWithSite** и вызовите **IObjectWithSite:: SetSite** с указателем на ваш поставщик ключей. Например, следующий код предоставляет программный ключ модулю визуализации:


```C++
// Create your key provider, using an application-defined function:
IServiceProvider *pKey;
hr = MyCreateKeyProviderFunction(&pKey);  

// Query the Render Engine for IObjectWithSite.
IObjectWithSite *pOWS;
hr = pRenderEngine->QueryInterface(__uuidof(IObjectWithSite), 
    reinterpret_cast<void**>(&pOWS));
if (SUCCEEDED(hr))
{
    // Give it your key provider.
    hr = pOWS->SetSite(pKey);
    pOWS->Release();
}
pKey->Release();
```



чтобы использовать Windows клипы источника мультимедиа в проекте DES, просто вызовите **IObjectWithSite:: SetSite** в подсистеме визуализации с указателем на ваш поставщик ключей.

сведения о записи Windows файлов мультимедиа см. [в разделе запись Windowsного файла мультимедиа в DES](writing-a-windows-media-file-in-des.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[использование служб DirectShow editing Services](using-directshow-editing-services.md)
</dt> </dl>

 

 



