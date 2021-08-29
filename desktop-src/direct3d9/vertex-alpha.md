---
description: В данных вершин можно указать альфа-данные. Чтобы включить вершинную альфа-версию, задайте для параметра D3DRS \_ диффусематериалсаурце \_ значение D3DMCS COLOR1, чтобы среда выполнения Direct3D воспользулись рассеянным значением из рассеянного цвета, а не из материала.
ms.assetid: 2b0d842d-ee7d-4633-846d-96697153adc7
title: Вершинная альфа-версия (Direct3D 9)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c2443b14d62698e342b7cbb9c4b79d30d3e11e32be76a3f584823ddf74b16685
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119984544"
---
# <a name="vertex-alpha-direct3d-9"></a>Вершинная альфа-версия (Direct3D 9)

В данных вершин можно указать альфа-данные. Чтобы включить вершинную альфа-версию, задайте для параметра D3DRS \_ диффусематериалсаурце \_ значение D3DMCS COLOR1, чтобы среда выполнения Direct3D воспользулись рассеянным значением из рассеянного цвета, а не из материала.


```
m_pd3dDevice->SetRenderState( D3DRS_DIFFUSEMATERIALSOURCE,  
                                D3DMCS_COLOR1 );
```



Затем укажите альфа-значения в рассеянном цвете. Функция Аддалфатоасфере добавляет альфа-канал в вершины сферы. Ниже приведен пример того, как предоставить функции сведения о альфа-составляющей.


```
AddAlphaToASphere( m_pObstacleVertices, 12,  
                    D3DRGBA(light.dcvDiffuse.r, light.dcvDiffuse.g, 
                            light.dcvDiffuse.b, vAlpha ));
```



Вот как выглядит функция.


```
 
void AddAlphaToASphere(D3DLVERTEX* pVertices, DWORD dwNumRings, D3DCOLOR lightcolor)
{
    WORD x, y;
    // rings around
    for( y=0; y < dwNumRings; y++ )
        for( x=0; x < (dwNumRings*2)+1; x++ )
            (pVertices++)->color = lightcolor;

    // top and bottom
    (pVertices++)->color = lightcolor;
    (pVertices++)->color = lightcolor;
}
```



Аддалфатоасфере просто изменяет элемент цвета каждой вершины, имеющей тип D3DLVERTEX, чтобы включить альфа-информацию.

D3DLVERTEX выглядит следующим образом.


```
 
// Lit vertex
typedef struct {
    D3DVALUE x, y, z;
    DWORD dwReserved;
    D3DCOLOR color, specular;
    D3DVALUE tu, tv;
} D3DLVERTEX, *LPD3DLVERTEX;
```



Рисование сферы,


```
#define D3DFVF_LVERTEX ( D3DFVF_XYZ | D3DFVF_DIFFUSE | D3DFVF_SPECULAR | \
                        D3DFVF_TEX0 )

//...

// Draw the lit sphere
m_pd3dDevice->DrawIndexedPrimitive( D3DPT_TRIANGLELIST, D3DFVF_LVERTEX,
                                    m_pObstacleVertices, m_dwNumObstacleVertices,
                                    m_pObstacleIndices,  m_dwNumObstacleIndices, 0 );
```



приводит к прозрачной сфере с использованием вершин альфа.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Альфа-смешение](alpha-blending.md)
</dt> </dl>

 

 



