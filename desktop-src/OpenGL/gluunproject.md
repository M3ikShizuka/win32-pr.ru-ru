---
title: Функция Глуунпрожект (GLU. h)
description: Функция Глуунпрожект сопоставляет координаты окна с координатами объекта.
ms.assetid: 6a719fc2-ad40-4b22-9c99-5753f5dbb8a0
keywords:
- Функция Глуунпрожект OpenGL
topic_type:
- apiref
api_name:
- gluUnProject
api_location:
- glu32.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f45311171dd3d71c9e699953c049e0813f2df361
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064914"
---
# <a name="gluunproject-function"></a>Функция Глуунпрожект

Функция **глуунпрожект** сопоставляет координаты окна с координатами объекта.

## <a name="syntax"></a>Синтаксис


```C++
int WINAPI gluUnProject(
         GLdouble winx,
         GLdouble winy,
         GLdouble winz,
   const GLdouble modelMatrix[16],
   const GLdouble projMatrix[16],
   const GLint    viewport[4],
         GLdouble *objx,
         GLdouble *objy,
         GLdouble *objz
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*винкс* 
</dt> <dd>

Координата окна x для сопоставления.

</dd> <dt>

*вини* 
</dt> <dd>

Координата окна y для сопоставления.

</dd> <dt>

*винз* 
</dt> <dd>

Координата окна z для сопоставления.

</dd> <dt>

*моделматрикс* 
</dt> <dd>

Матрица моделвиев (как в вызове [**глжетдаублев**](glgetdoublev.md) ).

</dd> <dt>

*прожматрикс* 
</dt> <dd>

Матрица проекции (как в вызове **глжетдаублев** ).

</dd> <dt>

*просмотра* 
</dt> <dd>

Окно просмотра (как в вызове [**глжетинтежерв**](glgetbooleanv--glgetdoublev--glgetfloatv--glgetintegerv.md) ).

</dd> <dt>

*обжкс* 
</dt> <dd>

Координата вычисленного объекта x.

</dd> <dt>

*обжи* 
</dt> <dd>

Координата вычисленного объекта y.

</dd> <dt>

*обжз* 
</dt> <dd>

Объектная координата вычисленного z.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если функция выполнена удачно, возвращается значение GL \_ true.

Если функция завершается ошибкой, возвращается значение GL \_ false.

## <a name="remarks"></a>Remarks

Функция **глуунпрожект** сопоставляет указанные координаты окна с координатами объекта с помощью *моделматрикс*, *прожматрикс* и *окна просмотра*. Результат сохраняется в *обжкс*, *обжи* и *обжз*.

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

[**глжет**](glgetbooleanv--glgetdoublev--glgetfloatv--glgetintegerv.md)
</dt> <dt>

[**глжетдаублев**](glgetbooleanv--glgetdoublev--glgetfloatv--glgetintegerv.md)
</dt> <dt>

[**глжетинтежерв**](glgetbooleanv--glgetdoublev--glgetfloatv--glgetintegerv.md)
</dt> <dt>

[**глупрожект**](gluproject.md)
</dt> </dl>

 

 





