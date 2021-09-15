---
description: В этом разделе содержатся справочные сведения по интерфейсам видео Microsoft Direct3D 12.
ms.assetid: ''
title: Интерфейсы видео Direct3D 12
ms.topic: article
ms.date: 06/03/2019
ms.openlocfilehash: 4451cac5983ddc300957b4661fc68ff30da0496a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574939"
---
# <a name="direct3d-12-video-interfaces"></a>Интерфейсы видео Direct3D 12

В этом разделе содержатся справочные сведения по интерфейсам видео Microsoft Direct3D 12.

## <a name="in-this-section"></a>В этом разделе



| Раздел                                                                                | Описание                                                                                              |
|---------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|
| [ID3D11VideoContext3](/windows/desktop/api/d3d11_4/nn-d3d11_4-id3d11videocontext3)  | Предоставляет функции видео устройства Microsoft Direct3D 11. |
| [ID3D12VideoDecodeCommandList](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videodecodecommandlist)  | Инкапсулирует список графических команд для декодирования видео.|
| [ID3D12VideoDecodeCommandList1](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videodecodecommandlist1)  | Инкапсулирует список графических команд для декодирования видео.|
| [ID3D12VideoDecoder](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videodecoder)  | Представляет видеодекодер Direct3D 12.|
| [ID3D12VideoDecoder1](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videodecoder1)  | Представляет видеодекодер Direct3D 12, который содержит независимые от разрешения ресурсы и состояние для выполнения операции декодирования. Добавляет поддержку для защищенных ресурсов.|
| [ID3D12VideoDecoderHeap](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videodecoderheap)  | Представляет кучу видеодекодера Direct3D 12.|
| [ID3D12VideoDevice](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videodevice)  | Предоставляет возможности декодирования и обработки видео устройства Microsoft Direct3D 12, включая возможность запрашивать возможности видео и создавать экземпляры видеодекодеров и процессоров.|
| [ID3D11VideoDevice2](/windows/desktop/api/d3d11_4/nn-d3d11_4-id3d11videodevice2)  | Предоставляет возможности декодирования и видеообработки видео устройства Microsoft Direct3D 11.|
| [ID3D12VideoDevice3](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videodevice3)  | Расширяет интерфейс ID3D12VideoDevice, добавляя возможности поддержки кодирования видео.|
| [ID3D12VideoExtensionCommand](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videoextensioncommand)  | Объект, который подсчитывает ссылку, представляющий команду расширения видео.|
| [ID3D12VideoEncodeCommandList](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videoencodecommandlist)  | Инкапсулирует список графических команд для кодирования видео, включая оценку движения.|
| [ID3D12VideoEncodeCommandList1](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videoencodecommandlist1)  | Этот интерфейс наследует от ID3D12VideoEncodeCommandList и добавляет поддержку команд расширения видео.|
| [ID3D12VideoEncodeCommandList2](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videoencodecommandlist2)  | Этот интерфейс наследует от ID3D12VideoEncodeCommandList1 и добавляет методы для кодирования видео и 
разрешение метаданных операции кодирования.|
| [ID3D12VideoEncoder](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videoencoder)  | Представляет видео кодировщик Direct3D 12.|
| [ID3D12VideoEncoderHeap](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videoencoderheap)  | Представляет кучу видео кодировщика Direct3D 12.|
| [ID3D12VideoMotionEstimator](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videomotionestimator)  | Этот интерфейс поддерживает контекст для операций оценки движения видео.|
| [ID3D12VideoMotionVectorHeap](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videomotionvectorheap)  | Представляет кучу, в которой хранятся предполагаемые векторы движения.|
| [ID3D12VideoProcessCommandList](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videoprocesscommandlist)  | Инкапсулирует список графических команд для обработки видео.|
| [ID3D12VideoProcessCommandList1](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videoprocesscommandlist1)  | Инкапсулирует список графических команд для обработки видео.|
| [ID3D12VideoProcessor](/windows/desktop/api/d3d12video/nn-d3d12video-id3d12videoprocessor)  | Предоставляет методы для получения сведений о параметрах для вызова ID3D12VideoDevice:: Креатевидеопроцессор, который создал обработчик видео.|



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[API-интерфейсы видео Direct3D 12](direct3d-12-video-apis.md)
</dt> </dl>

 

 




