---
title: Метод Сетстрингпроперти класса Win32_RDMSDeploymentSettings (Цертенролл. h)
description: Обновляет строковое свойство для параметров развертывания коллекции виртуальных рабочих столов.
ms.assetid: 500ab1cb-7336-47a8-adee-790976ea30fe
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Сетстрингпроперти
- Службы удаленных рабочих столов метода Сетстрингпроперти, класс Win32_RDMSDeploymentSettings
- Класс Win32_RDMSDeploymentSettings службы удаленных рабочих столов, метод Сетстрингпроперти
topic_type:
- apiref
api_name:
- Win32_RDMSDeploymentSettings.SetStringProperty
api_location:
- RDMS.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 138f6d91ed428caabf8da69e3d958675f879dd15
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127374404"
---
# <a name="setstringproperty-method-of-the-win32_rdmsdeploymentsettings-class"></a>Метод Сетстрингпроперти \_ класса Win32 рдмсдеплойментсеттингс

Обновляет строковое свойство для параметров развертывания коллекции виртуальных рабочих столов.

## <a name="syntax"></a>Синтаксис


```mof
uint32 SetStringProperty(
  [in] string Key,
  [in] string Value
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Ключ* \[ окне\]
</dt> <dd>

Псевдоним коллекции виртуальных рабочих столов.

</dd> <dt>

*Значение* \[ окне\]
</dt> <dd>

Новое значение свойства.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                                   |
| Минимальная версия сервера<br/> | Windows Server 2012<br/>                                                              |
| Пространство имен<br/>                | Корневой \\ \\ rdms CIMv2<br/>                                                                |
| Заголовок<br/>                   | <dl> <dt>Цертенролл. h</dt> </dl>     |
| MOF<br/>                      | <dl> <dt>Рдманажемент. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>RDMS.dll</dt> </dl>         |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Рдмсдеплойментсеттингс Win32**](win32-rdmsdeploymentsettings.md)
</dt> </dl>

 

 





