---
title: Функция Фрикаунтедстринг (Напутил. h)
description: Освобождает структуру данных Каунтедстринг.
ms.assetid: d080d247-9339-474b-866e-b412e82dd35f
keywords:
- Фрикаунтедстринг функция NAP
topic_type:
- apiref
api_name:
- FreeCountedString
api_location:
- qutil.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f732a069d19d6b8948854bd1fe2e23be070aa23f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461797"
---
# <a name="freecountedstring-function"></a>Функция Фрикаунтедстринг

> [!Note]  
> Платформа защиты доступа к сети недоступна начиная с Windows 10

 

Функция **фрикаунтедстринг** освобождает структуру данных [**каунтедстринг**](/windows/win32/api/naptypes/ns-naptypes-countedstring) .

## <a name="syntax"></a>Синтаксис


```C++
NAPAPI VOID WINAPI FreeCountedString(
  _In_ CountedString *countedString
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*каунтедстринг* \[ окне\]
</dt> <dd>

Указатель на структуру данных [**каунтедстринг**](/windows/win32/api/naptypes/ns-naptypes-countedstring) для освобождения.

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



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**аллоккаунтедстринг**](alloccountedstring-func.md)
</dt> </dl>

 

 





