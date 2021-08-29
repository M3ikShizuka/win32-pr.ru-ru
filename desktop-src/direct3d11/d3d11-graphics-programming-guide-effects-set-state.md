---
title: Установка состояния действия (Direct3D 11)
description: Некоторые константы эффектов необходимо инициализировать. См. базовый код для установки переменных эффектов в Direct3D 12.
ms.assetid: f94ba82e-fc67-4e4d-a49d-20e1163bdff7
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: dfa27e817299df9398bd6fa1752e636162d9b97f7b886a372b71c5d0845dff41
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119953084"
---
# <a name="set-effect-state-direct3d-11"></a>Установка состояния действия (Direct3D 11)

Некоторые константы эффектов необходимо инициализировать. После инициализации состояние воздействия устанавливается на устройство для всего цикла подготовки к просмотру. Другие переменные необходимо обновлять каждый раз при вызове цикла визуализации. Базовый код для установки переменных эффектов показан ниже для каждого типа переменных.

Действие инкапсулирует все состояние отрисовки, необходимое для выполнения этапа отрисовки. В терминах API существует три типа состояния, инкапсулированные в результате.

-   [Состояние константы](#constant-state)
-   [Состояние шейдера](#shader-state)
-   [Состояние текстуры](#texture-state)

## <a name="constant-state"></a>Состояние константы

Сначала объявите переменные в силе с помощью типов данных HLSL.


```
//--------------------------------------------------------------------------------------
// Global variables
//--------------------------------------------------------------------------------------
float4 g_MaterialAmbientColor;      // Material's ambient color
float4 g_MaterialDiffuseColor;      // Material's diffuse color
int g_nNumLights;

float3 g_LightDir[3];               // Light's direction in world space
float4 g_LightDiffuse[3];           // Light's diffuse color
float4 g_LightAmbient;              // Light's ambient color

Texture2D g_MeshTexture;            // Color texture for mesh

float    g_fTime;                   // App's time in seconds
float4x4 g_mWorld;                  // World matrix for object
float4x4 g_mWorldViewProjection;    // World * View * Projection matrix
```



Во вторых, объявите в приложении переменные, которые могут быть заданы приложением, а затем обновите переменные эффектов.


```
           
    D3DXMATRIX  mWorldViewProjection;
    D3DXVECTOR3 vLightDir[MAX_LIGHTS];
    D3DXVECTOR4 vLightDiffuse[MAX_LIGHTS];
    D3DXMATRIX  mWorld;
    D3DXMATRIX  mView;
    D3DXMATRIX  mProj;

    // Get the projection and view matrix from the camera class
    mWorld = g_mCenterMesh * *g_Camera.GetWorldMatrix();
    mProj = *g_Camera.GetProjMatrix();
    mView = *g_Camera.GetViewMatrix();

    
OnD3D11CreateDevice()
{
  ...
    g_pLightDir = g_pEffect11->GetVariableByName( "g_LightDir" )->AsVector();
    g_pLightDiffuse = g_pEffect11->GetVariableByName( "g_LightDiffuse" )->AsVector();
    g_pmWorldViewProjection = g_pEffect11->GetVariableByName( 
        "g_mWorldViewProjection" )->AsMatrix();
    g_pmWorld = g_pEffect11->GetVariableByName( "g_mWorld" )->AsMatrix();
    g_pfTime = g_pEffect11->GetVariableByName( "g_fTime" )->AsScalar();
    g_pMaterialAmbientColor = g_pEffect11->GetVariableByName("g_MaterialAmbientColor")->AsVector();
    g_pMaterialDiffuseColor = g_pEffect11->GetVariableByName( 
        "g_MaterialDiffuseColor" )->AsVector();
    g_pnNumLights = g_pEffect11->GetVariableByName( "g_nNumLights" )->AsScalar();
}
```



В третьих, используйте методы Update, чтобы задать значения переменных в приложении в переменных эффектов.


```
           
OnD3D11FrameRender()
{
    ...
    g_pLightDir->SetRawValue( vLightDir, 0, sizeof(D3DXVECTOR3)*MAX_LIGHTS );
    g_pLightDiffuse->SetFloatVectorArray( (float*)vLightDiffuse, 0, MAX_LIGHTS );
    g_pmWorldViewProjection->SetMatrix( (float*)&mWorldViewProjection );
    g_pmWorld->SetMatrix( (float*)&mWorld );
    g_pfTime->SetFloat( (float)fTime );
    g_pnNumLights->SetInt( g_nNumActiveLights );
}
```



### <a name="two-ways-to-get-the-state-in-an-effect-variable"></a>Два способа получения состояния в переменной Effect

Существует два способа получить состояние, содержащееся в переменной Effect. С учетом влияния, которое было загружено в память.

Один из способов — получить состояние образца из [**ID3DX11EffectVariable**](id3dx11effectvariable.md) , которое было приведено в качестве интерфейса выборки.


```
D3D11_SAMPLER_DESC sampler_desc;
ID3D11EffectSamplerVariable* l_pD3D11EffectVariable = NULL;
if( g_pEffect11 )
{
    l_pD3D11EffectVariable = g_pEffect11->GetVariableByName( "MeshTextureSampler" )->AsSampler();
    if( l_pD3D11EffectVariable->IsValid() )
        hr = (l_pD3D11EffectVariable->GetBackingStore( 0, 
            &sampler_desc );
}
```



Другой способ — получить состояние образца из [**ID3D11SamplerState**](/windows/desktop/api/D3D11/nn-d3d11-id3d11samplerstate).


```
ID3D11SamplerState* l_ppSamplerState = NULL;
D3D11_SAMPLER_DESC sampler_desc;
ID3D11EffectSamplerVariable* l_pD3D11EffectVariable = NULL;
if( g_pEffect11 )
{
    l_pD3D11EffectVariable = g_pEffect11->GetVariableByName( "MeshTextureSampler" )->AsSampler();
    if( l_pD3D11EffectVariable->IsValid )
    {
        hr = l_pD3D11EffectVariable->GetSampler( 0, 
            &l_ppSamplerState );
        if( l_ppSamplerState )
            l_ppSamplerState->GetDesc( &sampler_desc );
    }
}
```



## <a name="shader-state"></a>Состояние шейдера

Состояние шейдера объявляется и назначается в методике действия в рамках прохода.


```
VertexShader vsRenderScene = CompileShader( vs_4_0, RenderSceneVS( 1, true, true );  
technique10 RenderSceneWithTexture1Light
{
    pass P0
    {
        SetVertexShader( vsRenderScene );
        SetGeometryShader( NULL );
        SetPixelShader( CompileShader( ps_4_0, RenderScenePS( true ) ) );
    }
}
```



Это работает так же, как если бы вы не использовали никаких эффектов. Существует три вызова, по одному для каждого типа шейдера (вершина, геометрия и пиксель). Первый из них, Сетвертексшадер, вызывает [**ссылку ID3D11DeviceContext:: вссетшадер**](/windows/desktop/api/D3D11/nf-d3d11-id3d11devicecontext-vssetshader). Компилешадер — это специальная функция, которая принимает профиль шейдера (VS \_ 4 \_ 0) и имя функции шейдера вершин (рендервс). Иными словами, каждый из этих вызовов Компилешадер компилирует свою связанную функцию шейдера и возвращает указатель на скомпилированный шейдер.

Обратите внимание, что должно быть задано не все состояние шейдера. Этот проход не включает вызовы Сесуллшадер или Сетдомаиншадер, что означает, что привязанные в данный момент поверхности и шейдеры доменов будут неизменными.

## <a name="texture-state"></a>Состояние текстуры

Состояние текстуры немного сложнее, чем задание переменной, поскольку данные текстуры не просто считываются как переменная, она выдается из текстуры. Поэтому необходимо определить переменную текстуры (как и обычную переменную, за исключением того, что она использует тип текстуры), и необходимо определить условия выборки. Ниже приведен пример объявления переменной текстуры и соответствующего объявления состояния выборки.


```
Texture2D g_MeshTexture;            // Color texture for mesh

SamplerState MeshTextureSampler
{
    Filter = MIN_MAG_MIP_LINEAR;
    AddressU = Wrap;
    AddressV = Wrap;
};

```



Ниже приведен пример настройки текстуры из приложения. В этом примере текстура хранится в данных сетки, которая была загружена при создании результата.

Первый шаг — получение указателя на текстуру из результата (из сетки).


```
ID3D11EffectShaderResourceVariable* g_ptxDiffuse = NULL;

// Obtain variables
g_ptxDiffuse = g_pEffect11->GetVariableByName( "g_MeshTexture" )->AsShaderResource();
```



На втором шаге указывается представление для доступа к текстуре. Представление определяет общий способ доступа к данным из ресурса текстуры.


```
   
OnD3D11FrameRender()
{
  ID3D11ShaderResourceView* pDiffuseRV = NULL;

  ...
  pDiffuseRV = g_Mesh11.GetMaterial(pSubset->MaterialID)->pDiffuseRV11;
  g_ptxDiffuse->SetResource( pDiffuseRV );
  ...
}   
```



С точки зрения приложения неупорядоченные представления доступа обрабатываются аналогично представлениям ресурсов шейдера. Однако в построителейх шейдеров и функций шейдера неупорядоченные данные представления доступа считываются и записываются напрямую. Невозможно выполнить выборку из представления неупорядоченного доступа.

Дополнительные сведения о просмотре ресурсов см. в разделе [ресурсы](overviews-direct3d-11-resources.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Отрисовка результата (Direct3D 11)](d3d11-graphics-programming-guide-effects-render.md)
</dt> </dl>

 

 




