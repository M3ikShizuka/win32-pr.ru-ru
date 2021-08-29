---
title: Метод Modify класса MicrosoftDNS_ISDNType
description: Метод Modify обновляет запись ресурса ISDN.
ms.assetid: 09e23853-ca92-43a3-8bd9-7de10eb5eddc
keywords:
- Изменение метода DNS
- Изменение метода DNS, MicrosoftDNS_ISDNType класс
- MicrosoftDNS_ISDNType класса DNS, метод Modify
topic_type:
- apiref
api_name:
- MicrosoftDNS_ISDNType.Modify
api_location:
- Root\MicrosoftDNS
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 932eb1947287ad6c24592f025301bcf42d5ffb4fc1924d1c18f771bc000396c7
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119795574"
---
# <a name="modify-method-of-the-microsoftdns_isdntype-class"></a>Метод Modify \_ класса микрософтднс исднтипе

Метод **Modify** обновляет запись ресурса ISDN.

## <a name="syntax"></a>Синтаксис


```mof
void Modify(
  [in, optional] uint32                TTL,
  [in, optional] string                ISDNNumber,
  [in, optional] string                SubAddress,
  [out, ref]     MicrosoftDNS_ISDNType &RR
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Срок жизни* \[ в необязательное\]
</dt> <dd>

Время в секундах, в течение которого запись ресурса может быть кэширована распознавателем DNS.

</dd> <dt>

*Исдннумбер* \[ в необязательное\]
</dt> <dd>

Номер ISDN и DDI владельца записи.

</dd> <dt>

*Подадрес* \[ в необязательное\]
</dt> <dd>

Подадрес владельца, если он определен.

</dd> <dt>

*RR* \[ out, ref\]
</dt> <dd>

Ссылка на новый объект.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Любой параметр, не указанный, остается неизменным в измененной записи.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                              |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                   |
| Пространство имен<br/>                | Корневой \\ микрософтднс<br/>                                                          |
| MOF<br/>                      | <dl> <dt>Днспров. mof</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Микрософтднс \_ исднтипе**](microsoftdns-isdntype.md)
</dt> <dt>

[**Метод Креатеинстанцефромпропертидата \_ класса Исднтипе микрософтднс**](microsoftdns-isdntype-createinstancefrompropertydata.md)
</dt> <dt>

[**Микрософтднс \_ ресаурцерекорд**](microsoftdns-resourcerecord.md)
</dt> </dl>

 

 





