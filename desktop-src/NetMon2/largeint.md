---
description: Тип данных ЛАРЖЕИНТ определяет большое \_ целочисленное значение.
ms.assetid: 65801136-bde7-4bca-af1f-243e757f3d8d
title: ЛАРЖЕИНТ (Netmon. h)
ms.topic: article
ms.date: 05/31/2018
topic_type:
- kbSyntax
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: d857179e97586974e11815ced5ec7c50ca276789
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171416"
---
# <a name="largeint"></a>ларжеинт

Тип данных **ларжеинт** определяет [**большое \_ целочисленное**](/windows/win32/api/winnt/ns-winnt-large_integer-r1) значение.


```C++
typedef LARGE_INTEGER* LPLARGEINT;
typedef LARGE_INTEGER UNALIGNED* ULPLARGEINT;
```



## <a name="remarks"></a>Комментарии

Элемент **лпларжеинттабле** структуры [**Set**](set.md) указывает на массив структур **набора** , определяющих одно или несколько значений ларжеинт. Если **задан этот тип структуры,** сетевой монитор отображает одну из следующих меток с каждым значением ларжеинт, найденным в пакете протокола.

-   Соответствует заданному значению. Значение ЛАРЖЕИНТ включается в набор.
-   Неизвестное значение набора. Значение ЛАРЖЕИНТ не включено в набор.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Netmon. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[SET](set.md)
</dt> </dl>

 

