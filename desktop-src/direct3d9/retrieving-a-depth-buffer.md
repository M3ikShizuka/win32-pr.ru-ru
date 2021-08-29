---
description: 'В следующем примере кода показано, как использовать метод IDirect3DDevice9:: ЖетдепсстенЦилсурфаце для получения указателя на поверхность буфера глубины, принадлежащую устройству.'
ms.assetid: cd5c158a-d2c4-4ced-aa6f-cd8c0e426a74
title: Получение буфера глубины (Direct3D 9)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 9ad335dae0441d61110c7c1275a01544e1834a8b3846fb442f5adab6b3169044
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119628304"
---
# <a name="retrieving-a-depth-buffer-direct3d-9"></a>Получение буфера глубины (Direct3D 9)

В следующем примере кода показано, как использовать метод [**IDirect3DDevice9:: жетдепсстенЦилсурфаце**](/windows/win32/api/d3d9helper/nf-d3d9helper-idirect3ddevice9-getdepthstencilsurface) для получения указателя на поверхность буфера глубины, принадлежащую устройству.


```
LPDIRECT3DSURFACE9 pZBuffer;

m_d3dDevice->GetDepthStencilSurface( &pZBuffer );
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Буферы глубины](depth-buffers.md)
</dt> </dl>

 

 
