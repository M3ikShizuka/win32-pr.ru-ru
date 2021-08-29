---
title: Метод Modify класса MicrosoftDNS_MRType
description: Метод Modify обновляет запись ресурса переименования почтового ящика (MR).
ms.assetid: eb833735-d485-4603-9976-305244537acd
keywords:
- Изменение метода DNS
- Изменение метода DNS, MicrosoftDNS_MRType класс
- MicrosoftDNS_MRType класса DNS, метод Modify
topic_type:
- apiref
api_name:
- MicrosoftDNS_MRType.Modify
api_location:
- Root\MicrosoftDNS
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 17bc22f87a8f06bbd9497ec6dc6648e411fa8abfe3a6b8f5a1eccad81cbaf3da
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120131704"
---
# <a name="modify-method-of-the-microsoftdns_mrtype-class"></a>Метод Modify \_ класса микрософтднс мртипе

Метод **Modify** обновляет запись ресурса переименования почтового ящика (MR).

## <a name="syntax"></a>Синтаксис


```mof
void Modify(
  [in, optional] uint32              TTL,
  [in]           string              MRMailbox,
  [out, ref]     MicrosoftDNS_MRType &RR
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Срок жизни* \[ в необязательное\]
</dt> <dd>

Время в секундах, в течение которого запись ресурса может быть кэширована распознавателем DNS.

</dd> <dt>

*Мрмаилбокс* \[ окне\]
</dt> <dd>

Полное доменное имя, указывающее почтовый ящик, который является правильным именем почтового ящика, указанного в имени владельца записи.

</dd> <dt>

*RR* \[ out, ref\]
</dt> <dd>

Ссылка на измененный объект.

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



## <a name="see-also"></a>См. также

<dl> <dt>

[**Микрософтднс \_ мртипе**](microsoftdns-mrtype.md)
</dt> <dt>

[**Метод Креатеинстанцефромпропертидата \_ класса Мртипе микрософтднс**](microsoftdns-mrtype-createinstancefrompropertydata.md)
</dt> <dt>

[**Микрософтднс \_ ресаурцерекорд**](microsoftdns-resourcerecord.md)
</dt> </dl>

 

 





