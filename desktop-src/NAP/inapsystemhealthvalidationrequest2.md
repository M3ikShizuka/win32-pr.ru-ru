---
title: Интерфейс INapSystemHealthValidationRequest2 (Напсистемхеалсвалидатор. h)
description: Предоставляет методы, используемые для поддержки средств проверки работоспособности системы, которые определяются разработчиком приложения.
ms.assetid: 12094203-bb6c-4028-9baf-a2a9b124ce6d
keywords:
- INapSystemHealthValidationRequest2 интерфейса NAP
- INapSystemHealthValidationRequest2 интерфейс NAP, описание
topic_type:
- apiref
api_name:
- INapSystemHealthValidationRequest2
api_location:
- qshvhost.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 12fdbfc46578a4e64a92accc46f6b910a44dd946
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127147222"
---
# <a name="inapsystemhealthvalidationrequest2-interface"></a>Интерфейс INapSystemHealthValidationRequest2

> [!Note]  
> Платформа защиты доступа к сети недоступна начиная с Windows 10

 

Интерфейс **INapSystemHealthValidationRequest2** предоставляет методы, используемые для поддержки средств проверки работоспособности системы, которые определяются разработчиком приложения.

> [!Note]  
> Этот интерфейс наследует все методы [**инапсистемхеалсвалидатионрекуест**](inapsystemhealthvalidationrequest.md) и использовать вместо него.

 

## <a name="members"></a>Элементы

Интерфейс **INapSystemHealthValidationRequest2** наследует от [**инапсистемхеалсвалидатионрекуест**](inapsystemhealthvalidationrequest.md). **INapSystemHealthValidationRequest2** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **INapSystemHealthValidationRequest2** содержит следующие методы.



| Метод                                                                                                    | Описание                                                        |
|:----------------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------|
| [**INapSystemHealthValidationRequest2:: Жетконфигид**](inapsystemhealthvalidationrequest2-getconfigid.md) | Извлекает идентификатор конфигурации в запросе на проверку.<br/> |



 

## <a name="remarks"></a>Remarks

Если SHV не поддерживает [**INapComponentConfig3**](inapcomponentconfig3.md), этот интерфейс не применяется.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                                               |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/>                                                 |
| Заголовок<br/>                   | <dl> <dt>Напсистемхеалсвалидатор. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Напсистемхеалсвалидатор. idl</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Qshvhost.dll</dt> </dl>                 |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**инапсистемхеалсвалидатионрекуест**](inapsystemhealthvalidationrequest.md)
</dt> <dt>

[Интерфейсы NAP](nap-interfaces.md)
</dt> <dt>

[Справочник по NAP](nap-reference.md)
</dt> </dl>

 

 





