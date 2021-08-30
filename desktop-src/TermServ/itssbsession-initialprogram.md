---
title: Итссбсессион Инитиалпрограм, свойство
description: Возвращает или задает начальную программу для данного сеанса.
ms.assetid: c299c4f7-3c5f-468f-9fc7-81eac322dfa2
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов свойства Инитиалпрограм
- Службы удаленных рабочих столов свойства Инитиалпрограм, интерфейс Итссбсессион
- Службы удаленных рабочих столов интерфейса Итссбсессион, свойство Инитиалпрограм
topic_type:
- apiref
api_name:
- ITsSbSession.InitialProgram
- ITsSbSession.get_InitialProgram
- ITsSbSession.put_InitialProgram
api_location:
- Sbtsv.idl
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: fc1ec332283c6eb68d915c7fa0aa92070af1fb34f572d7a27adb058fa40de433
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119989894"
---
# <a name="itssbsessioninitialprogram-property"></a>Свойство Итссбсессион:: Инитиалпрограм

Возвращает или задает начальную программу для данного сеанса. Начальная программа — это программа, которая запускается при запуске сеанса пользователя.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT put_InitialProgram(
  [in]          BSTR Application
);

HRESULT get_InitialProgram(
  [out, retval] BSTR *app
);
```



## <a name="property-value"></a>Значение свойства

Переменная **BSTR** , содержащая начальную программу.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                            |
| Минимальная версия сервера<br/> | Windows Server 2012<br/>                                                       |
| IDL<br/>                      | <dl> <dt>Сбтсв. idl</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**итссбсессион**](/windows/desktop/api/sbtsv/nn-sbtsv-itssbsession)
</dt> </dl>

 

 





