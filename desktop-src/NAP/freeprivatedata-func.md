---
title: Функция Фриприватедата (Напутил. h)
description: Освобождает структуру данных PrivateData.
ms.assetid: 94b3618e-224f-4801-94f3-2faa1a298ec0
keywords:
- Фриприватедата функция NAP
topic_type:
- apiref
api_name:
- FreePrivateData
api_location:
- qutil.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e4629c264c91a4e0c6e18443cf27a9fd9d182164
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461786"
---
# <a name="freeprivatedata-function"></a>Функция Фриприватедата

> [!Note]  
> Платформа защиты доступа к сети недоступна начиная с Windows 10

 

Функция **фриприватедата** освобождает структуру данных [**PrivateData**](/windows/win32/api/naptypes/ns-naptypes-privatedata) .

## <a name="syntax"></a>Синтаксис


```C++
NAPAPI VOID WINAPI FreePrivateData(
  _In_ PrivateData *privateData
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*privateData* \[ окне\]
</dt> <dd>

Указатель на структуру данных [**PrivateData**](/windows/win32/api/naptypes/ns-naptypes-privatedata) для освобождения.

</dd> </dl>

## <a name="remarks"></a>Remarks

Все COM-интерфейсы, поддерживаемые системой защиты доступа к сети, используют стандартные правила управления памятью COM и распределителя памяти COM (**CoTaskMemAlloc** и **CoTaskMemFree**):

-   **Входные** параметры выделяются и освобождаются вызывающей стороной.
-   **Выходные** параметры выделяются вызываемым методом и освобождаются вызывающей стороной с помощью **котаскмем**.
-   **Входные и выходные** параметры выделяются вызывающим объектом, освобождаются и перераспределяются вызываемым объектом, и в итоге освобождаются вызывающей стороной с помощью **котаскмем**.

Все функции NAP для освобождения памяти также освобождают все внедренные указатели.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Напутил. h</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Qutil.dll</dt> </dl> |



 

 





