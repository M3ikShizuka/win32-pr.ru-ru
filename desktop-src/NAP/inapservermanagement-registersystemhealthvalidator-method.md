---
title: Метод Инапсерверманажемент Регистерсистемхеалсвалидатор (Напсерверманажемент. h)
description: Регистрирует SHV.
ms.assetid: 23f147d5-3c4e-48ca-940a-c4350ad6ecb3
keywords:
- Метод Регистерсистемхеалсвалидатор NAP
- Метод Регистерсистемхеалсвалидатор NAP, интерфейс Инапсерверманажемент
- Инапсерверманажемент интерфейса NAP, метод Регистерсистемхеалсвалидатор
topic_type:
- apiref
api_name:
- INapServerManagement.RegisterSystemHealthValidator
api_location:
- qsvrmgmt.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 2abd8d42da196caa804a8919c6425fda9fcb950c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057436"
---
# <a name="inapservermanagementregistersystemhealthvalidator-method"></a>Метод Инапсерверманажемент:: Регистерсистемхеалсвалидатор

> [!Note]  
> Платформа защиты доступа к сети недоступна начиная с Windows 10

 

Метод **инапсерверманажемент:: регистерсистемхеалсвалидатор** регистрирует SHV.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT RegisterSystemHealthValidator(
  [in] const NapComponentRegistrationInfo *validator,
  [in] const CLSID                        *validatorClsid
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*проверяющий элемент управления* \[ окне\]
</dt> <dd>

Указатель на структуру [**напкомпонентрегистратионинфо**](/windows/win32/api/naptypes/ns-naptypes-napcomponentregistrationinfo) , содержащую сведения о регистрации SHV.

</dd> <dt>

*валидаторклсид* \[ окне\]
</dt> <dd>

Указатель на идентификатор CLSID класса COM, который реализует интерфейс [**инапсистемхеалсвалидатор**](inapsystemhealthvalidator.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Также могут возвращаться другие коды ошибок, относящиеся к COM.



| Код возврата                                                                                            | Описание                                                        |
|--------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------|
| <dl> <dt>**С \_ ОК**</dt> </dl>                  | Операция успешно завершена.<br/>                                    |
| <dl> <dt>**Д \_ ACCESSDENIED**</dt> </dl>        | Ошибка разрешений, доступ запрещен.<br/>                       |
| <dl> <dt>**Д \_ OUTOFMEMORY**</dt> </dl>         | Не удалось выполнить операцию из – за пределов системных ресурсов.<br/> |
| <dl> <dt>**\_ \_ конфликтующий идентификатор NAP \_ E**</dt> </dl> | Идентификатор SHV уже зарегистрирован.<br/>                           |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                                          |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                               |
| Заголовок<br/>                   | <dl> <dt>Напсерверманажемент. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Напсерверманажемент. idl</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Qsvrmgmt.dll</dt> </dl>            |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**инапсерверманажемент**](inapservermanagement.md)
</dt> </dl>

 

 





