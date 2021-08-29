---
title: Метод Сетсмбпас класса Win32_RDMSDeploymentSettings
description: Обновляет UNC-путь к общему ресурсу SMB, в котором развернуты виртуальные машины коллекции виртуальных рабочих столов.
ms.assetid: 0b0b5b17-7b52-41e5-b9c6-c5f3e51c7853
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Сетсмбпас
- Службы удаленных рабочих столов метода Сетсмбпас, класс Win32_RDMSDeploymentSettings
- Класс Win32_RDMSDeploymentSettings службы удаленных рабочих столов, метод Сетсмбпас
topic_type:
- apiref
api_name:
- Win32_RDMSDeploymentSettings.SetSMBPath
api_location:
- RDMS.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3c91d64b589ed61e7cc9713636dcc0f0b090da749ca9d8e8d9ab7567e8500175
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120008584"
---
# <a name="setsmbpath-method-of-the-win32_rdmsdeploymentsettings-class"></a>Метод Сетсмбпас \_ класса Win32 рдмсдеплойментсеттингс

Обновляет UNC-путь к общему ресурсу SMB, в котором развернуты виртуальные машины коллекции виртуальных рабочих столов.

## <a name="syntax"></a>Синтаксис


```mof
uint32 SetSMBPath(
  [in] string DirectoryPath
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*DirectoryPath* \[ окне\]
</dt> <dd>

Новый путь к общему ресурсу SMB в формате UNC.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение 0 при успешном выполнении, в противном случае возвращает код ошибки WMI.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                                   |
| Минимальная версия сервера<br/> | Windows Server 2012<br/>                                                              |
| Пространство имен<br/>                | Корневой \\ \\ rdms CIMv2<br/>                                                                |
| MOF<br/>                      | <dl> <dt>Рдманажемент. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>RDMS.dll</dt> </dl>         |



## <a name="see-also"></a>См. также

<dl> <dt>

[**\_Рдмсдеплойментсеттингс Win32**](win32-rdmsdeploymentsettings.md)
</dt> </dl>

 

 





