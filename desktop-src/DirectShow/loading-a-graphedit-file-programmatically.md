---
description: Программная загрузка файла Графедит
ms.assetid: 0e1cff4e-43f8-4d0a-b7a7-b6d0278e9e4a
title: Программная загрузка файла Графедит
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a9a4780ead7b65d883bdd48917c6372425612435
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127055456"
---
# <a name="loading-a-graphedit-file-programmatically"></a>Программная загрузка файла Графедит

Приложение может использовать интерфейс **IPersistStream** для загрузки файла графедит (. ГРФ). Используйте следующий код:


```C++
HRESULT LoadGraphFile(IGraphBuilder *pGraph, const WCHAR* wszName)
{
    IStorage *pStorage = 0;
    if (S_OK != StgIsStorageFile(wszName))
    {
        return E_FAIL;
    }
    HRESULT hr = StgOpenStorage(wszName, 0, 
        STGM_TRANSACTED | STGM_READ | STGM_SHARE_DENY_WRITE, 
        0, 0, &pStorage);
    if (FAILED(hr))
    {
        return hr;
    }
    IPersistStream *pPersistStream = 0;
    hr = pGraph->QueryInterface(IID_IPersistStream,
             reinterpret_cast<void**>(&pPersistStream));
    if (SUCCEEDED(hr))
    {
        IStream *pStream = 0;
        hr = pStorage->OpenStream(L"ActiveMovieGraph", 0, 
            STGM_READ | STGM_SHARE_EXCLUSIVE, 0, &pStream);
        if(SUCCEEDED(hr))
        {
            hr = pPersistStream->Load(pStream);
            pStream->Release();
        }
        pPersistStream->Release();
    }
    pStorage->Release();
    return hr;
}

```



> [!Note]  
> вызов **IPersistStream:: Load** в предыдущем примере кода может вернуть DirectShow ошибку или код успешного выполнения. Список возможных возвращаемых значений см. в разделе [коды ошибок и успешности](error-and-success-codes.md).

 

Файлы Графедит предназначены только для тестирования и отладки. Они не предназначены для использования приложениями конечных пользователей.

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[имитация Graph сборки с помощью графедит](simulating-graph-building-with-graphedit.md)
</dt> <dt>

[**стгиссторажефиле**](/windows/win32/api/coml2api/nf-coml2api-stgisstoragefile)
</dt> <dt>

[**стгопенстораже**](/windows/win32/api/coml2api/nf-coml2api-stgopenstorage)
</dt> </dl>

 

 
