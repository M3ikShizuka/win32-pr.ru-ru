---
description: Проверка поддерживаемых форматов ДКСВА-HD
ms.assetid: 43ae9f70-34a1-48ca-be61-e974e2daebd7
title: Проверка поддерживаемых форматов ДКСВА-HD
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d07d47043ed200d256e2bef8fa2c9ab6717f3b82
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574986"
---
# <a name="checking-supported-dxva-hd-formats"></a>Проверка поддерживаемых форматов ДКСВА-HD

## <a name="checking-supported-input-formats"></a>Проверка поддерживаемых форматов входных данных

Чтобы получить список форматов входных данных, поддерживаемых устройством Microsoft DirectX Video ускорение High Definition (ДКСВА-HD), выполните следующие действия.

1.  Вызовите [**идксвахд \_ Device:: жетвидеопроцессордевицекапс**](/windows/desktop/api/dxvahd/nf-dxvahd-idxvahd_device-getvideoprocessordevicecaps) , чтобы получить возможности устройства.
2.  Проверьте элемент **инпутформаткаунт** структуры [**дксвахд \_ впдевкапс**](/windows/desktop/api/dxvahd/ns-dxvahd-dxvahd_vpdevcaps) . Этот член предоставляет количество поддерживаемых входных форматов.
3.  Выделите массив значений **D3DFORMAT** размером **инпутформаткаунт**.
4.  Передайте этот массив в метод [**идксвахд \_ устройства:: жетвидеопроцессоринпутформатс**](/windows/desktop/api/dxvahd/nf-dxvahd-idxvahd_device-getvideoprocessorinputformats) . Методы заполняют массив списком входных форматов.

Следующий код показывает эти действия.


```C++
// Checks whether a DXVA-HD device supports a specified input format.

HRESULT CheckInputFormatSupport(
    IDXVAHD_Device          *pDXVAHD,
    const DXVAHD_VPDEVCAPS& caps,
    D3DFORMAT               d3dformat
    )
{
    D3DFORMAT *pFormats = new (std::nothrow) D3DFORMAT[ caps.InputFormatCount ];
    if (pFormats == NULL)
    {
        return E_OUTOFMEMORY;
    }

    HRESULT hr = pDXVAHD->GetVideoProcessorInputFormats(
        caps.InputFormatCount, 
        pFormats
        );

    if (FAILED(hr)) 
    { 
        goto done; 
    }

    UINT index;
    for (index = 0; index < caps.InputFormatCount; index++)
    {
        if (pFormats[index] == d3dformat)
        {
            break;
        }
    }
    if (index == caps.InputFormatCount)
    {
        hr = E_FAIL;
    }

done:
    delete [] pFormats;
    return hr;
}
```



## <a name="checking-supported-output-formats"></a>Проверка поддерживаемых форматов выходных данных

Чтобы получить список форматов вывода, поддерживаемых устройством ДКСВА-HD, выполните следующие действия.

1.  Вызовите [**идксвахд \_ Device:: жетвидеопроцессордевицекапс**](/windows/desktop/api/dxvahd/nf-dxvahd-idxvahd_device-getvideoprocessordevicecaps) , чтобы получить возможности устройства.
2.  Проверьте элемент **аутпутформаткаунт** структуры [**дксвахд \_ впдевкапс**](/windows/desktop/api/dxvahd/ns-dxvahd-dxvahd_vpdevcaps) . Этот член предоставляет количество поддерживаемых входных форматов.
3.  Выделите массив значений **D3DFORMAT** размером **аутпутформаткаунт**.
4.  Передайте этот массив в метод [**идксвахд \_ устройства:: жетвидеопроцессораутпутформатс**](/windows/desktop/api/dxvahd/nf-dxvahd-idxvahd_device-getvideoprocessoroutputformats) . Методы заполняют массив списком выходных форматов.

Следующий код показывает эти действия.


```C++
// Checks whether a DXVA-HD device supports a specified output format.

HRESULT CheckOutputFormatSupport(
    IDXVAHD_Device          *pDXVAHD,
    const DXVAHD_VPDEVCAPS& caps,
    D3DFORMAT               d3dformat
    )
{
    D3DFORMAT *pFormats = new (std::nothrow) D3DFORMAT[caps.OutputFormatCount];
    if (pFormats == NULL)
    {
        return E_OUTOFMEMORY;
    }

    HRESULT hr = pDXVAHD->GetVideoProcessorOutputFormats(
        caps.OutputFormatCount, 
        pFormats
        );

    if (FAILED(hr)) 
    { 
        goto done; 
    }

    UINT index;
    for (index = 0; index < caps.OutputFormatCount; index++)
    {
        if (pFormats[index] == d3dformat)
        {
            break;
        }
    }
    if (index == caps.OutputFormatCount)
    {
        hr = E_FAIL;
    }

done:
    delete [] pFormats;
    return hr;
}
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[ДКСВА-HD](dxva-hd.md)
</dt> </dl>

 

 



