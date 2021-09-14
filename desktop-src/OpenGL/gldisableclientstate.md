---
title: Функция Глдисаблеклиентстате (GL. h)
description: Функции Гленаблеклиентстате и Глдисаблеклиентстате включают и отключают массивы соответственно. | Функция Глдисаблеклиентстате (GL. h)
ms.assetid: b3316519-00ed-45f8-9c4b-2e04c483751e
keywords:
- Функция Глдисаблеклиентстате OpenGL
topic_type:
- apiref
api_name:
- glDisableClientState
api_location:
- Opengl32.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 163a7c3b679c979e5c800d2aa41ba2abb00e11f4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127348394"
---
# <a name="gldisableclientstate-function"></a>Функция Глдисаблеклиентстате

Функции [**гленаблеклиентстате**](glenableclientstate.md) и **глдисаблеклиентстате** включают и отключают массивы соответственно.

## <a name="syntax"></a>Синтаксис


```C++
void WINAPI glDisableClientState(
   GLenum array
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*array*. 
</dt> <dd>

Символьная константа для массива, который необходимо включить или отключить. Этот параметр может принимать одно из следующих значений.



| Значение                                                                                                                                                                                      | Значение                                                                                                                                                                                                                                                             |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span id="GL_COLOR_ARRAY"></span><span id="gl_color_array"></span><dl> <dt>**\_массив цветов \_ GL**</dt> </dl>                          | Если параметр включен, используйте массивы цветов с вызовами [**гларрайелемент**](glarrayelement.md), [**глдравелементс**](gldrawelements.md)или [**глдраваррайс**](gldrawarrays.md).<br/> См. также [**глколорпоинтер**](glcolorpointer.md).<br/>                    |
| <span id="GL_EDGE_FLAG_ARRAY"></span><span id="gl_edge_flag_array"></span><dl> <dt>**\_ \_ массив флагов РЕБРы GL \_**</dt> </dl>             | Если параметр включен, используйте массивы пограничных флагов с вызовами [**гларрайелемент**](glarrayelement.md), [**глдравелементс**](gldrawelements.md)или [**глдраваррайс**](gldrawarrays.md).<br/> См. также [**гледжефлагпоинтер**](gledgeflagpointer.md).<br/>          |
| <span id="GL_INDEX_ARRAY"></span><span id="gl_index_array"></span><dl> <dt>**\_массив индексов GL \_**</dt> </dl>                          | Если параметр включен, используйте индексные массивы с вызовами [**гларрайелемент**](glarrayelement.md), [**глдравелементс**](gldrawelements.md)или [**глдраваррайс**](gldrawarrays.md).<br/> См. также [**глиндекспоинтер**](glindexpointer.md).<br/>                    |
| <span id="GL_NORMAL_ARRAY"></span><span id="gl_normal_array"></span><dl> <dt>**\_стандартный \_ массив GL**</dt> </dl>                       | Если параметр включен, используйте обычные массивы с вызовами [**гларрайелемент**](glarrayelement.md), [**глдравелементс**](gldrawelements.md)или [**глдраваррайс**](gldrawarrays.md).<br/> См. также [**глнормалпоинтер**](glnormalpointer.md).<br/>                 |
| <span id="GL_TEXTURE_COORD_ARRAY"></span><span id="gl_texture_coord_array"></span><dl> <dt>**\_ \_ массив курд текстуры \_ GL**</dt> </dl> | Если параметр включен, используйте массивы координат текстуры с вызовами [**гларрайелемент**](glarrayelement.md), [**глдравелементс**](gldrawelements.md)или [**глдраваррайс**](gldrawarrays.md).<br/> См. также [**глтекскурдпоинтер**](gltexcoordpointer.md).<br/> |
| <span id="GL_VERTEX_ARRAY"></span><span id="gl_vertex_array"></span><dl> <dt>**\_массив ВЕРШИН \_ GL**</dt> </dl>                       | Если параметр включен, используйте массивы вершин с вызовами [**гларрайелемент**](glarrayelement.md), [**глдравелементс**](gldrawelements.md)или [**глдраваррайс**](gldrawarrays.md).<br/> См. также [**глвертекспоинтер**](glvertexpointer.md).<br/>                 |



 

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Эта функция не возвращает значение.

## <a name="error-codes"></a>Коды ошибок

С помощью функции [**глжетеррор**](glgeterror.md) можно получить следующий код ошибки.



| Имя                                                                                             | Значение                                       |
|--------------------------------------------------------------------------------------------------|-----------------------------------------------|
| <dl> <dt>**\_недействительное \_ перечисление GL**</dt> </dl> | *массив* не является допустимым значением.<br/> |



## <a name="remarks"></a>Remarks

Функции [**гленаблеклиентстате**](glenableclientstate.md) и **глдисаблеклиентстате** включают и отключают различные отдельные массивы. Чтобы определить текущее значение любой возможности, используйте [**глисенаблед**](glisenabled.md) или [**глжет**](glgetbooleanv--glgetdoublev--glgetfloatv--glgetintegerv.md) .

Вызов [**гленаблеклиентстате**](glenableclientstate.md) и **глдисаблеклиентстате** между вызовами [**Глбегин**](glbegin.md) и соответствующим вызовом [**гленд**](glend.md) может привести к ошибке. Если ошибка не возникает, поведение не определено.

> [!Note]  
> Функции [**гленаблеклиентстате**](glenableclientstate.md) и **глдисаблеклиентстате** доступны только в OpenGL версии 1,1 или более поздней.

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                              |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                    |
| Заголовок<br/>                   | <dl> <dt>GL. h</dt> </dl>         |
| Библиотека<br/>                  | <dl> <dt>Opengl32. lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Opengl32.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**гларрайелемент**](glarrayelement.md)
</dt> <dt>

[**глбегин**](glbegin.md)
</dt> <dt>

[**глколорпоинтер**](glcolorpointer.md)
</dt> <dt>

[**глдраваррайс**](gldrawarrays.md)
</dt> <dt>

[**glDrawElements**](gldrawelements.md)
</dt> <dt>

[**гледжефлагпоинтер**](gledgeflagpointer.md)
</dt> <dt>

[**гленабле**](glenable.md)
</dt> <dt>

[**гленаблеклиентстате**](glenableclientstate.md)
</dt> <dt>

[**гленд**](glend.md)
</dt> <dt>

[**глжетпоинтерв**](glgetpointerv.md)
</dt> <dt>

[**глиндекспоинтер**](glindexpointer.md)
</dt> <dt>

[**глинтерлеаведаррайс**](glinterleavedarrays.md)
</dt> <dt>

[**глнормалпоинтер**](glnormalpointer.md)
</dt> <dt>

[**глтекскурдпоинтер**](gltexcoordpointer.md)
</dt> <dt>

[**глвертекспоинтер**](glvertexpointer.md)
</dt> </dl>

 

 





