---
description: Режим адреса текстуры цвета границы, определяемый \_ элементом Border D3DTADDRESS перечисляемого типа D3DTEXTUREADDRESS, заставляет Direct3D использовать произвольный цвет, известный как цвет границы, для всех координат текстуры за пределами диапазона от 0,0 до 1,0 включительно.
ms.assetid: 689dbda1-0692-411d-9727-2fdf1df960ec
title: Режим адресации цветовой текстуры границы (Direct3D 9)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4b42b18d88f3b9305d0602e43a9528357a9397d6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127569954"
---
# <a name="border-color-texture-address-mode-direct3d-9"></a>Режим адресации цветовой текстуры границы (Direct3D 9)

Режим адреса текстуры цвета границы, определяемый \_ элементом Border D3DTADDRESS перечисляемого типа [**D3DTEXTUREADDRESS**](./d3dtextureaddress.md) , заставляет Direct3D использовать произвольный цвет, известный как цвет границы, для всех координат текстуры за пределами диапазона от 0,0 до 1,0 включительно.

На следующем рисунке приложение задает применение текстуры к примитиву с помощью рамки красного цвета.

![изображение текстуры и текстуры с красной рамкой](images/border.png)

Приложения задают цвет границы путем вызова [**IDirect3DDevice9:: сетсамплерстате**](/windows/win32/api/d3d9helper/nf-d3d9helper-idirect3ddevice9-setsamplerstate). Задайте первый параметр для вызова требуемого идентификатора стадии текстуры, второй параметр — \_ значение состояния D3DSAMP, а третий параметр — для нового цвета границы RGBA.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Режимы адресации текстур](texture-addressing-modes.md)
</dt> </dl>

 

 
