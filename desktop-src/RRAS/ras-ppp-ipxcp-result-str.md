---
title: Структура RAS_PPP_IPXCP_RESULT (Рассапи. h)
description: '\_структура результатов протокола удаленного доступа ppp ррр \_ \_ используется для передачи результатов операции проекции IPX-Exchange пакетов ppp для порта.'
ms.assetid: e1236e1b-f0ef-46cf-a12f-35529215752c
keywords:
- RAS структуры RAS_PPP_IPXCP_RESULT
topic_type:
- apiref
api_name:
- RAS_PPP_IPXCP_RESULT
api_location:
- Rassapi.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5bb7ca4d006bd1a1df5a645799998b463c0b14f7
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127470102"
---
# <a name="ras_ppp_ipxcp_result-structure"></a>\_ \_ Структура результатов PPP для RAS РРР \_

\[структура **\_ \_ \_ результатов протокола удаленного доступа ррр PPP** не поддерживается для Windows Vista.\]

структура **\_ \_ \_ результатов протокола удаленного доступа ppp ррр** используется для передачи результатов операции проекции IPX-Exchange пакетов ppp для порта.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _RAS_PPP_IPXCP_RESULT {
  DWORD dwError;
  WCHAR wszAddress[RAS_IPXADDRESSLEN + 1];
} RAS_PPP_IPXCP_RESULT;
```



## <a name="members"></a>Участники

<dl> <dt>

**дверрор**
</dt> <dd>

Указывает результаты операции IPX-проекции. Значение NO \_ Error указывает на успешное выполнение, в этом случае член **всзаддресс** является допустимым. Если операция проекции не выполнена, **дверрор** является кодом ошибки из Winerror. h или расеррор. h.

</dd> <dt>

**всзаддресс**
</dt> <dd>

Строка в Юникоде, заканчивающаяся нулем и указывающая IPX-адрес, назначенный удаленному клиенту. Эта строка содержит * NET ***.** Форма _узла_ .

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                 |
| Окончание поддержки клиента<br/>    | Windows XP<br/>                                                                |
| Поддержка конца сервера<br/>    | Windows Server 2003<br/>                                                       |
| Заголовок<br/>                   | <dl> <dt>Рассапи. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Обзор службы удаленного доступа (RAS)](about-remote-access-service.md)
</dt> <dt>

[Структуры администрирования сервера RAS](ras-server-administration-structures.md)
</dt> <dt>

[**\_Порт RAS \_ 1**](ras-port-1-str.md)
</dt> <dt>

[**\_ \_ результат проекции PPP для RAS \_**](ras-ppp-projection-result-str.md)
</dt> <dt>

[**расадминпортжетинфо**](rasadminportgetinfo.md)
</dt> </dl>

 

 





