---
title: Метод инициализации Ирдвтаскплугин
description: Вызывается для инициализации агента задачи.
ms.assetid: eef813e6-ecca-400a-a9f3-efca6bd81161
ms.tgt_platform: multiple
keywords:
- Инициализация метода службы удаленных рабочих столов
- Инициализация метода службы удаленных рабочих столов, интерфейс Ирдвтаскплугин
- Интерфейс Ирдвтаскплугин службы удаленных рабочих столов, метод Initialize
topic_type:
- apiref
api_name:
- IRDVTaskPlugin.Initialize
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 9530be7334e1f3fefa7f73007334e448362a95ed
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127168675"
---
# <a name="irdvtaskplugininitialize-method"></a>Метод Ирдвтаскплугин:: Initialize

Вызывается для инициализации агента задачи.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Initialize(
  [in] IRDVTaskPluginNotifySink *pNotifySink
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пнотифисинк* \[ окне\]
</dt> <dd>

Тип: **[ **ирдвтаскплугиннотифисинк**](irdvtaskpluginnotifysink.md)\***

Указатель на интерфейс [**ирдвтаскплугиннотифисинк**](irdvtaskpluginnotifysink.md) , который агент задачи использует для взаимодействия с агентом триггера. Этот интерфейс необходимо освобождать, если он больше не нужен.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

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

 

 





