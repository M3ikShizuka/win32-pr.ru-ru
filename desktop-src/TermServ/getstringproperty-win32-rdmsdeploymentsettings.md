---
title: Метод Жетстрингпроперти класса Win32_RDMSDeploymentSettings
description: Извлекает строковое свойство для параметров развертывания коллекции виртуальных рабочих столов.
ms.assetid: 468ffdea-57a9-4478-adae-3629e4522762
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Жетстрингпроперти
- Службы удаленных рабочих столов метода Жетстрингпроперти, класс Win32_RDMSDeploymentSettings
- Класс Win32_RDMSDeploymentSettings службы удаленных рабочих столов, метод Жетстрингпроперти
topic_type:
- apiref
api_name:
- Win32_RDMSDeploymentSettings.GetStringProperty
api_location:
- RDMS.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f4a7cb338cd6f6858bba0536b012effb8621eee0d68dc386eceb79cdfd694e30
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120033694"
---
# <a name="getstringproperty-method-of-the-win32_rdmsdeploymentsettings-class"></a>Метод Жетстрингпроперти \_ класса Win32 рдмсдеплойментсеттингс

Извлекает строковое свойство для параметров развертывания коллекции виртуальных рабочих столов.

## <a name="syntax"></a>Синтаксис


```mof
uint32 GetStringProperty(
  [in]  string Key,
  [out] string Value
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Ключ* \[ окне\]
</dt> <dd>

Псевдоним коллекции виртуальных рабочих столов.

</dd> <dt>

*Значение* \[ заполняет\]
</dt> <dd>

Строка, принимающая извлеченное значение.

</dd> </dl>

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

 

 





