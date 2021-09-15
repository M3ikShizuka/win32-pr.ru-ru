---
description: Приложения используют методы интерфейса ID3DXFileSaveObject для записи файла. x на диск, а также для добавления и сохранения объектов и шаблонов данных.
ms.assetid: 1131c151-fa21-4654-9776-484922d58487
title: Интерфейс ID3DXFileSaveObject (D3DX9Xof. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ID3DXFileSaveObject
api_type:
- COM
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: f8d657c327c75045cf4feb2080a2e57d80f752df
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127567822"
---
# <a name="id3dxfilesaveobject-interface"></a>Интерфейс ID3DXFileSaveObject

Приложения используют методы интерфейса ID3DXFileSaveObject для записи файла. x на диск, а также для добавления и сохранения объектов и шаблонов данных.

## <a name="members"></a>Элементы

Интерфейс **ID3DXFileSaveObject** наследует от интерфейса [**IUnknown**](/windows/win32/api/unknwn/nn-unknwn-iunknown) . **ID3DXFileSaveObject** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **ID3DXFileSaveObject** содержит следующие методы.



| Метод                                                      | Описание                                                                                                                  |
|:------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------|
| [**адддатаобжект**](id3dxfilesaveobject--adddataobject.md) | Добавляет объект данных в качестве дочернего элемента для объекта [**ID3DXFileSaveData**](id3dxfilesavedata.md) .<br/>                       |
| [**Файл.**](id3dxfilesaveobject--getfile.md)             | Возвращает интерфейс [**ID3DXFile**](id3dxfile.md) объекта, который создал этот объект **ID3DXFileSaveObject** .<br/> |
| [**Сохранить**](id3dxfilesaveobject--save.md)                   | Сохраняет объект данных и его дочерние элементы в файл. x на диске.<br/>                                                        |



 

## <a name="remarks"></a>Комментарии

Шаблоны не являются обязательными для каждого файла. Например, можно разместить все шаблоны в одном файле x, а не дублировать их в каждый файл. x.

Интерфейс ID3DXFileSaveObject получается путем вызова метода [**ID3DXFile:: креатесавеобжект**](id3dxfile--createsaveobject.md) .

Глобальный уникальный идентификатор (GUID) для интерфейса ID3DXFileSaveObject — IID \_ ID3DXFileSaveObject.

Тип LPD3DXFILESAVEOBJECT определяется как указатель на этот интерфейс.


```
typedef interface ID3DXFileSaveObject *LPD3DXFILESAVEOBJECT;
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX9Xof. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>  |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Файловые интерфейсы D3DX X](dx9-graphics-reference-d3dx-x-file-interfaces.md)
</dt> </dl>

 

 
