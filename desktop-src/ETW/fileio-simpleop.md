---
description: Этот класс является классом типа события для простых событий файловых операций. Следующий синтаксис упрощен из MOF-кода.
ms.assetid: 5b6374e0-b39a-4d5a-acbd-25b410f1ba52
title: Класс FileIo_SimpleOp
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- FileIo_SimpleOp
- FileIo_SimpleOp.IrpPtr
- FileIo_SimpleOp.TTID
- FileIo_SimpleOp.FileObject
- FileIo_SimpleOp.FileKey
api_type:
- NA
api_location: ''
ms.openlocfilehash: f7ff09830653278c9b37cfefa81b182b0f1dc054
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127470377"
---
# <a name="fileio_simpleop-class"></a>\_Класс FileIo симплеоп

Этот класс является классом типа события для простых событий файловых операций.

Следующий синтаксис упрощен из MOF-кода.

## <a name="syntax"></a>Синтаксис

``` syntax
[EventType{65, 66, 73}, EventTypeName{"Cleanup", "Close", "Flush"}]
class FileIo_SimpleOp : FileIo
{
  uint32 IrpPtr;
  uint32 TTID;
  uint32 FileObject;
  uint32 FileKey;
};
```

## <a name="members"></a>Участники

Класс **FileIo \_ симплеоп** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Класс **FileIo \_ симплеоп** имеет следующие свойства.

<dl> <dt>

**филекэй**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: Вмидатаид (4), Pointer
</dt> </dl>

Чтобы определить имя файла, сопоставьте значение этого свойства со свойством **FileObject** события [**FileIo \_ Name**](fileio-name.md) .

</dd> <dt>

**Закрыт**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: Вмидатаид (3), Pointer
</dt> </dl>

Идентификатор, который можно использовать для сопоставления операций с одним и тем же открытым экземпляром объекта File между событиями создания и закрытия файла.

</dd> <dt>

**ирпптр**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: Вмидатаид (1), Pointer
</dt> </dl>

Пакет запроса ввода-вывода. Это свойство определяет действие ввода-вывода.

</dd> <dt>

**ттид**
</dt> <dd> <dl> <dt>

Тип данных: **UInt32**
</dt> <dt>

Тип доступа: только для чтения
</dt> <dt>

Квалификаторы: Вмидатаид (2), Pointer
</dt> </dl>

Идентификатор потока, выполняющего операцию.

</dd> </dl>

## <a name="remarks"></a>Remarks

Событие очистки регистрируется при закрытии последнего маркера файла. Событие закрытия указывает, что файловый объект освобождается. Событие Flush указывает, когда буферы файлов полностью сброшены на диск.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>       |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**FileIo**](fileio.md)
</dt> </dl>

 

 




