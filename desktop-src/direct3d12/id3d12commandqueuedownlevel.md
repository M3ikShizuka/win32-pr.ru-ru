---
title: Интерфейс ID3D12CommandQueueDownlevel
description: предоставляет Windowsный механизм, относящийся к -7.
keywords:
- Интерфейс ID3D12CommandQueueDownlevel
topic_type:
- apiref
api_name:
- ID3D12CommandQueueDownlevel
api_location:
- D3D12.dll
api_type:
- COM
ms.localizationpriority: low
ms.topic: reference
ms.date: 08/29/2019
ms.openlocfilehash: 61b41171d484797ff522cd32171e6ca168d586845c748de5a90e8c349bafdc1c
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120069654"
---
# <a name="id3d12commandqueuedownlevel-interface"></a>Интерфейс ID3D12CommandQueueDownlevel

доступ к этому интерфейсу можно получить через **QueryInterface** из [очереди команд direct3d 12](/windows/desktop/api/d3d12/nn-d3d12-id3d12commandqueue) при использовании [Direct3D 12 в Windows 7](https://devblogs.microsoft.com/directx/porting-directx-12-games-to-windows-7/). он предоставляет Windowsный механизм, специфичный для -7.

### <a name="methods"></a>Методы

Интерфейс **ID3D12CommandQueueDownlevel** содержит следующие методы.

| Метод | Описание |
|:-------|:------------|
| [**Настоящее**](id3d12commandqueuedownlevel-present.md) | Копирует содержимое из ресурса D3D12 Texture2D в окно. |

## <a name="requirements"></a>Requirements (Требования)

| Требование | Значение |
|--------|------------------|
| Заголовок | d3d12downlevel. h |
| DLL    | D3D12.dll (только Windows 7) |

## <a name="see-also"></a>См. также
* [Интерфейсы Direct3D 12 в Windows 7](direct3d-12on7-interfaces.md)
* [справочник по Direct3D 12 на Windows 7 (d3d12downlevel. h)](direct3d-12on7-reference.md)
* [Direct3D 12 в Windows 7](https://devblogs.microsoft.com/directx/porting-directx-12-games-to-windows-7/)
