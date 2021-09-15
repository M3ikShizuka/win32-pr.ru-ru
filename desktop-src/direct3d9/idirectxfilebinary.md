---
description: Приложения используют методы интерфейса Идиректксфилебинари для чтения и извлечения информации о двоичных данных. Не рекомендуется.
ms.assetid: 43b20ab3-67b2-4717-ad90-0bf4ddb3207e
title: Интерфейс Идиректксфилебинари (Дксфиле. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IDirectXFileBinary
api_type:
- COM
api_location:
- d3dxof.lib
- d3dxof.dll
ms.openlocfilehash: b6707e4e685289f16b85ab85c2cce13dcd1da962
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458313"
---
# <a name="idirectxfilebinary-interface"></a>Интерфейс Идиректксфилебинари

Приложения используют методы интерфейса Идиректксфилебинари для чтения и извлечения информации о двоичных данных. Не рекомендуется.

## <a name="members"></a>Элементы

Интерфейс **идиректксфилебинари** наследует от [**идиректксфилеобжект**](idirectxfileobject.md). **Идиректксфилебинари** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **идиректксфилебинари** содержит следующие методы.



| Метод                                                 | Описание                                                                                                 |
|:-------------------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| [**жетмиметипе**](idirectxfilebinary--getmimetype.md) | Извлекает тип MIME для двоичных данных. Не рекомендуется.<br/> |
| [**GetSize**](idirectxfilebinary--getsize.md)         | Возвращает размер двоичных данных. Не рекомендуется.<br/>                                               |
| [**Просмотр**](idirectxfilebinary--read.md)               | Считывает двоичные данные. Не рекомендуется.<br/>                                                               |



 

## <a name="remarks"></a>Remarks

Идентификатор GUID для интерфейса Идиректксфилебинари — IID \_ идиректксфилебинари.

Тип Лпдиректксфилебинари определяется как указатель на этот интерфейс.


```
typedef interface IDirectXFileBinary *LPDIRECTXFILEBINARY;
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Дксфиле. h</dt> </dl>   |
| Библиотека<br/> | <dl> <dt>D3dxof. lib</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**идиректксфилеобжект**](idirectxfileobject.md)
</dt> <dt>

[Файловые интерфейсы X](dx9-graphics-reference-x-file-interfaces.md)
</dt> </dl>

 

 




