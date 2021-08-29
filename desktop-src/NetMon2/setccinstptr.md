---
description: Функция СеткЦинстптр захватывает указатель экземпляра контекста.
ms.assetid: 31924608-4aa1-4801-a5de-d8de054e12d9
title: Функция СеткЦинстптр (Netmon. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SetCCInstPtr
api_type:
- DllExport
api_location:
- Nmapi.dll
ms.openlocfilehash: 8a438327a6c1e160ea989434666ae535660d9b5ef26fc9289a3afa9d80d3f63e
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120074364"
---
# <a name="setccinstptr-function"></a>Функция СеткЦинстптр

Функция **сеткЦинстптр** захватывает указатель экземпляра контекста.

## <a name="syntax"></a>Синтаксис


```C++
VOID WINAPI SetCCInstPtr(
   LPVOID lpCurCaptureInst
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*лпкуркаптуреинст* 
</dt> <dd>

Указатель на данные экземпляра, добавленные в запись.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет.

## <a name="remarks"></a>Remarks

Эта функция используется для сохранения указателя на блок, который был выделен с помощью функции **кчеапаллок** . Каждый синтаксический анализатор может устанавливать один экземпляр данных для записи.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl>  |
| Библиотека<br/>                  | <dl> <dt>Нмапи. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Nmapi.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[жеткЦинстптр](getccinstptr.md)
</dt> <dt>

[кчеапаллок](ccheapalloc.md)
</dt> <dt>

[кчеапфри](ccheapfree.md)
</dt> <dt>

[кчеапреаллок](ccheaprealloc.md)
</dt> <dt>

[кчеапсизе](ccheapsize.md)
</dt> </dl>

 

 




