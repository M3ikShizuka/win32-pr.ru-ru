---
description: Image_V0_Load класс. Этот класс является классом типа события для событий загрузки изображения. Следующий синтаксис упрощен из MOF-кода.
ms.assetid: e2836153-8e4f-4c7f-9542-9402ed9e4356
title: Класс Image_V0_Load
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Image_V0_Load
- Image_V0_Load.BaseAddress
- Image_V0_Load.ModuleSize
- Image_V0_Load.ImageFileName
api_type:
- NA
api_location: ''
ms.openlocfilehash: 006dc57aefdec374a85167580280b171d852172bf45bf979b76948a5014f1c24
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119070184"
---
# <a name="image_v0_load-class"></a>Image \_ v0 \_ Load, класс

Этот класс является классом типа событий для событий загрузки изображения.

Следующий синтаксис упрощен из MOF-кода.

## <a name="syntax"></a>Синтаксис

``` syntax
[EventType(10), EventTypeName("Load")]
class Image_V0_Load
{
  uint32 BaseAddress;
  uint32 ModuleSize;
  string ImageFileName;
};
```

## <a name="members"></a>Члены

Класс **image \_ v0 \_ Load** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **image \_ v0 \_ Load** имеет следующие свойства.

<dl> <dt>

BaseAddress
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: Вмидатаид (1), Pointer
</dt> </dl>

Базовый адрес приложения, в котором загружается образ.

</dd> <dt>

имажефиленаме
</dt> <dd> <dl> <dt>

Тип данных: **строка**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: Вмидатаид (3), Стрингтерминатион ("NullTerminated"), Format ("w")
</dt> </dl>

Имя и расширение файла DLL или исполняемого образа для загрузки.

</dd> <dt>

модулесизе
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: Вмидатаид (2)
</dt> </dl>

Размер изображения.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/> |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>       |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_V0 изображения**](image-v0.md)
</dt> </dl>

 

 




