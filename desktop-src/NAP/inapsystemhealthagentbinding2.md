---
title: Интерфейс INapSystemHealthAgentBinding2 (Напсистемхеалсажент. h)
description: SHA использует для взаимодействия с Напажент. | Интерфейс INapSystemHealthAgentBinding2 (Напсистемхеалсажент. h)
ms.assetid: 2b087d79-a738-42d6-a8f2-4698ab844446
keywords:
- INapSystemHealthAgentBinding2 интерфейса NAP
- INapSystemHealthAgentBinding2 интерфейс NAP, описание
topic_type:
- apiref
api_name:
- INapSystemHealthAgentBinding2
api_location:
- qagent.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f9a7491a2e78d66399f9ca246bcee9182e4f95d0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065111"
---
# <a name="inapsystemhealthagentbinding2-interface"></a>Интерфейс INapSystemHealthAgentBinding2

> [!Note]  
> Платформа защиты доступа к сети недоступна начиная с Windows 10

 

**INapSystemHealthAgentBinding2** предоставляет методы, которые SHA использует для взаимодействия с напажент.

> [!Note]  
> Этот интерфейс наследует все методы [**инапсистемхеалсажентбиндинг**](inapsystemhealthagentbinding.md) и использовать вместо него.

 

## <a name="members"></a>Элементы

Интерфейс **INapSystemHealthAgentBinding2** наследует от [**инапсистемхеалсажентбиндинг**](inapsystemhealthagentbinding.md). **INapSystemHealthAgentBinding2** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **INapSystemHealthAgentBinding2** содержит следующие методы.



| Метод                                                                                                                    | Описание                                                                                     |
|:--------------------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------|
| [**INapSystemHealthAgentBinding2:: Жетсистемисолатионинфоекс**](inapsystemhealthagentbinding2-getsystemisolationinfoex.md) | Вызывается SHA для определения состояния изоляции системы и расширенного состояния изоляции.<br/> |



 

## <a name="remarks"></a>Remarks

Все API-интерфейсы в этом интерфейсе будут возвращать **RPC \_ E \_ disconnected** , если напажент остановлен. После перезапуска этот объект будет автоматически восстановлен и повторно привязан к Напажент.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                                      |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                                |
| Заголовок<br/>                   | <dl> <dt>Напсистемхеалсажент. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Напсистемхеалсажент. idl</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Qagent.dll</dt> </dl>               |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**инапсистемхеалсажентбиндинг**](inapsystemhealthagentbinding.md)
</dt> <dt>

[Интерфейсы NAP](nap-interfaces.md)
</dt> <dt>

[Справочник по NAP](nap-reference.md)
</dt> </dl>

 

 





