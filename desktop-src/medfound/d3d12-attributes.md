---
description: Атрибуты Direct3D 12
title: Атрибуты Direct3D 12
ms.topic: article
ms.date: 08/13/2021
ms.openlocfilehash: 646d2cea8923286714982a3e083eade65f664be7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572867"
---
# <a name="direct3d-12-attributes"></a>Атрибуты Direct3D 12

Для настройки ресурсов Media Foundation Direct3D 12 можно использовать следующие атрибуты.



| attribute                                                                                                         | Описание                                                                                                              |
|-------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------|
| [MF_MT_D3D_RESOURCE_VERSION](mf-mt-d3d-resource-version.md) | Указывает версию Direct3D ресурсов, хранящихся в потоке данных, связанном с типом носителя. |
| [MF_MT_D3D12_CPU_READBACK](mf-mt-d3d12-cpu-readback.md) | Указывает, требуется ли доступ к ЦП для связанных ресурсов Direct3D. |
| [MF_MT_D3D12_RESOURCE_FLAG_ALLOW_CROSS_ADAPTER](mf-mt-d3d12-resource-flag-allow-cross-adapter.md) | Указывает, могут ли ресурсы в потоке использоваться для данных перекрестных адаптеров.  |
| [MF_MT_D3D12_RESOURCE_FLAG_ALLOW_DEPTH_STENCIL](mf-mt-d3d12-resource-flag-allow-depth-stencil.md) | Указывает, можно ли создать представление трафарета глубины для ресурсов Direct3D в потоке, связанном с типом носителя. |
| [MF_MT_D3D12_RESOURCE_FLAG_ALLOW_RENDER_TARGET](mf-mt-d3d12-resource-flag-allow-render-target.md) | Указывает, можно ли создать представление целевого объекта прорисовки для ресурсов Direct3D в потоке, связанном с типом носителя.  |
| [MF_MT_D3D12_RESOURCE_FLAG_ALLOW_SIMULTANEOUS_ACCESS](mf-mt-d3d12-resource-flag-allow-simultaneous-access.md) | Указывает, могут ли ресурсы Direct3D в потоке быть доступны одновременно нескольким различным командным очередям.  |
| [MF_MT_D3D12_RESOURCE_FLAG_ALLOW_UNORDERED_ACCESS](mf-mt-d3d12-resource-flag-allow-unordered-access.md) | Указывает, можно ли создать неупорядоченное представление доступа для ресурсов Direct3D в потоке, связанном с типом носителя. |
| [MF_MT_D3D12_RESOURCE_FLAG_DENY_SHADER_RESOURCE](mf-mt-d3d12-resource-flag-deny-shader-resource.md) | Указывает, запрещено ли создание представления ресурсов шейдера для ресурсов Direct3D в потоке, связанном с типом носителя.  |
| [MF_MT_D3D12_TEXTURE_LAYOUT](mf-mt-d3d12-texture-layout.md) | Указывает параметры макета текстуры, которые использовались для создания связанных ресурсов Direct3D.  |
| [MF_SA_D3D12_CLEAR_VALUE](mf-sa-d3d12-clear-value.md) | Содержит большой двоичный объект с информацией, используемой для оптимизации операций очистки для ресурсов Direct3D в потоке. |
| [MF_SA_D3D12_HEAP_FLAGS](mf-sa-d3d12-heap-flags.md) | Содержит значение, указывающее параметры кучи, используемые для ресурсов Direct3D в потоке. |
| [MF_SA_D3D12_HEAP_TYPE](mf-sa-d3d12-heap-type.md)  | Содержит значение, указывающее тип кучи, используемой для ресурсов Direct3D в потоке. |




 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Атрибуты Media Foundation](media-foundation-attributes.md)
</dt> <dt>

[Улучшенный модуль подготовки видео](enhanced-video-renderer.md)
</dt> </dl>

 

 



