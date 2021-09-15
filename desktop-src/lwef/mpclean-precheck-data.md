---
title: Структура MPCLEAN_PRECHECK_DATA (Мпклиент. h)
description: Данные уведомления передаются в функцию очистки функции обратного вызова.
ms.assetid: 65B3B116-6E83-46F5-AE2B-92A41AE39480
keywords:
- MPCLEAN_PRECHECK_DATA структуры устаревшие функции среды Windows
- функции PMPCLEAN_PRECHECK_DATA Windows указателя структур в устаревшей среде
topic_type:
- apiref
api_name:
- MPCLEAN_PRECHECK_DATA
api_location:
- MpClient.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: bc3d67e0c71c95db49b633feeb3048cc9f104b2f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127248623"
---
# <a name="mpclean_precheck_data-structure"></a>\_Структура данных ПРЕДПРОВЕРКИ мпклеан \_

Данные уведомления передаются в функцию очистки функции обратного вызова.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct tagMPCLEAN_PRECHECK_DATA {
  PMPRESOURCE_INFO     BlockedResourceInfo;
  BlockingResourceInfo PMPRESOURCE_INFO;
} MPCLEAN_PRECHECK_DATA, *PMPCLEAN_PRECHECK_DATA;
```



## <a name="members"></a>Участники

<dl> <dt>

**блоккедресаурцеинфо**
</dt> <dd>

Тип: **пмпресаурце \_ info** .

</dd> <dd>

Сведения о ресурсе блокируемого ресурса. Например, если выполняется **Проверка мпнотифиности \_ \_ ресурса \_**. См [**. \_ сведения о мпресаурце**](mpresource-info.md).

</dd> <dt>

**\_сведения о пмпресаурце**
</dt> <dd>

Тип: **блоккингресаурцеинфо**

</dd> <dd>

Сведения о ресурсе, который блокируется. Например, если выполняется **Проверка мпнотифиности \_ \_ ресурса \_**. См [**. \_ сведения о мпресаурце**](mpresource-info.md).

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                            |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Мпклиент. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_сведения о мпресаурце**](mpresource-info.md)
</dt> </dl>

 

 





