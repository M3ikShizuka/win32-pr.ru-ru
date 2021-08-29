---
title: Создание шейдера домена
description: В этом разделе показано, как создать шейдер домена.
ms.assetid: 7d02fee4-2d7c-434b-86ab-e5ee615ae93b
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 40e76c581062460f7ec9d232e3594d88a4dd2bd4a346ccc30a373917671ffafa
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119566224"
---
# <a name="how-to-create-a-domain-shader"></a>Как создать Шейдер доменов

Шейдер доменов — это третий из трех этапов, которые работают вместе для реализации [тесселяции](direct3d-11-advanced-stages-tessellation.md). Входные данные для этапа доменного шейдера берутся из шейдера поверхности. В этом разделе показано, как создать шейдер домена.

Шейдер домена преобразует геометрию поверхности (созданную стадией тесселяции с фиксированной функцией) с помощью точек управления выходными данными шейдера поверхности, выходных данных исправления шейдеров поверхности-Constant Data и единого набора координат тесселяции UV.

**Создание шейдера домена**

1.  Создайте шейдер домена. См. раздел [как создать шейдер домена](direct3d-11-advanced-stages-domain-shader-design.md).
2.  Скомпилируйте код шейдера.
3.  Создайте объект шейдера домена с помощью [**ID3D11Device:: креатедомаиншадер**](/windows/desktop/api/D3D11/nf-d3d11-id3d11device-createdomainshader).
    ```
    HRESULT CreateDomainShader(
      const void *pShaderBytecode, // 
      SIZE_T BytecodeLength, // 
      ID3D11ClassLinkage *pClassLinkage, // 
      ID3D11DomainShader **ppDomainShader
    );
    ```

    

4.  Инициализируйте стадию конвейера с помощью [**ссылку ID3D11DeviceContext::D ссетшадер**](/windows/desktop/api/D3D11/nf-d3d11-id3d11devicecontext-dssetshader).
    ```
    void DSSetShader(
      ID3D11DomainShader *pDomainShader, // 
      ID3D11ClassInstance *const *ppClassInstances,
      UINT NumClassInstances
    );
    ```

    

При наличии привязки шейдера поверхности необходимо привязать шейдер домена к конвейеру. В частности, недопустимый прямой потоковая передача контрольных точек шейдера поверхности с помощью шейдера Geometry.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Использование Direct3D 11](how-to-use-direct3d-11.md)
</dt> <dt>

[Общие сведения об тесселяции](direct3d-11-advanced-stages-tessellation.md)
</dt> </dl>

 

 




