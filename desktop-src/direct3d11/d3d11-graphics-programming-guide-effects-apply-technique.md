---
title: Применение методики (Direct3D 11)
description: Узнайте, как задать состояние воздействия на устройстве для Direct3D 11 после объявления и инициализации констант, текстур и состояния шейдера.
ms.assetid: 16001913-7ae2-4629-a625-eb850e29fc77
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 136d03f92957eaf1b3d501c0acd54aafde7e16d8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066433"
---
# <a name="apply-a-technique-direct3d-11"></a>Применение методики (Direct3D 11)

Когда константы, текстуры и состояние шейдера объявлены и инициализированы, осталось только установить состояние воздействия на устройстве.

## <a name="set-non-shader-state-in-the-device"></a>Задание состояния, отличного от шейдера, на устройстве

Некоторые состояния конвейера не задаются каким-либо действием. Например, очистка целевого объекта рендеринга готовит целевой объект отрисовки для данных. Ниже приведен пример очистки выходных буферов перед установкой состояния воздействия на устройство.


```
    // Clear the render target and depth stencil
    float ClearColor[4] = { 0.0f, 0.25f, 0.25f, 0.55f };
    ID3D11RenderTargetView* pRTV = DXUTGetD3D11RenderTargetView();
    pD3DDevice->ClearRenderTargetView( pRTV, ClearColor );
    ID3D11DepthStencilView* pDSV = DXUTGetD3D11DepthStencilView();
    pD3DDevice->ClearDepthStencilView( pDSV, D3D11_CLEAR_DEPTH, 1.0, 0 );
```



## <a name="set-effect-state-in-the-device"></a>Установка состояния воздействия на устройстве

Установка состояния действия выполняется путем применения состояния действия в цикле подготовки к просмотру. Это делается из внешней среды в. То есть выберите метод, а затем задайте состояние для каждого из проходов (в зависимости от желаемого результата).


```
    D3D11_TECHNIQUE_DESC techDesc;
    pRenderTechnique->GetDesc( &techDesc );
    for( UINT p = 0; p < techDesc.Passes; ++p )
    {
        }
            ....
            pRenderTechnique->GetPassByIndex( p )->Apply(0);
            pd3dDevice->DrawIndexed( (UINT)pSubset->IndexCount, 0,  
                 (UINT)pSubset->VertexStart );
        }
    }
```



Результат не отображает ничего, он просто устанавливает состояние воздействия на устройство. Код отрисовки вызывается после того, как состояние действия изменит состояние устройства. В этом примере вызов Дравиндексед выполняет отрисовку.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Отрисовка результата (Direct3D 11)](d3d11-graphics-programming-guide-effects-render.md)
</dt> </dl>

 

 




