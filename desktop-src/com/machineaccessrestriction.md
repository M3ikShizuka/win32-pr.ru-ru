---
title: MachineAccessRestriction
description: Задает политику ограничения на уровне компьютера для доступа к компоненту.
ms.assetid: aeb37e49-6425-4058-968e-f9d00acf4fc2
keywords:
- COM-значение реестра Мачинеакцессрестриктион
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a9d99e747b8a38dbb41cb8a6a8adc0935d3f9fa8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127249253"
---
# <a name="machineaccessrestriction"></a>MachineAccessRestriction

Задает политику ограничения на уровне компьютера для доступа к компоненту.

> [!Caution]  
> Изменение этого значения повлияет на все серверные приложения COM и может препятствовать их правильной работе. Если существуют приложения COM-сервера с ограничениями, которые менее строгими по сравнению с ограничениями на уровне компьютера, уменьшение ограничений на уровне компьютера может предоставить этим приложениям нежелательный доступ. И наоборот, при увеличении ограничений на уровне компьютера некоторые серверные приложения COM могут быть недоступны при вызове приложений.

 

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Ole
   MachineAccessRestriction = SECURITY_DESCRIPTOR
```

## <a name="remarks"></a>Комментарии

Это **\_ двоичное значение reg** .

Участники, не имеющие разрешений здесь, не могут получить их, даже если разрешения предоставлены значением реестра [дефаултакцесспермиссион](defaultaccesspermission.md) или функцией [**CoInitializeSecurity**](/windows/desktop/api/combaseapi/nf-combaseapi-coinitializesecurity) .

По умолчанию члены группы «все» могут получать разрешения локального и удаленного доступа, а анонимные пользователи могут получать разрешения локального доступа.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Настройка безопасности для приложений COM](setting-security-for-com-applications.md)
</dt> </dl>

 

 




