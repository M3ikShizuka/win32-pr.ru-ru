---
title: Функция Глупрожект (GLU. h)
description: Функция Глупрожект сопоставляет координаты объектов с координатами окна.
ms.assetid: cfd8bc5b-b684-4207-8bdb-bf086858da13
keywords:
- Функция Глупрожект OpenGL
topic_type:
- apiref
api_name:
- gluProject
api_location:
- glu32.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 84972d95d381a630bf6caf7f0099ce740a4f2741
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127244918"
---
# <a name="gluproject-function"></a>Функция Глупрожект

Функция **глупрожект** сопоставляет координаты объектов с координатами окна.

## <a name="syntax"></a>Синтаксис


```C++
int WINAPI gluProject(
         GLdouble objx,
         GLdouble objy,
         GLdouble objz,
   const GLdouble modelMatrix[16],
   const GLdouble projMatrix[16],
   const GLint    viewport[4],
         GLdouble *winx,
         GLdouble *winy,
         GLdouble *winz
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*обжкс* 
</dt> <dd>

Координата объекта x.

</dd> <dt>

*обжи* 
</dt> <dd>

Координата объекта y.

</dd> <dt>

*обжз* 
</dt> <dd>

Координата объекта z.

</dd> <dt>

*моделматрикс* 
</dt> <dd>

Текущая матрица моделвиев (как в вызове [**глжетдаублев**](glgetdoublev.md) ).

</dd> <dt>

*прожматрикс* 
</dt> <dd>

Матрица текущей проекции (как в вызове **глжетдаублев** ).

</dd> <dt>

*просмотра* 
</dt> <dd>

Текущее окно просмотра (как в вызове [**глжетинтежерв**](glgetintegerv.md) ).

</dd> <dt>

*винкс* 
</dt> <dd>

Координата вычисленного x окна.

</dd> <dt>

*вини* 
</dt> <dd>

Координата окна вычисленного y.

</dd> <dt>

*винз* 
</dt> <dd>

Координата вычисленного z окна.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если функция выполнена удачно, возвращается значение GL \_ true.

Если функция завершается ошибкой, возвращается значение GL \_ false.

## <a name="remarks"></a>Remarks

Функция **глупрожект** Преобразует указанные координаты объекта в координаты окна с помощью *моделматрикс*, *прожматрикс* и *окна просмотра*. Результат сохраняется в *Винкс*, *Вини* и *Винз*.

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

[**глжетдаублев**](glgetdoublev.md)
</dt> <dt>

[**глжетинтежерв**](glgetbooleanv--glgetdoublev--glgetfloatv--glgetintegerv.md)
</dt> <dt>

[**глуунпрожект**](gluunproject.md)
</dt> </dl>

 

 





