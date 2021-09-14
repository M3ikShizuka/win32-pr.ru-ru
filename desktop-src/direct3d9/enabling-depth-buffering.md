---
description: 'После создания буфера глубины, как описано в разделе Создание буфера глубины (Direct3D 9), можно включить буферизацию глубины, вызвав метод IDirect3DDevice9:: Сетрендерстате.'
ms.assetid: a3c972dd-3630-4d21-a22b-64a68e9acd19
title: Включение буферизации глубины (Direct3D 9)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 935d4f2e1db164a3aac2a39627be88d71887cc14
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126964954"
---
# <a name="enabling-depth-buffering-direct3d-9"></a>Включение буферизации глубины (Direct3D 9)

После создания буфера глубины, как описано в разделе [Создание буфера глубины (Direct3D 9)](creating-a-depth-buffer.md), можно включить буферизацию глубины, вызвав метод [**IDirect3DDevice9:: сетрендерстате**](/windows/desktop/api) . Установите \_ состояние отрисовки D3DRS зенабле, чтобы включить буферизацию глубины. Используйте член D3DZB \_ true перечисляемого типа [**D3DZBUFFERTYPE**](./d3dzbuffertype.md) (или **true**), чтобы включить z-буферизацию, D3DZB \_ усев для включения w-Buffering или D3DZB \_ false (или **false**) для отключения буферизации глубины.

> [!Note]  
> Чтобы использовать w-Buffering, приложение должно установить соответствующую матрицу проекции, даже если она не использует конвейер преобразования Direct3D. Сведения о предоставлении соответствующей матрицы проекции см. [в разделе матрица проекций, ориентированная на W](projection-transform.md)

 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Буферы глубины](depth-buffers.md)
</dt> </dl>

 

 
