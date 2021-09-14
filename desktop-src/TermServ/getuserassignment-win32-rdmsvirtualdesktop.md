---
title: Метод Жетусерассигнмент класса Win32_RDMSVirtualDesktop
description: Получение имени пользователя и домена пользователя, назначенного виртуальному рабочему столу.
ms.assetid: 1887c49d-85df-4fb4-9b40-42fb7763bf95
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Жетусерассигнмент
- Службы удаленных рабочих столов метода Жетусерассигнмент, класс Win32_RDMSVirtualDesktop
- Класс Win32_RDMSVirtualDesktop службы удаленных рабочих столов, метод Жетусерассигнмент
topic_type:
- apiref
api_name:
- Win32_RDMSVirtualDesktop.GetUserAssignment
api_location:
- RDMS.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 87293a471bb4f69b3f4c57de0f964fa0daa043cf
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127374732"
---
# <a name="getuserassignment-method-of-the-win32_rdmsvirtualdesktop-class"></a>Метод Жетусерассигнмент \_ класса Win32 рдмсвиртуалдесктоп

Получение имени пользователя и домена пользователя, назначенного виртуальному рабочему столу.

## <a name="syntax"></a>Синтаксис


```mof
uint32 GetUserAssignment(
  [out] string UserName,
  [out] string UserDomain
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Имя пользователя* \[ заполняет\]
</dt> <dd>

Получает имя пользователя.

</dd> <dt>

*Доменпользователя* \[ заполняет\]
</dt> <dd>

Получает доменное имя.

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

 

 





