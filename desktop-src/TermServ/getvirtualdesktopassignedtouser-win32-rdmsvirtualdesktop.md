---
title: Метод Жетвиртуалдесктопассигнедтаусер класса Win32_RDMSVirtualDesktop
description: Извлекает виртуальный рабочий стол, назначенный указанному пользователю.
ms.assetid: cbc22c45-4492-4651-b164-a6fd717c5ab4
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Жетвиртуалдесктопассигнедтаусер
- Службы удаленных рабочих столов метода Жетвиртуалдесктопассигнедтаусер, класс Win32_RDMSVirtualDesktop
- Класс Win32_RDMSVirtualDesktop службы удаленных рабочих столов, метод Жетвиртуалдесктопассигнедтаусер
topic_type:
- apiref
api_name:
- Win32_RDMSVirtualDesktop.GetVirtualDesktopAssignedToUser
api_location:
- RDMS.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: fcbbbed20b6b571e8867689ac901344af8e23b93
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127374729"
---
# <a name="getvirtualdesktopassignedtouser-method-of-the-win32_rdmsvirtualdesktop-class"></a>Метод Жетвиртуалдесктопассигнедтаусер \_ класса Win32 рдмсвиртуалдесктоп

Извлекает виртуальный рабочий стол, назначенный указанному пользователю.

## <a name="syntax"></a>Синтаксис


```mof
uint32 GetVirtualDesktopAssignedToUser(
  [in]  string CollectionAlias,
  [in]  string UserName,
  [in]  string UserDomain,
  [out] string VMName
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Коллектионалиас* \[ окне\]
</dt> <dd>

Псевдоним коллекции виртуальных рабочих столов, содержащей виртуальный рабочий стол.

</dd> <dt>

*Имя пользователя* \[ окне\]
</dt> <dd>

Имя пользователя.

</dd> <dt>

*Доменпользователя* \[ окне\]
</dt> <dd>

Доменное имя пользователя.

</dd> <dt>

*VMName* \[ заполняет\]
</dt> <dd>

Получает имя виртуальной машины для виртуального рабочего стола.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение 0 при успешном выполнении, в противном случае возвращает код ошибки WMI.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                                   |
| Минимальная версия сервера<br/> | Windows Server 2012<br/>                                                              |
| Пространство имен<br/>                | Корневой \\ \\ rdms CIMv2<br/>                                                                |
| MOF<br/>                      | <dl> <dt>Рдманажемент. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>RDMS.dll</dt> </dl>         |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_Рдмсвиртуалдесктоп Win32**](win32-rdmsvirtualdesktop.md)
</dt> </dl>

 

 





