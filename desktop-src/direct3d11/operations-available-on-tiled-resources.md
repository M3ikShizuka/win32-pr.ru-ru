---
title: Операции, доступные для мозаичных ресурсов
description: В этом разделе перечислены операции, которые можно выполнять с мозаичными ресурсами.
ms.assetid: 1CF42A18-B6EA-4BA9-BEDE-9A8CC083CBAF
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3dcc002a0724b6f545d72f0c1a7a348ce71f44c612289e0e079c85c7768f8a54
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119045602"
---
# <a name="operations-available-on-tiled-resources"></a>Операции, доступные для мозаичных ресурсов

В этом разделе перечислены операции, которые можно выполнять с мозаичными ресурсами.

-   void [**ID3D11DeviceContext2:: упдатетилемаппингс**](/windows/desktop/api/D3D11_2/nf-d3d11_2-id3d11devicecontext2-updatetilemappings) and [**ID3D11DeviceContext2:: копитилемаппингс**](/windows/desktop/api/D3D11_2/nf-d3d11_2-id3d11devicecontext2-copytilemappings) Operations — эти расположения плиток точек в мозаичном ресурсе для размещения в пулах плиток, а также для значений NULL или для обоих. Эти операции могут обновлять раздельные подмножества указателей плиток.
-   \*Операции копирования () и Update \* () — все API-интерфейсы, которые могут копировать данные в рабочую область пула по умолчанию (например, [**ID3D11DeviceContext1:: CopySubresourceRegion1**](/windows/desktop/api/D3D11_1/nf-d3d11_1-id3d11devicecontext1-copysubresourceregion1) и [**ID3D11DeviceContext1:: UpdateSubresource1**](/windows/desktop/api/D3D11_1/nf-d3d11_1-id3d11devicecontext1-updatesubresource1)), работают для мозаичных ресурсов. Чтение из несопоставленных плиток дает 0, а операции записи в несопоставленные плитки не выполняются.
-   Операции [**ID3D11DeviceContext2:: копитилес**](/windows/desktop/api/D3D11_2/nf-d3d11_2-id3d11devicecontext2-copytiles) и [**ID3D11DeviceContext2:: упдатетилес**](/windows/desktop/api/D3D11_2/nf-d3d11_2-id3d11devicecontext2-updatetiles) . Эти операции существуют для копирования плиток по степени гранулярности 64 КБ на детализацию и из любого ресурса-буфера в каноническом макете памяти. Видеодрайвер и оборудование выполняют любую память "группирующие", необходимую для мозаичного ресурса.
-   Привязки конвейера Direct3D и представления и привязки представлений, которые будут работать с ресурсами, не являющимися мозаичными, работают и для мозаичных ресурсов.

Элементы управления плиткой доступны в немедленных и отложенных контекстах (так же, как и обновления типичных ресурсов) и после выполнения влияют на последующие обращения к плиткам (но не ранее отправленные операции).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Создание мозаичных ресурсов](creating-tiled-resources.md)
</dt> </dl>

 

 




