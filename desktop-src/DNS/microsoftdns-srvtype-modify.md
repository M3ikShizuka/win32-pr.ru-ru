---
title: Метод Modify класса MicrosoftDNS_SRVType
description: Метод Modify обновляет запись ресурса службы (SRV).
ms.assetid: 626483c9-4b36-4e62-b9ad-dd7bb18f2e1e
keywords:
- Изменение метода DNS
- Изменение метода DNS, MicrosoftDNS_SRVType класс
- MicrosoftDNS_SRVType класса DNS, метод Modify
topic_type:
- apiref
api_name:
- MicrosoftDNS_SRVType.Modify
api_location:
- Root\MicrosoftDNS
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3b9e1a4b3b3da3fc7f7cb732c094f4ddfce2e2c0ca3e8836f25bb3034b590bf4
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119076718"
---
# <a name="modify-method-of-the-microsoftdns_srvtype-class"></a>Метод Modify \_ класса микрософтднс срвтипе

Метод **Modify** обновляет запись ресурса службы (SRV).

## <a name="syntax"></a>Синтаксис


```mof
void Modify(
  [in, optional] uint32               TTL,
  [in, optional] uint16               Priority,
  [in, optional] uint16               Weight,
  [in, optional] uint16               Port,
  [in, optional] string               SRVDomainName,
  [out, ref]     MicrosoftDNS_SRVType &RR
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Срок жизни* \[ в необязательное\]
</dt> <dd>

Время в секундах, в течение которого запись ресурса может быть кэширована распознавателем DNS.

</dd> <dt>

*Приоритет* \[ в необязательное\]
</dt> <dd>

Приоритет целевого узла, указанного в имени владельца. Более низкие значения подразумевают более высокие приоритеты.

</dd> <dt>

*Вес* \[ в необязательное\]
</dt> <dd>

Вес целевого узла. Это полезно при выборе между узлами с одинаковым приоритетом. Вероятность использования этого узла должна быть пропорциональна его весу.

</dd> <dt>

*Порт* \[ в необязательное\]
</dt> <dd>

Порт, используемый на целевом узле службы протокола.

</dd> <dt>

*Срвдомаиннаме* \[ в необязательное\]
</dt> <dd>

Полное доменное имя целевого узла. Целевой объект \\ . \\ означает, что служба не будет доступна в этом домене.

</dd> <dt>

*RR* \[ out, ref\]
</dt> <dd>

Ссылка на новый объект.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Любой параметр, не указанный, остается неизменным в измененной записи.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                              |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                   |
| Пространство имен<br/>                | Корневой \\ микрософтднс<br/>                                                          |
| MOF<br/>                      | <dl> <dt>Днспров. mof</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Микрософтднс \_ срвтипе**](microsoftdns-srvtype.md)
</dt> <dt>

[**Метод Креатеинстанцефромпропертидата \_ класса Срвтипе микрософтднс**](microsoftdns-srvtype-createinstancefrompropertydata.md)
</dt> <dt>

[**Микрософтднс \_ ресаурцерекорд**](microsoftdns-resourcerecord.md)
</dt> </dl>

 

 





