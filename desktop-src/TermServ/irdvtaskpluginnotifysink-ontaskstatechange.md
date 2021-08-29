---
title: Ирдвтаскплугиннотифисинк Онтаскстатечанже, метод
description: Используется для уведомления агента активации о том, что состояние задачи изменилось.
ms.assetid: 3021ea7a-2627-48d1-8df5-c40e7a9b51c5
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Онтаскстатечанже
- Службы удаленных рабочих столов метода Онтаскстатечанже, интерфейс Ирдвтаскплугиннотифисинк
- Службы удаленных рабочих столов интерфейса Ирдвтаскплугиннотифисинк, метод Онтаскстатечанже
topic_type:
- apiref
api_name:
- IRDVTaskPluginNotifySink.OnTaskStateChange
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: b6e580a78ba14363b140d48896d63ddafaf27f5a2e64c9ff18045b007bcc8d9f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118129116"
---
# <a name="irdvtaskpluginnotifysinkontaskstatechange-method"></a>Метод Ирдвтаскплугиннотифисинк:: Онтаскстатечанже

Используется для уведомления агента активации о том, что состояние задачи изменилось.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT OnTaskStateChange(
  [in] BSTR            bstrIdentifier,
  [in] RDV_TASK_STATUS status
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*bstrIdentifier* \[ окне\]
</dt> <dd>

Тип: **BSTR**

Идентификатор задачи. Это идентификатор, передаваемый методу [**StartTask**](irdvtaskplugin-starttask.md) .

</dd> <dt>

*состояние* \[ окне\]
</dt> <dd>

Тип: **[ **RDV \_ задача \_ состояние**](/windows/desktop/api/SessDirPublicTypes/ne-sessdirpublictypes-rdv_task_status)**

Значение перечисления [**\_ \_ состояния задачи RDV**](/windows/desktop/api/SessDirPublicTypes/ne-sessdirpublictypes-rdv_task_status) , которое указывает новое состояние задачи.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------|
| Минимальная версия клиента<br/> | Windows 7 Корпоративная<br/>   |
| Минимальная версия сервера<br/> | Windows Server 2008 R2<br/> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**\_состояние задачи \_ RDV**](/windows/desktop/api/SessDirPublicTypes/ne-sessdirpublictypes-rdv_task_status)
</dt> <dt>

[**ирдвтаскплугиннотифисинк**](irdvtaskpluginnotifysink.md)
</dt> </dl>

 

 





