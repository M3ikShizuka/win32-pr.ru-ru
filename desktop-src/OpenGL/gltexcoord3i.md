---
title: Функция glTexCoord3i (GL. h)
description: Задает текущие координаты текстуры. | Функция glTexCoord3i (GL. h)
ms.assetid: a153bbce-9f8c-48e1-a33a-a4474efe3ffd
keywords:
- Функция glTexCoord3i OpenGL
topic_type:
- apiref
api_name:
- glTexCoord3i
api_location:
- opengl32.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 2e49c063c8bb3bd60ece9cf2cf9677efa7c0235010dd0a17810227ec980b32be
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119491024"
---
# <a name="gltexcoord3i-function"></a>Функция glTexCoord3i

Задает текущие координаты текстуры.

## <a name="syntax"></a>Синтаксис


```C++
void WINAPI glTexCoord3i(
   GLint s,
   GLint t,
   GLint r
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*s* 
</dt> <dd>

Координата текстуры "s".

</dd> <dt>

*t* 
</dt> <dd>

Координата текстуры t.

</dd> <dt>

*r* 
</dt> <dd>

Координата текстуры r.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Эта функция не возвращает значение.

## <a name="remarks"></a>Remarks

Функция [**глтекскурд**](gltexcoord-functions.md) задает текущие координаты текстуры, которые являются частью данных, связанных с вершинами многоугольников. Функция **глтекскурд** задает координаты текстуры в одном, двух, трех или четырех измерениях. Функция glTexCoord1 устанавливает для текущих координат текстуры значение (s, 0, 0, 1); вызов glTexCoord2 задает для них значение (s, t, 0, 1). Аналогичным образом glTexCoord3 определяет координаты текстуры как (s, t, r, 1), а glTexCoord4 определяет все четыре компонента явным образом (s, t, r, q). Текущие координаты текстуры можно обновить в любое время. В частности, можно вызвать Глтекскурд между вызовом [**глбегин**](glbegin.md) и соответствующим вызовом [**гленд**](glend.md). Следующая функция получает сведения, связанные с **глтекскурд**:

[**глжет**](glgetbooleanv--glgetdoublev--glgetfloatv--glgetintegerv.md) с аргументом в качестве \_ \_ координат текущей текстуры главной книги \_

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                              |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                    |
| Заголовок<br/>                   | <dl> <dt>GL. h</dt> </dl>         |
| Библиотека<br/>                  | <dl> <dt>Opengl32. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Opengl32.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[глвертекс](glvertex-functions.md)
</dt> </dl>

 

 





