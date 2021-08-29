---
title: Функция Дллдебугобжектрпчук
description: Экспортировано библиотеками DLL COM для включения удаленной отладки.
ms.assetid: a0f8bf12-0889-452d-84d0-255c5c143bc1
keywords:
- COM-функция Дллдебугобжектрпчук
topic_type:
- apiref
api_name:
- DllDebugObjectRPCHook
api_location:
- ole32.dll
- API-MS-Win-Core-Com-private-l1-1-0.dll
- ComBase.dll
- API-MS-Win-Core-COM-Private-l1-1-1.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: aaaa8932a5db6325f9a63afa50cf6a2f4fef88621567f965c3e0a7e611abb696
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119854614"
---
# <a name="dlldebugobjectrpchook-function"></a>Функция Дллдебугобжектрпчук

Экспортировано библиотеками DLL COM для включения удаленной отладки.

## <a name="syntax"></a>Синтаксис


```C++
BOOL WINAPI DllDebugObjectRPCHook(
   BOOL             fTrace,
   LPORPC_INIT_ARGS lpOrpcInitArgs
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*фтраце* 
</dt> <dd>

Если **значение — true**, удаленная отладка включена. Если задано **значение false**, удаленная отладка не включена.

</dd> <dt>

*лпорпЦинитаргс* 
</dt> <dd>

Указатель на структуру [**\_ \_ args ОРПК**](orpc-init-args.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

**Значение true** , если выполнено успешно; в противном случае — **false**

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Н/Д</dt> </dl>       |
| Библиотека<br/>                  | <dl> <dt>Ole32. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Ole32.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**ОРПК \_ dbg \_ ALL**](orpc-dbg-all.md)
</dt> <dt>

[**\_БУФЕР ОРПК dbg \_**](orpc-dbg-buffer.md)
</dt> <dt>

[**\_аргументы инициализации \_ ОРПК**](orpc-init-args.md)
</dt> <dt>

[**иорпкдебугнотифи**](iorpcdebugnotify.md)
</dt> </dl>

 

 





