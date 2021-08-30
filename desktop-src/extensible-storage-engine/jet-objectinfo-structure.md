---
description: 'Дополнительные сведения: структура JET_OBJECTINFO'
title: Структура JET_OBJECTINFO
TOCTitle: JET_OBJECTINFO Structure
ms:assetid: 9d348ab3-d453-4316-9233-681f165e8ef1
ms:mtpsurl: https://msdn.microsoft.com/library/Gg269353(v=EXCHG.10)
ms:contentKeyID: 32765640
ms.date: 04/11/2016
ms.topic: reference
api_name: ''
topic_type:
- apiref
- kbArticle
api_type:
- COM
api_location: ''
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: a24f27982285622e3b5f0893768757d27041f1c0
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122465111"
---
# <a name="jet_objectinfo-structure"></a>Структура JET_OBJECTINFO


_**Применимо к:** Windows | Windows Сервером_

## <a name="jet_objectinfo-structure"></a>Структура JET_OBJECTINFO

Структура **JET_OBJECTINFO** содержит сведения об объекте. В настоящее время поддерживаются только таблицы типов объектов.

```cpp
    typedef struct {
      unsigned long cbStruct;
      JET_OBJTYP objtyp;
      JET_DATESERIAL dtCreate;
      JET_DATESERIAL dtUpdate;
      JET_GRBIT grbit;
      unsigned long flags;
      unsigned long cRecord;
      unsigned long cPage;
    } JET_OBJECTINFO;
```

### <a name="members"></a>Элементы

**кбструкт**

Размер структуры **JET_OBJECTINFO** в байтах.

**обжтип**

Содержит [JET_OBJTYP](./jet-objtyp.md) структуры. В настоящее время возвращаются только таблицы (то есть JET_objtypTable).

**дткреате**

Является устаревшей. Не используйте.

**дтупдате**

Является устаревшей. Не используйте.

**грбит**

Группа битов, содержащая параметры, доступные для данного вызова, которые включают ноль или более следующих значений.


| <p>Значение</p> | <p>Значение</p> | 
|--------------|----------------|
| <p>JET_bitTableInfoBookmark</p> | <p>В таблице могут быть закладки.</p> | 
| <p>JET_bitTableInfoRollback</p> | <p>Можно выполнить откат таблицы.</p> | 
| <p>JET_bitTableInfoUpdatable</p> | <p>Таблицу можно обновить.</p> | 



**flags**

Битовое поле, которое содержит ноль или более следующих флагов.


| <p>Значение</p> | <p>Значение</p> | 
|--------------|----------------|
| <p>JET_bitObjectSystem</p> | <p>Таблица является системной таблицей и предназначена только для внутреннего использования.</p> | 
| <p>JET_bitObjectTableDerived</p> | <p>Таблица, унаследованная на языке DDL из таблицы шаблонов.</p> | 
| <p>JET_bitObjectTableFixedDDL</p> | <p>Невозможно изменить DDL для таблицы.</p> | 
| <p>JET_bitObjectTableNoFixedVarColumnsInDerivedTables</p> | <p>Используется в сочетании с JET_bitObjectTableTemplate для запрета фиксированных или переменных столбцов в производных таблицах (чтобы в будущем можно было добавить в шаблон фиксированные или переменные столбцы).</p><p><strong>Windows XP:</strong> это значение вводится в Windows XP.</p> | 
| <p>JET_bitObjectTableTemplate</p> | <p>Таблица является таблицей шаблонов.</p> | 



**крекорд**

Число записей в таблице.

Это значение извлекается, только если **JET_OBJECTINFO** был передан в [жетжетобжектинфо](./jetgetobjectinfo-function.md).

**кпаже**

Количество страниц, используемых таблицей.

Это значение извлекается, только если **JET_OBJECTINFO** был передан в [жетжетобжектинфо](./jetgetobjectinfo-function.md).

### <a name="remarks"></a>Комментарии

Структура **JET_OBJECTINFO** заполняется вызовом [жетжетобжектинфо](./jetgetobjectinfo-function.md) или [жетжеттаблеинфо](./jetgettableinfo-function.md). Если вызов API не выполняется, содержимое структуры не определено.

Если применимо, статистика таблицы включает количество записей и количество страниц в кластеризованном индексе (то есть индекс, содержащий данные записи). Доступ к статистике индекса осуществляется отдельно по имени с помощью [жетжетиндексинфо](./jetgetindexinfo-function.md) или [жетжеттаблеиндексинфо](./jetgettableindexinfo-function.md).

### <a name="requirements"></a>Требования


| | | <p><strong>Клиент</strong></p> | <p>требуется Windows Vista, Windows XP или Windows 2000 Professional.</p> | | <p><strong>Сервер</strong></p> | <p>требуется Windows server 2008, Windows server 2003 или сервер Windows 2000.</p> | | <p><strong>Header</strong></p> | <p>Объявлено в ESENT. h.</p> | 



### <a name="see-also"></a>См. также:

[JET_ERR](./jet-err.md)  
[JET_GRBIT](./jet-grbit.md)  
[JET_OBJTYP](./jet-objtyp.md)  
[JET_SESID](./jet-sesid.md)  
[JET_TABLEID](./jet-tableid.md)  
[жетжетиндексинфо](./jetgetindexinfo-function.md)  
[жетжетобжектинфо](./jetgetobjectinfo-function.md)  
[жетжеттаблеиндексинфо](./jetgettableindexinfo-function.md)  
[жетжеттаблеинфо](./jetgettableinfo-function.md)
