---
title: Символ D3D12SDKVersion
description: Номер версии пакета SDK Direct3D 12.
ms.localizationpriority: low
ms.topic: reference
ms.date: 08/25/2021
req.lib: ''
req.dll: d3d12core.dll
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- d3d12core.dll
api_name:
- D3D12SDKVersion
targetos: Windows
ms.openlocfilehash: f77786d0a057d8922923913984149c4b8ecd3bc8
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128520040"
---
# <a name="d3d12sdkversion-symbol"></a>Символ D3D12SDKVersion

Номер версии пакета SDK Direct3D 12.

## <a name="syntax"></a>Синтаксис

```cpp
extern "C" { _declspec(dllexport) extern const UINT D3D12SDKVersion = n;}
```

## <a name="return-value"></a>Возвращаемое значение

Значение типа [uint](../winprog/windows-data-types.md) , содержащее номер версии пакета SDK Direct3D 12.

## <a name="remarks"></a>Комментарии

**D3D12SDKVersion** не связан с библиотекой импорта или файлом заголовка.

## <a name="requirements"></a>Требования

| &nbsp; | &nbsp; |
| ---- |:---- |
| **Целевая платформа** | Windows |
| **Header** | Н/Д |
| **Библиотека** | Н/Д |
| **DLL** | d3d12core.dll |

## <a name="see-also"></a>См. также раздел
