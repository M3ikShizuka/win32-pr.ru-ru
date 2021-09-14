---
title: Метод Инапенфорцементклиентконнектион Жетстрингкоррелатионид (Напенфорцементклиент. h)
description: Возвращает строковую версию идентификатора, используемого для корреляции запросов и ответов.
ms.assetid: d744fa4e-5e30-429e-810d-7326047bb3f8
keywords:
- Метод Жетстрингкоррелатионид NAP
- Метод Жетстрингкоррелатионид NAP, интерфейс Инапенфорцементклиентконнектион
- Инапенфорцементклиентконнектион интерфейса NAP, метод Жетстрингкоррелатионид
topic_type:
- apiref
api_name:
- INapEnforcementClientConnection.GetStringCorrelationId
api_location:
- qagent.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c6a01ca16bffb627f4ca5be38ef547980951c0ee
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461774"
---
# <a name="inapenforcementclientconnectiongetstringcorrelationid-method"></a>Метод Инапенфорцементклиентконнектион:: Жетстрингкоррелатионид

> [!Note]  
> Платформа защиты доступа к сети недоступна начиная с Windows 10

 

Метод **инапенфорцементклиентконнектион:: жетстрингкоррелатионид** Получает строковую версию идентификатора, используемого для корреляции запросов и ответов.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetStringCorrelationId(
  [out] CountedString **correlationId
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*correlationId* \[ заполняет\]
</dt> <dd>

Указатель на структуру [**каунтедстринг**](/windows/win32/api/naptypes/ns-naptypes-countedstring) , которая содержит строковую версию [**correlationId**](/windows/win32/api/naptypes/ns-naptypes-correlationid)объекта Connection.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Также могут возвращаться другие коды ошибок, относящиеся к COM.



| Код возврата                                                                                     | Описание                                                        |
|-------------------------------------------------------------------------------------------------|--------------------------------------------------------------------|
| <dl> <dt>**С \_ ОК**</dt> </dl>           | Операция успешно завершена.<br/>                                    |
| <dl> <dt>**Д \_ ACCESSDENIED**</dt> </dl> | Ошибка разрешений, доступ запрещен.<br/>                       |
| <dl> <dt>**Д \_ OUTOFMEMORY**</dt> </dl>  | Не удалось выполнить операцию из – за пределов системных ресурсов.<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                      |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                                |
| Заголовок<br/>                   | <dl> <dt>Напенфорцементклиент. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Напенфорцементклиент. idl</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Qagent.dll</dt> </dl>               |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**инапенфорцементклиентконнектион**](inapenforcementclientconnection.md)
</dt> </dl>

 

 





