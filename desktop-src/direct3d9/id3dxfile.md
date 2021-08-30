---
description: Приложения используют методы интерфейса ID3DXFile для создания экземпляров интерфейсов ID3DXFileEnumObject и ID3DXFileSaveObject, а также для регистрации шаблонов.
ms.assetid: 472d45b1-5c03-4417-a005-91f802667919
title: Интерфейс ID3DXFile (D3DX9Xof. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ID3DXFile
api_type:
- COM
api_location:
- d3dx9.lib
- d3dx9.dll
ms.openlocfilehash: 8abbfaf93250f6c80888d82b291f4294d893703a383552fbef94d50c6fc57f1e
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119893354"
---
# <a name="id3dxfile-interface"></a>Интерфейс ID3DXFile

Приложения используют методы интерфейса ID3DXFile для создания экземпляров интерфейсов [**ID3DXFileEnumObject**](id3dxfileenumobject.md) и [**ID3DXFileSaveObject**](id3dxfilesaveobject.md) , а также для регистрации шаблонов.

## <a name="members"></a>Элементы

Интерфейс **ID3DXFile** наследует от интерфейса [**IUnknown**](/windows/win32/api/unknwn/nn-unknwn-iunknown) . **ID3DXFile** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **ID3DXFile** содержит следующие методы.



| Метод                                                            | Описание                                                                                                            |
|:------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------|
| [**креатинумобжект**](id3dxfile--createenumobject.md)           | Создает объект перечислителя, который будет считывать x-файл.<br/>                                                      |
| [**креатесавеобжект**](id3dxfile--createsaveobject.md)           | Создает объект Save, который будет использоваться для сохранения данных в файл. x.<br/>                                          |
| [**регистеренумтемплатес**](id3dxfile--registerenumtemplates.md) | Регистрирует пользовательские шаблоны при наличии объекта перечисления [**ID3DXFileEnumObject**](id3dxfileenumobject.md) .<br/> |
| [**регистертемплатес**](id3dxfile--registertemplates.md)         | Регистрирует пользовательские шаблоны.<br/>                                                                                 |



 

## <a name="remarks"></a>Remarks

Объект ID3DXFile также содержит локальное хранилище шаблонов. Это локальное хранилище может быть добавлено только с методами [**ID3DXFile:: регистеренумтемплатес**](id3dxfile--registerenumtemplates.md) и [**ID3DXFile:: регистертемплатес**](id3dxfile--registertemplates.md) .

Объекты [**ID3DXFileEnumObject**](id3dxfileenumobject.md) и [**ID3DXFileSaveObject**](id3dxfilesaveobject.md) , созданные с помощью [**ID3DXFile:: Креатинумобжект**](id3dxfile--createenumobject.md) и [**ID3DXFile:: креатесавеобжект**](id3dxfile--createsaveobject.md) , также используют хранилище шаблонов родительского объекта ID3DXFile.

Интерфейс ID3DXFile получается путем вызова функции [**D3DXFileCreate**](d3dxfilecreate.md) .

Глобальный уникальный идентификатор (GUID) для интерфейса ID3DXFile — IID \_ ID3DXFile.

Тип LPD3DXFILE определяется как указатель на интерфейс ID3DXFile.


```
typedef interface ID3DXFile *LPD3DXFILE;
```



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>D3DX9Xof. h</dt> </dl> |
| Библиотека<br/> | <dl> <dt>D3dx9. lib</dt> </dl>  |



## <a name="see-also"></a>См. также

<dl> <dt>

[Файловые интерфейсы D3DX X](dx9-graphics-reference-d3dx-x-file-interfaces.md)
</dt> </dl>

 

 
