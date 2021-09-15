---
title: Метод Инапклиентманажемент Жетрегистередсистемхеалсажентс (Напманажемент. h)
description: Извлекает сведения о зарегистрированном SHA.
ms.assetid: c38d2d23-62d4-49f0-81a3-52394866f0c4
keywords:
- Метод Жетрегистередсистемхеалсажентс NAP
- Метод Жетрегистередсистемхеалсажентс NAP, интерфейс Инапклиентманажемент
- Инапклиентманажемент интерфейса NAP, метод Жетрегистередсистемхеалсажентс
topic_type:
- apiref
api_name:
- INapClientManagement.GetRegisteredSystemHealthAgents
api_location:
- qagent.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a4852e2d4c1ffa08b1a7ea7b3d8395c1b116cca6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127470223"
---
# <a name="inapclientmanagementgetregisteredsystemhealthagents-method"></a>Метод Инапклиентманажемент:: Жетрегистередсистемхеалсажентс

> [!Note]  
> Платформа защиты доступа к сети недоступна начиная с Windows 10

 

Метод **жетрегистередсистемхеалсажентс** извлекает сведения о зарегистрированных SHA.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetRegisteredSystemHealthAgents(
  [out] SystemHealthEntityCount      *count,
  [out] NapComponentRegistrationInfo **agents
) const;
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*количество* \[ заполняет\]
</dt> <dd>

Указатель на [**системхеалсентитикаунт**](nap-datatypes.md) , описывающий число зарегистрированных SHA.

</dd> <dt>

*агенты* \[ заполняет\]
</dt> <dd>

Указатель на массив структур [**напкомпонентрегистратионинфо**](/windows/win32/api/naptypes/ns-naptypes-napcomponentregistrationinfo) , описывающих зарегистрированный SHA.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Метод возвращает код состояния HRESULT, включая, помимо прочего, один из следующих.



| Код возврата                                                                                         | Описание                                                        |
|-----------------------------------------------------------------------------------------------------|--------------------------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>                | Операция выполнена успешно.<br/>                                   |
| <dl> <dt>**E \_ ACCESSDENIED**</dt> </dl>      | Ошибка разрешений, доступ запрещен.<br/>                       |
| <dl> <dt>**E \_ OUTOFMEMORY**</dt> </dl>       | Не удалось выполнить операцию из – за пределов системных ресурсов.<br/> |
| <dl> <dt>**RPC \_ E \_ отключен**</dt> </dl> | Напажент не работает.<br/>                            |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                               |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                         |
| Заголовок<br/>                   | <dl> <dt>Напманажемент. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Напманажемент. idl</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Qagent.dll</dt> </dl>        |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**инапклиентманажемент**](inapclientmanagement.md)
</dt> </dl>

 

 





