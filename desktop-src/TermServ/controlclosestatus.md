---
title: Перечисление Контролклосестатус
description: Указывает, может ли приложение, содержащее элемент управления, немедленно закрыть элемент управления.
ms.assetid: ac2e1c68-81b1-4b51-aa7e-0ff703e619a2
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов перечисления Контролклосестатус
topic_type:
- apiref
api_name:
- ControlCloseStatus
api_location:
- MsTscAx.dll
api_type:
- LibDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e663ce5f6b8fd4536942bd9426c230255aa5132c04a3e2ed0133d6d32d4e6272
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119401624"
---
# <a name="controlclosestatus-enumeration"></a>Перечисление Контролклосестатус

Указывает, может ли приложение, содержащее элемент управления, немедленно закрыть элемент управления.

## <a name="syntax"></a>Синтаксис


```C++
enum ControlCloseStatus {
  controlCloseCanProceed     = 0x0000, 
  controlCloseWaitForEvents  = 0x0001 

};
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="controlCloseCanProceed"></span><span id="controlclosecanproceed"></span><span id="CONTROLCLOSECANPROCEED"></span>**контролклосеканпроцеед**
</dt> <dd>

Контейнер может немедленно закрываться. Это может произойти, если элемент управления не подключен.

</dd> <dt>

<span id="controlCloseWaitForEvents"></span><span id="controlclosewaitforevents"></span><span id="CONTROLCLOSEWAITFOREVENTS"></span>**контролклосеваитфоревентс**
</dt> <dd>

Контейнер должен ожидать событий [**имстскаксевентс:: Ondisconnectо**](imstscaxevents-ondisconnected.md) или [**Имстскаксевентс:: онконфирмклосе**](imstscaxevents-onconfirmclose.md).

</dd> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1<br/>                                                                 |
| Минимальная версия сервера<br/> | Windows Server 2012 R2<br/>                                                      |
| Библиотека типов<br/>             | <dl> <dt>MsTscAx.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Имсрдпклиент:: RequestClose**](imsrdpclient-requestclose.md)
</dt> <dt>

[**Имстскаксевентс:: Онконфирмклосе**](imstscaxevents-onconfirmclose.md)
</dt> <dt>

[**Имстскаксевентс:: ondisconnectо**](imstscaxevents-ondisconnected.md)
</dt> </dl>

 

 





