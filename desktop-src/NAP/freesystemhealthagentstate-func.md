---
title: Функция Фрисистемхеалсажентстате (Напутил. h)
description: Освобождает структуру данных Системхеалсажентстате.
ms.assetid: e9bfa8ee-c335-416e-94cf-28646709d419
keywords:
- Фрисистемхеалсажентстате функция NAP
topic_type:
- apiref
api_name:
- FreeSystemHealthAgentState
api_location:
- qutil.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5161b24f983936b2eb380f1863489ea6c5c927d9b18a278e5942e162f156c6fe
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119891654"
---
# <a name="freesystemhealthagentstate-function"></a>Функция Фрисистемхеалсажентстате

> [!Note]  
> Платформа защиты доступа к сети недоступна начиная с Windows 10

 

Функция **фрисистемхеалсажентстате** освобождает структуру данных [**системхеалсажентстате**](/windows/win32/api/naptypes/ns-naptypes-systemhealthagentstate) .

## <a name="syntax"></a>Синтаксис


```C++
NAPAPI VOID WINAPI FreeSystemHealthAgentState(
  _In_ SystemHealthAgentState *state
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*состояние* \[ окне\]
</dt> <dd>

Указатель на структуру данных [**системхеалсажентстате**](/windows/win32/api/naptypes/ns-naptypes-systemhealthagentstate) для освобождения.

</dd> </dl>

## <a name="remarks"></a>Remarks

Все COM-интерфейсы, поддерживаемые системой защиты доступа к сети, используют стандартные правила управления памятью COM и распределителя памяти COM (**CoTaskMemAlloc** и **CoTaskMemFree**):

-   **Входные** параметры выделяются и освобождаются вызывающей стороной.
-   **Выходные** параметры выделяются вызываемым методом и освобождаются вызывающей стороной с помощью **котаскмем**.
-   **Входные и выходные** параметры выделяются вызывающим объектом, освобождаются и перераспределяются вызываемым объектом, и в итоге освобождаются вызывающей стороной с помощью **котаскмем**.

Все функции NAP для освобождения памяти также освобождают все внедренные указатели.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Напутил. h</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Qutil.dll</dt> </dl> |



 

 





