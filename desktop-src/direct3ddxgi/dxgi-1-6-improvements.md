---
description: В этом разделе описаны новые возможности графической инфраструктуры Microsoft DirectX (DXGI) 1,6 для различных выпусков Windows 10.
ms.assetid: C68EC437-7600-43A8-8DEA-5A6AEE75D5AA
title: Усовершенствования DXGI 1,6
ms.topic: article
ms.date: 12/04/2019
ms.openlocfilehash: 03961b4f9af50675ee157c4840b9ed744c54f423
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574058"
---
# <a name="dxgi-16-improvements"></a>Усовершенствования DXGI 1,6

В этом разделе описаны новые возможности графической инфраструктуры Microsoft DirectX (DXGI) 1,6 для различных выпусков Windows 10.

## <a name="windows-10-october-2018-update"></a>Обновление Windows 10 за октябрь 2018 г.

эти api были добавлены для Windows 10, версия 1809 (10,0; сборка 17763) &mdash; также называется обновление Windows 10 за октябрь 2018 г..

- Интерфейс [**IDXGIFactory7**](/windows/win32/api/dxgi1_6/nn-dxgi1_6-idxgifactory7) и его методы.

## <a name="windows-10-april-2018-update"></a>Обновление Windows 10 за апрель 2018 г.

эти api были добавлены для Windows 10 версии 1803 (10,0; сборка 17134) &mdash; также называется обновлением Windows 10 апреля 2018.

- Перечисление [**DXGI_GPU_PREFERENCE**](/windows/win32/api/dxgi1_6/ne-dxgi1_6-dxgi_gpu_preference) .
- Интерфейс [**IDXGIFactory6**](/windows/win32/api/dxgi1_6/nn-dxgi1_6-idxgifactory6) и его методы.

## <a name="windows-10-fall-creators-update"></a>Windows 10 Fall Creators Update

для Windows 10 версии 1709 (10,0; сборка 16299), &mdash; также известная как Windows 10 Fall Creators Update &mdash; эти константы были добавлены в перечисление [**DXGI_ADAPTER_FLAG3**](/windows/win32/api/dxgi1_6/ne-dxgi1_6-dxgi_adapter_flag3) . 

- **DXGI_ADAPTER_FLAG3_SUPPORT_MONITORED_FENCES**
- **DXGI_ADAPTER_FLAG3_SUPPORT_NON_MONITORED_FENCES**
- **DXGI_ADAPTER_FLAG3_KEYED_MUTEX_CONFORMANCE**

## <a name="windows-10-creators-update"></a>Обновление Windows 10 Creators Update

для Windows 10 версии 1703 (10,0; сборка 15063) &mdash; также известна как Windows 10 Creators Update &mdash; для обнаружения HDR-изображений в Microsoft DirectX Graphics framework (DXGI) 1,6 были добавлены следующие функциональные возможности.

### <a name="high-dynamic-range-hdr-detection"></a>Обнаружение высокого динамического диапазона (HDR)

Эти API были добавлены для обнаружения HDR-отображений.

- Структура [**DXGI_ADAPTER_DESC3**](/windows/win32/api/dxgi1_6/ns-dxgi1_6-dxgi_adapter_desc3)
- Перечисление [**DXGI_ADAPTER_FLAG3**](/windows/win32/api/dxgi1_6/ne-dxgi1_6-dxgi_adapter_flag3)
- Перечисление [**DXGI_HARDWARE_COMPOSITION_SUPPORT_FLAGS**](/windows/win32/api/dxgi1_6/ne-dxgi1_6-dxgi_hardware_composition_support_flags)
- Структура [**DXGI_OUTPUT_DESC1**](/windows/win32/api/dxgi1_6/ns-dxgi1_6-dxgi_output_desc1)
- Функция [**дксгидеклареадаптерремовалсуппорт**](/windows/win32/api/dxgi1_6/nf-dxgi1_6-dxgideclareadapterremovalsupport)
- Интерфейс [**IDXGIAdapter4**](/windows/win32/api/dxgi1_6/nn-dxgi1_6-idxgiadapter4) и его методы
- Интерфейс [**IDXGIOutput6**](/windows/win32/api/dxgi1_6/nn-dxgi1_6-idxgioutput6) и его методы

Кроме того, для поддержки этих API-интерфейсов в перечисление [**DXGI_COLOR_SPACE_TYPE**](/windows/win32/api/dxgicommon/ne-dxgicommon-dxgi_color_space_type) добавлены константы.

## <a name="related-topics"></a>Связанные темы
[Руководством по программированию для DXGI](dx-graphics-dxgi-overviews.md)
