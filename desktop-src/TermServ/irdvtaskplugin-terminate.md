---
title: Метод Terminate Ирдвтаскплугин
description: Вызывается при завершении работы агента задачи.
ms.assetid: b693a318-1da7-4207-8046-a62b7ccca471
ms.tgt_platform: multiple
keywords:
- Метод Terminate службы удаленных рабочих столов
- Метод Terminate службы удаленных рабочих столов, интерфейс Ирдвтаскплугин
- Интерфейс Ирдвтаскплугин службы удаленных рабочих столов, метод Terminate
topic_type:
- apiref
api_name:
- IRDVTaskPlugin.Terminate
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 178f0a7c054169d972acb6b60a9cc80578fd13e9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127168660"
---
# <a name="irdvtaskpluginterminate-method"></a>Метод Ирдвтаскплугин:: Terminate

Вызывается при завершении работы агента задачи.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Terminate(
  [in] HRESULT hr
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*HR* \[ окне\]
</dt> <dd>

Указывает, находится ли завершение работы из-за нормального завершения работы или сбоя. Если завершение работы является нормальным, оно содержит **S \_ ОК**. В противном случае он содержит код ошибки **HRESULT** .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------|
| Минимальная версия клиента<br/> | Windows 7 Корпоративная<br/>   |
| Минимальная версия сервера<br/> | Windows Server 2008 R2<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ирдвтаскплугин**](irdvtaskplugin.md)
</dt> </dl>

 

 





