---
title: Основные интерфейсы Direct3D 11
description: В этом разделе содержатся сведения об основных интерфейсах.
ms.assetid: e96804db-0987-49ca-b1b1-321f36c13024
keywords:
- интерфейсы, Direct3D 11 Core
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2485e633158d3eb1f8448249812eb6699b37a6ea
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122465011"
---
# <a name="direct3d-11-core-interfaces"></a>Основные интерфейсы Direct3D 11

В этом разделе содержатся сведения об основных интерфейсах.

## <a name="in-this-section"></a>В этом разделе




| Раздел | Описание | 
|-------|-------------|
| <a href="/windows/desktop/api/D3D11/nn-d3d11-id3d11asynchronous"><strong>ID3D11Asynchronous</strong></a><br /> | Этот интерфейс инкапсулирует методы для асинхронного извлечения данных из GPU.<br /> | 
| <a href="/windows/desktop/api/D3D11/nn-d3d11-id3d11blendstate"><strong>ID3D11BlendState</strong></a><br /> | Интерфейс состояния Blend содержит описание состояния наложения, которое можно привязать к <a href="d3d10-graphics-programming-guide-output-merger-stage.md">этапу слияния вывода</a>.<br /> | 
| <a href="/windows/desktop/api/D3D11_1/nn-d3d11_1-id3d11blendstate1"><strong>ID3D11BlendState1</strong></a><br /> | Интерфейс состояния Blend содержит описание состояния наложения, которое можно привязать к <a href="d3d10-graphics-programming-guide-output-merger-stage.md">этапу слияния вывода</a>. Этот интерфейс состояния Blend поддерживает логические операции, а также операции смешения.<br /> | 
| <a href="/windows/desktop/api/D3D11/nn-d3d11-id3d11commandlist"><strong>ID3D11CommandList</strong></a><br /> | Интерфейс <a href="/windows/desktop/api/D3D11/nn-d3d11-id3d11commandlist"><strong>ID3D11CommandList</strong></a> инкапсулирует список графических команд для воспроизведения.<br /> | 
| <a href="/windows/desktop/api/D3D11/nn-d3d11-id3d11counter"><strong>ID3D11Counter</strong></a><br /> | Этот интерфейс инкапсулирует методы для измерения производительности GPU.<br /> | 
| <a href="/windows/desktop/api/D3D11/nn-d3d11-id3d11depthstencilstate"><strong>ID3D11DepthStencilState</strong></a><br /> | Интерфейс состояния "Глубина-трафарет" содержит описание состояния шаблона глубины, которое можно привязать к <a href="d3d10-graphics-programming-guide-output-merger-stage.md">этапу слияния вывода</a>.<br /> | 
| <a href="/windows/desktop/api/D3D11/nn-d3d11-id3d11device"><strong>ID3D11Device</strong></a><br /> | Интерфейс устройства представляет виртуальный адаптер; Он используется для создания ресурсов.<br /> | 
| <a href="/windows/desktop/api/D3D11_1/nn-d3d11_1-id3d11device1"><strong>ID3D11Device1</strong></a><br /> | Интерфейс устройства представляет виртуальный адаптер; Он используется для создания ресурсов. <a href="/windows/desktop/api/D3D11_1/nn-d3d11_1-id3d11device1"><strong>ID3D11Device1</strong></a> добавляет новые методы к элементам в <a href="/windows/desktop/api/D3D11/nn-d3d11-id3d11device"><strong>ID3D11Device</strong></a>.<br /> | 
| <a href="/windows/desktop/api/D3D11_2/nn-d3d11_2-id3d11device2"><strong>ID3D11Device2</strong></a><br /> | Интерфейс устройства представляет виртуальный адаптер; Он используется для создания ресурсов. <a href="/windows/desktop/api/D3D11_2/nn-d3d11_2-id3d11device2"><strong>ID3D11Device2</strong></a> добавляет новые методы к элементам в <a href="/windows/desktop/api/D3D11_1/nn-d3d11_1-id3d11device1"><strong>ID3D11Device1</strong></a>.<br /> | 
| <a href="/windows/desktop/api/D3D11_3/nn-d3d11_3-id3d11device3"><strong>ID3D11Device3</strong></a><br /> | Интерфейс устройства представляет виртуальный адаптер; Он используется для создания ресурсов. <a href="/windows/desktop/api/D3D11_3/nn-d3d11_3-id3d11device3"><strong>ID3D11Device3</strong></a> добавляет новые методы к элементам в <a href="/windows/desktop/api/D3D11_2/nn-d3d11_2-id3d11device2"><strong>ID3D11Device2</strong></a>.<br /> | 
| <a href="/windows/desktop/api/d3d11_4/nn-d3d11_4-id3d11device4"><strong>ID3D11Device4</strong></a><br /> | Интерфейс устройства представляет виртуальный адаптер; Он используется для создания ресурсов. <a href="/windows/desktop/api/d3d11_4/nn-d3d11_4-id3d11device4"><strong>ID3D11Device4</strong></a> добавляет новые методы в <a href="/windows/desktop/api/D3D11_3/nn-d3d11_3-id3d11device3"><strong>ID3D11Device3</strong></a>, такие как <strong>регистердевицеремоведевент</strong> и <strong>унрегистердевицеремовед</strong>. <br /> | 
| <a href="/windows/desktop/api/d3d11_4/nn-d3d11_4-id3d11device5"><strong>ID3D11Device5</strong></a><br /> | Интерфейс устройства представляет виртуальный адаптер; Он используется для создания ресурсов. <a href="/windows/desktop/api/d3d11_4/nn-d3d11_4-id3d11device5"><strong>ID3D11Device5</strong></a> добавляет новые методы к элементам в <a href="/windows/desktop/api/d3d11_4/nn-d3d11_4-id3d11device4"><strong>ID3D11Device4</strong></a>.<br /> | 
| <a href="/windows/desktop/api/D3D11/nn-d3d11-id3d11devicechild"><strong>ID3D11DeviceChild</strong></a><br /> | Дочерний интерфейс устройства получает доступ к данным, используемым устройством.<br /> | 
| <a href="/windows/desktop/api/D3D11/nn-d3d11-id3d11devicecontext"><strong>ID3D11DeviceContext</strong></a><br /> | Интерфейс <a href="/windows/desktop/api/D3D11/nn-d3d11-id3d11devicecontext"><strong>ссылку ID3D11DeviceContext</strong></a> представляет контекст устройства, который создает команды отрисовки.<br /><blockquote>[!Note]<br />Последняя версия этого интерфейса — <a href="/windows/desktop/api/d3d11_3/nn-d3d11_3-id3d11devicecontext4"><strong>ID3D11DeviceContext4</strong></a> , представленная в Windows 10 Creators Update. приложения, предназначенных Windows 10 Creators Update, должны использовать интерфейс <strong>ID3D11DeviceContext4</strong> вместо <strong>ID3D11Device</strong>.</blockquote><br /> | 
| <a href="/windows/desktop/api/D3D11_1/nn-d3d11_1-id3d11devicecontext1"><strong>ID3D11DeviceContext1</strong></a><br /> | Интерфейс контекста устройства представляет контекст устройства; Он используется для визуализации команд. <a href="/windows/desktop/api/D3D11_1/nn-d3d11_1-id3d11devicecontext1"><strong>ID3D11DeviceContext1</strong></a> добавляет новые методы к элементам в <a href="/windows/desktop/api/D3D11/nn-d3d11-id3d11devicecontext"><strong>ссылку ID3D11DeviceContext</strong></a>.<br /> | 
| <a href="/windows/desktop/api/D3D11_2/nn-d3d11_2-id3d11devicecontext2"><strong>ID3D11DeviceContext2</strong></a><br /> | Интерфейс контекста устройства представляет контекст устройства; Он используется для визуализации команд. <a href="/windows/desktop/api/D3D11_2/nn-d3d11_2-id3d11devicecontext2"><strong>ID3D11DeviceContext2</strong></a> добавляет новые методы к элементам в <a href="/windows/desktop/api/D3D11_1/nn-d3d11_1-id3d11devicecontext1"><strong>ID3D11DeviceContext1</strong></a>.<br /> | 
| <a href="/windows/desktop/api/d3d11_3/nn-d3d11_3-id3d11devicecontext3"><strong>ID3D11DeviceContext3</strong></a><br /> | Интерфейс контекста устройства представляет контекст устройства; Он используется для визуализации команд. <a href="/windows/desktop/api/d3d11_3/nn-d3d11_3-id3d11devicecontext3"><strong>ID3D11DeviceContext3</strong></a> добавляет новые методы к элементам в <a href="/windows/desktop/api/D3D11_2/nn-d3d11_2-id3d11devicecontext2"><strong>ID3D11DeviceContext2</strong></a>. <br /> | 
| <a href="/windows/desktop/api/d3d11_3/nn-d3d11_3-id3d11devicecontext4"><strong>ID3D11DeviceContext4</strong></a><br /> | Интерфейс контекста устройства представляет контекст устройства; Он используется для визуализации команд. <a href="/windows/desktop/api/d3d11_3/nn-d3d11_3-id3d11devicecontext4"><strong>ID3D11DeviceContext4</strong></a> добавляет новые методы к элементам в <a href="/windows/desktop/api/d3d11_3/nn-d3d11_3-id3d11devicecontext3"><strong>ID3D11DeviceContext3</strong></a>.<br /> | 
| <a href="/windows/desktop/api/d3d11_1/nn-d3d11_1-id3ddevicecontextstate"><strong>ID3DDeviceContextState</strong></a><br /> | Интерфейс <a href="/windows/desktop/api/d3d11_1/nn-d3d11_1-id3ddevicecontextstate"><strong>ID3DDeviceContextState</strong></a> представляет объект состояния контекста, который содержит сведения о состоянии и поведении для устройства Microsoft Direct3D.<br /> | 
| <a href="/windows/desktop/api/D3D11_3/nn-d3d11_3-id3d11fence"><strong>ID3D11Fence</strong></a><br /> | Представляет ограждение, объект, используемый для синхронизации ЦП и один или несколько GPU.<br /> | 
| <a href="/windows/desktop/api/d3d11/nn-d3d11-id3d11inputlayout"><strong>ID3D11InputLayout</strong></a><br /> | Интерфейс макета ввода содержит определение того, как передавать данные вершин, размещенные в памяти, в <a href="d3d10-graphics-programming-guide-input-assembler-stage.md">этап ассемблерного</a> <a href="overviews-direct3d-11-graphics-pipeline.md">конвейера</a>.<br /> | 
| <a href="/windows/desktop/api/d3d11_4/nn-d3d11_4-id3d11multithread"><strong>ID3D11Multithread</strong></a><br /> | Обеспечивает защиту потоков для критически важных частей многопоточного приложения.<br /> | 
| <a href="/windows/desktop/api/d3d11/nn-d3d11-id3d11predicate"><strong>ID3D11Predicate</strong></a><br /> | Интерфейс предиката определяет, должна ли быть обработана геометрия в зависимости от результатов предыдущего вызова Draw.<br /> | 
| <a href="/windows/desktop/api/D3D11/nn-d3d11-id3d11query"><strong>ID3D11Query</strong></a><br /> | Интерфейс запроса запрашивает информацию из GPU.<br /> | 
| <a href="/windows/desktop/api/D3D11_3/nn-d3d11_3-id3d11query1"><strong>ID3D11Query1</strong></a><br /> | Представляет объект запроса для запроса сведений из графического процессора.<br /> | 
| <a href="/windows/desktop/api/D3D11/nn-d3d11-id3d11rasterizerstate"><strong>ID3D11RasterizerState</strong></a><br /> | Интерфейс состояния средства программной прорисовки содержит описание состояния средства растеризации, которое можно привязать к <a href="d3d10-graphics-programming-guide-rasterizer-stage.md">этапу средства прорисовки</a>.<br /> | 
| <a href="/windows/desktop/api/D3D11_1/nn-d3d11_1-id3d11rasterizerstate1"><strong>ID3D11RasterizerState1</strong></a><br /> | Интерфейс состояния средства программной прорисовки содержит описание состояния средства растеризации, которое можно привязать к <a href="d3d10-graphics-programming-guide-rasterizer-stage.md">этапу средства прорисовки</a>. Этот интерфейс состояния средства отображения программной прорисовки поддерживает принудительное число выборок.<br /> | 
| <a href="/windows/desktop/api/D3D11_3/nn-d3d11_3-id3d11rasterizerstate2"><strong>ID3D11RasterizerState2</strong></a><br /> | Интерфейс состояния средства программной прорисовки содержит описание состояния средства растеризации, которое можно привязать к <a href="d3d10-graphics-programming-guide-rasterizer-stage.md">этапу средства прорисовки</a>. Этот интерфейс состояния средства отображения программной прорисовки поддерживает принудительное число выборок и консервативный режим растрирования.<br /> | 
| <a href="/windows/desktop/api/D3D11/nn-d3d11-id3d11samplerstate"><strong>ID3D11SamplerState</strong></a><br /> | В интерфейсе состояния выборки содержится описание состояния образца, которое можно привязать к любому этапу шейдера <a href="overviews-direct3d-11-graphics-pipeline.md">конвейера</a> для ссылки на операции выборки текстуры.<br /> | 




 

Direct3D 11 реализует интерфейсы для:

-   [Ресурсы](d3d11-graphics-reference-resource-interfaces.md)
-   [Шейдеры](d3d11-graphics-reference-d3d11-shader-interfaces.md)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Справочник по основным](d3d11-graphics-reference-d3d11-core.md)
</dt> </dl>

