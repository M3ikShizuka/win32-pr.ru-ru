---
title: Метод Синчронизепублишингдата класса Win32_RDMSManagementData
description: Синхронизирует указанный набор данных публикации для служб управления удаленный рабочий стол (RDMS).
ms.assetid: 0476ce12-9b08-418c-83c2-208275574f5b
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Синчронизепублишингдата
- Службы удаленных рабочих столов метода Синчронизепублишингдата, класс Win32_RDMSManagementData
- Класс Win32_RDMSManagementData службы удаленных рабочих столов, метод Синчронизепублишингдата
topic_type:
- apiref
api_name:
- Win32_RDMSManagementData.SynchronizePublishingData
api_location:
- RDMS.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: b5cadc3581419fa758775a48ba0190300a176364dcf0aad5a8a3ed77fa1db8bf
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119000334"
---
# <a name="synchronizepublishingdata-method-of-the-win32_rdmsmanagementdata-class"></a>Метод Синчронизепублишингдата \_ класса Win32 рдмсманажементдата

Синхронизирует указанный набор данных публикации для служб управления удаленный рабочий стол (RDMS).

## <a name="syntax"></a>Синтаксис


```mof
uint32 SynchronizePublishingData(
  [in] string Context
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Контекст* \[ окне\]
</dt> <dd>

Сведения о контексте публикуемых данных для синхронизации.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение 0 при успешном выполнении, в противном случае возвращает код ошибки WMI.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                                   |
| Минимальная версия сервера<br/> | Windows Server 2012<br/>                                                              |
| Пространство имен<br/>                | Корневой \\ \\ rdms CIMv2<br/>                                                                |
| MOF<br/>                      | <dl> <dt>Рдманажемент. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>RDMS.dll</dt> </dl>         |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Рдмсманажементдата Win32**](win32-rdmsmanagementdata.md)
</dt> </dl>

 

 





