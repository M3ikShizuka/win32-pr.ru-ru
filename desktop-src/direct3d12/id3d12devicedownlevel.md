---
title: Интерфейс ID3D12DeviceDownlevel
description: предоставляет Windows запрос статистики памяти, относящейся к -7.
keywords:
- Интерфейс ID3D12DeviceDownlevel
topic_type:
- apiref
api_name:
- ID3D12DeviceDownlevel
api_location:
- D3D12.dll
api_type:
- COM
ms.localizationpriority: low
ms.topic: reference
ms.date: 08/29/2019
ms.openlocfilehash: 401cbd0045211ef51e3ef6b06042262964ae2ec5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126966822"
---
# <a name="id3d12devicedownlevel-interface"></a>Интерфейс ID3D12DeviceDownlevel

доступ к этому интерфейсу можно получить через **QueryInterface** с [устройства direct3d 12](/windows/desktop/api/d3d12/nn-d3d12-id3d12device) при использовании [Direct3D 12 на Windows 7](https://devblogs.microsoft.com/directx/porting-directx-12-games-to-windows-7/). он предоставляет Windows запрос статистики памяти, зависящей от -7.

### <a name="methods"></a>Методы

Интерфейс **ID3D12DeviceDownlevel** содержит следующие методы.

| Метод | Описание |
|:-------|:------------|
| [**куеривидеомеморинфо**](id3d12devicedownlevel-queryvideomemoryinfo.md) | предоставляет статистику памяти для Windows 7. |

## <a name="requirements"></a>Требования

| Требование | Значение |
|--------|------------------|
| Заголовок | d3d12downlevel. h |
| DLL    | D3D12.dll (только Windows 7) |

## <a name="see-also"></a>См. также раздел
* [Интерфейсы Direct3D 12 в Windows 7](direct3d-12on7-interfaces.md)
* [справочник по Direct3D 12 на Windows 7 (d3d12downlevel. h)](direct3d-12on7-reference.md)
* [Direct3D 12 в Windows 7](https://devblogs.microsoft.com/directx/porting-directx-12-games-to-windows-7/)
