---
title: Создание цепочки буферов
description: В этом разделе показано, как создать цепочку подкачки, которая инкапсулирует два или больше буферов, используемых для отрисовки и отображения.
ms.assetid: 0e290b37-0807-42c7-9e50-fd2db6affb14
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 8355eafff6e233b89be82fd9e58ca53224248e84
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127342035"
---
# <a name="how-to-create-a-swap-chain"></a>Как создать цепочку буферов

В этом разделе показано, как создать цепочку подкачки, которая инкапсулирует два или больше буферов, используемых для отрисовки и отображения. Обычно они содержат интерфейсный буфер, представленный для устройства отображения, и задний буфер, который выступает в качестве целевого объекта отрисовки. После того как непосредственный контекст будет готов к просмотру в обратном буфере, цепочка буфера обмена представляет задний буфер путем переключения двух буферов.

Цепочка буфера обмена определяет несколько характеристик отрисовки, включая:

-   Размер области рендеринга.
-   Частота обновления дисплея.
-   Режим отображения.
-   Формат поверхности.

Определите характеристики цепочки буферов, заполнив структуру для [**\_ \_ цепочки буфера \_ обмена**](/windows/desktop/api/dxgi/ns-dxgi-dxgi_swap_chain_desc) и инициализируя интерфейс [**идксгисвапчаин**](/windows/desktop/api/dxgi/nn-dxgi-idxgiswapchain) . Инициализируйте цепочку подкачки путем вызова [**идксгифактори:: креатесвапчаин**](/windows/desktop/api/dxgi/nf-dxgi-idxgifactory-createswapchain) или [**D3D11CreateDeviceAndSwapChain**](/windows/desktop/api/D3D11/nf-d3d11-d3d11createdeviceandswapchain).

## <a name="create-a-device-and-a-swap-chain"></a>Создание устройства и цепочки буферов

Чтобы инициализировать устройство и цепочку буферов, используйте одну из следующих двух функций:

-   Используйте функцию [**D3D11CreateDeviceAndSwapChain**](/windows/desktop/api/D3D11/nf-d3d11-d3d11createdeviceandswapchain) , если вы хотите инициализировать цепочку буферов одновременно с инициализацией устройства. Обычно это самый простой вариант.

-   Используйте функцию [**D3D11CreateDevice**](/windows/desktop/api/D3D11/nf-d3d11-d3d11createdevice) , если цепь подкачки уже создана с помощью [**Идксгифактори:: креатесвапчаин**](/windows/desktop/api/dxgi/nf-dxgi-idxgifactory-createswapchain).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Устройства](overviews-direct3d-11-devices.md)
</dt> <dt>

[Использование Direct3D 11](how-to-use-direct3d-11.md)
</dt> </dl>

 

 