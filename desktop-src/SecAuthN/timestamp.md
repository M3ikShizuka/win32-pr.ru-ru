---
description: Тип данных TimeStamp содержит сведения о допустимости времени маркеров безопасности. Формат значения типа данных TimeStamp совпадает со значением структуры FILETIME.
ms.assetid: 0a609b32-dbd7-4905-8990-65ebabcd0668
title: Метка времени (SSPI. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4898e85b0c11f55e5bb0dba2dbdefe2a3b6a2e4e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127146553"
---
# <a name="timestamp"></a>TimeStamp

Тип данных **timestamp** содержит сведения о допустимости времени маркеров безопасности. Формат значения типа данных **timestamp** совпадает со значением структуры [**fileTime**](/windows/win32/api/minwinbase/ns-minwinbase-filetime) .


```C++
typedef SECURITY_INTEGER TimeStamp, *PTimeStamp;
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                                            |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                   |
| Заголовок<br/>                   | <dl> <dt>SSPI. h (включая Security. h)</dt> </dl> |



 

 
