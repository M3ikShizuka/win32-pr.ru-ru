---
title: Функция Глуделететесс (GLU. h)
description: Функция Глуделететесс уничтожает объект тесселяции.
ms.assetid: 7e1540f7-5e7d-4a3b-8c94-5a6800b17411
keywords:
- Функция Глуделететесс OpenGL
topic_type:
- apiref
api_name:
- gluDeleteTess
api_location:
- glu32.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ee4625f0a9c2f51e9d7147c9564fcd4fb1fa7117
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064950"
---
# <a name="gludeletetess-function"></a>Функция Глуделететесс

Функция **глуделететесс** уничтожает объект тесселяции.

## <a name="syntax"></a>Синтаксис


```C++
void WINAPI gluDeleteTess(
   GLUtesselator *tess
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*тесс* 
</dt> <dd>

Объект тесселяции для уничтожения (создается с помощью [**глуневтесс**](glunewtess.md)).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Эта функция не возвращает значение.

## <a name="remarks"></a>Remarks

Функция **глуделететесс** уничтожает указанный объект тесселяции и освобождает используемую память.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                           |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                 |
| Заголовок<br/>                   | <dl> <dt>Glu. h</dt> </dl>     |
| Библиотека<br/>                  | <dl> <dt>Glu32. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Glu32.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**глуневтесс**](glunewtess.md)
</dt> <dt>

[**глутессбегинполигон**](glubeginpolygon.md)
</dt> <dt>

[*глутесскаллбакк*](glutess.md)
</dt> </dl>

 

 





