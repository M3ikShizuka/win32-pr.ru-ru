---
description: Внешний свет является окружающим светом, который исходят из всех направлений. Сведения о том, как Direct3D использует окружающий свет, см. в разделе Математика освещения (Direct3D 9).
ms.assetid: c5aa493e-09b8-433c-a21c-e39af795b3c9
title: Состояние окружающего освещения (Direct3D 9)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 57bd604941961f5b4abdb301d5c23efba9980791
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053034"
---
# <a name="ambient-lighting-state-direct3d-9"></a>Состояние окружающего освещения (Direct3D 9)

Внешний свет является окружающим светом, который исходят из всех направлений. Сведения о том, как Direct3D использует окружающий свет, см. в разделе [математика освещения (Direct3D 9)](mathematics-of-lighting.md).

Приложение C++ задает цвет окружающего освещения, вызывая метод [**IDirect3DDevice9:: сетрендерстате**](/windows/win32/api/d3d9helper/nf-d3d9helper-idirect3ddevice9-setrenderstate) и передавая в качестве первого параметра перечисленное значение D3DRS \_ окружения. Вторым параметром является значение цвета. Значение по умолчанию равно нулю.


```
// This code example assumes that d3dDevice is a
// valid pointer to an IDirect3DDevice9 interface.

// Set the ambient light.

d3dDevice->SetRenderState(D3DRS_AMBIENT, 0x00202020);
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Состояния отрисовки](render-states.md)
</dt> </dl>

 

 
