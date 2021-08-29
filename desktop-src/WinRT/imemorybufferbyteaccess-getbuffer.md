---
description: Возвращает Имеморибуффер в виде массива байтов.
ms.assetid: E9C2AF2D-ADBE-4D76-A549-2DBCB9818B09
title: 'Метод Имеморибуффербитеакцесс:: with buffer'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IMemoryBufferByteAccess.GetBuffer
api_type:
- COM
api_location: ''
ms.openlocfilehash: df4e7897999dabd3ef7faff7d1e6f6b73c66f721256630e3ef91b154f4833b6f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119758674"
---
# <a name="imemorybufferbyteaccessgetbuffer-method"></a>Метод Имеморибуффербитеакцесс:: with buffer

Возвращает [**имеморибуффер**](/uwp/api/Windows.Foundation.IMemoryBuffer?view=winrt-19041) в виде массива байтов.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetBuffer(
  [out] BYTE   **value,
  [out] UINT32 *capacity
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*значение* \[ заполняет\]
</dt> <dd>

Указатель на массив байтов, содержащий данные буфера.

</dd> <dt>

*емкость* \[ заполняет\]
</dt> <dd>

Число байтов в возвращаемом массиве

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

При вызове [**параметр memorybuffer:: Close**](/uwp/api/Windows.Foundation.MemoryBuffer?view=winrt-19041) код, использующий этот буфер, должен установить указатель на *значение* null.

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**имеморибуффербитеакцесс**](/previous-versions//mt297505(v=vs.85))
</dt> </dl>

 

 
