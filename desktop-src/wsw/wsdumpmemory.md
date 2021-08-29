---
title: Функция Всдумпмемори (Вебсервицесдебуг. h)
description: Эта функция создает дамп всех выделений памяти для консоли.
ms.assetid: 84a4f1e7-7d62-48c2-a8a3-ee4573bde5e4
keywords:
- Веб-службы функции Всдумпмемори для Windows
topic_type:
- apiref
api_name:
- WsDumpMemory
api_location:
- WebServicesDebug.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b92941603b78c25db06415fec42524d978a90953d0c15eaea191a8874e6b34fb
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119770894"
---
# <a name="wsdumpmemory-function"></a>Функция Всдумпмемори

Эта функция создает дамп всех выделений памяти для консоли.

> [!Note]  
> Эта функция предназначена только для отладки.

 

## <a name="syntax"></a>Синтаксис


```C++
HRESULT WINAPI  WsDumpMemory(
  _In_opt_ WS_ERROR* error
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Ошибка при* \[ в необязательное\]
</dt> <dd>

Указатель на объект [ \_ ошибки WS](ws-error.md) , в котором необходимо сохранить дополнительные сведения об ошибке в случае сбоя функции.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если эта функция завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | \[приложения UWP для классических приложений Windows 7 \|\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows \[Приложения UWP для настольных приложений Server 2008 R2 \|\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Вебсервицесдебуг. h</dt> </dl> |



 

 





