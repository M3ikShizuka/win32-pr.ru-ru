---
description: Вызывает метод, вызываемый при завершении указанного асинхронного действия.
ms.assetid: 97199C1A-7CE3-4BBD-86A3-2CA9B27CC05E
title: 'Метод Асинкактионкомплетедхандлер:: Invoke'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- AsyncActionCompletedHandler.Invoke
api_type:
- COM
api_location:
- Windows.Foundation.idl
ms.openlocfilehash: f106dca9d1d01b2da12ffb527f3556a0a44cf535167e5af79adbd69e4a097055
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119898654"
---
# <a name="asyncactioncompletedhandlerinvoke-method"></a>Метод Асинкактионкомплетедхандлер:: Invoke

Вызывает метод, вызываемый при завершении указанного асинхронного действия.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Invoke(
  [in] IAsyncAction *asyncInfo
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*асинЦинфо* \[ окне\]
</dt> <dd>

Тип: **[ **IAsyncAction**](/windows/win32/api/windows.foundation/nn-windows-foundation-iasyncaction)\***

Асинхронное действие, которое сообщает о завершении.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8<br/>                                                                              |
| Минимальная версия сервера<br/> | Windows Server 2012<br/>                                                                    |
| Заголовок<br/>                   | <dl> <dt>Windows. Foundation. idl</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**асинкактионкомплетедхандлер**](asyncactioncompletedhandler.md)
</dt> </dl>

 

