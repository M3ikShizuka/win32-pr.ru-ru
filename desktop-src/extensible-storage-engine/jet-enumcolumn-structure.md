---
description: 'Дополнительные сведения: структура JET_ENUMCOLUMN'
title: Структура JET_ENUMCOLUMN
TOCTitle: JET_ENUMCOLUMN Structure
ms:assetid: f8f512fd-5fcf-47ed-a5db-2fb3bd76c2d7
ms:mtpsurl: https://msdn.microsoft.com/library/Gg294138(v=EXCHG.10)
ms:contentKeyID: 32765752
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
ms.openlocfilehash: 4f27fd08cb9df4c9e777524b14c1dfbdfe274dab
ms.sourcegitcommit: 4665ebce0c106bdb52eef36e544280b496b6f50b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122988647"
---
# <a name="jet_enumcolumn-structure"></a>Структура JET_ENUMCOLUMN


_**Применимо к:** Windows | Windows Сервером_

## <a name="jet_enumcolumn-structure"></a>Структура JET_ENUMCOLUMN

Структура **JET_ENUMCOLUMN** перечисляет значения столбцов записи a при использовании функции [жетенумератеколумнс](./jetenumeratecolumns-function.md) . [Жетенумератеколумнс](./jetenumeratecolumns-function.md) возвращает массив структур **JET_ENUMCOLUMN** . Массив возвращается в памяти, выделенной с помощью обратного вызова, [перераспределения](/cpp/c-runtime-library/reference/realloc?view=vs-2019) которого было предоставлено этому API.

```cpp
    typedef struct {
      JET_COLUMNID columnid;
      JET_ERR err;
      union {
        struct {
          unsigned long cEnumColumnValue;
          JET_ENUMCOLUMNVALUE rgEnumColumnValue;
        };
        struct {
          unsigned long cbData;
          void* pvData;
        };
      };
    } JET_ENUMCOLUMN;
```

### <a name="members"></a>Элементы

**columnid**

Идентификатор столбца, который был перечислен.

**Err**

Код состояния столбца, полученный в результате перечисления столбца.


| <p>Коды ошибок</p> | <p>Значение</p> | 
|--------------------|----------------|
| <p>JET_errBadColumnId</p> | <p>Идентификатор столбца находится за пределами допустимых ограничений идентификатора столбца.</p> | 
| <p>JET_errColumnNotFound</p> | <p>Столбец, описываемый ИДЕНТИФИКАТОРом столбца, не существует в таблице.</p> | 
| <p>JET_wrnColumnNull</p> | <p>Все значения для этого столбца равны NULL.</p> | 
| <p>JET_wrnColumnPresent</p> | <p>Указан JET_bitEnumeratePresenceOnly, и для этого столбца было возвращено по крайней мере одно значение столбца, отличное от NULL.</p> | 
| <p>JET_wrnColumnSingleValue</p> | <p>Указан JET_bitEnumerateCompressOutput, и для этого столбца возвращено ровно одно значение столбца, отличное от NULL. В результате возвращается сжатая форма <strong>JET_ENUMCOLUMN</strong> . Дополнительные сведения см. в разделе <strong>JET_ENUMCOLUMN</strong> .</p> | 
| <p>JET_wrnColumnSkipped</p> | <p>Идентификатор столбца в структуре <a href="gg269251(v=exchg.10).md">JET_ENUMCOLUMNID</a> , соответствующей этой <strong>JET_ENUMCOLUMN</strong> структуре, равен нулю.</p> | 



**ценумколумнвалуе**

Массив значений столбца, перечисленных для столбца. Выходной буфер возвращается в память, которая была выделена с помощью обратного вызова, [перераспределения](/cpp/c-runtime-library/reference/realloc?view=vs-2019) которого было предоставлено в [жетенумератеколумнс](./jetenumeratecolumns-function.md).

Этот выходной буфер используется, когда код состояния столбца не равен JET_wrnColumnSingleValue. Дополнительные сведения см. в разделе [жетенумератеколумнс](./jetenumeratecolumns-function.md).

Возвращается, если "Err \! = JET_wrnColumnSingleValue".

**рженумколумнвалуе**

Массив значений столбца, перечисленных для столбца. Выходной буфер возвращается в память, которая была выделена с помощью обратного вызова, [перераспределения](/cpp/c-runtime-library/reference/realloc?view=vs-2019) которого было предоставлено в [жетенумератеколумнс](./jetenumeratecolumns-function.md).

Этот выходной буфер используется, когда код состояния столбца не равен JET_wrnColumnSingleValue. Дополнительные сведения см. в разделе [жетенумератеколумнс](./jetenumeratecolumns-function.md).

Возвращается, если "Err \! = JET_wrnColumnSingleValue".

**cbData**

Значение столбца, перечисленное для столбца.

Выходной буфер возвращается в память, которая была выделена с помощью обратного вызова, [перераспределения](/cpp/c-runtime-library/reference/realloc?view=vs-2019) которого было предоставлено в [жетенумератеколумнс](./jetenumeratecolumns-function.md).

Этот выходной буфер используется только в том случае, если код состояния столбца имеет значение JET_wrnColumnSingleValue. Дополнительные сведения см. в разделе [жетенумератеколумнс](./jetenumeratecolumns-function.md).

Возвращается, если "Err = = JET_wrnColumnSingleValue".

**пвдата**

Значение столбца, перечисленное для столбца.

Выходной буфер возвращается в память, которая была выделена с помощью обратного вызова, [перераспределения](/cpp/c-runtime-library/reference/realloc?view=vs-2019) которого было предоставлено в [жетенумератеколумнс](./jetenumeratecolumns-function.md).

Этот выходной буфер используется только в том случае, если код состояния столбца имеет значение JET_wrnColumnSingleValue. Дополнительные сведения см. в разделе [жетенумератеколумнс](./jetenumeratecolumns-function.md).

Возвращается, если "Err = = JET_wrnColumnSingleValue".

### <a name="requirements"></a>Требования


| Требование | Применение |
|------------|----------|
| <p><strong>Клиент</strong></p> | <p>требуется Windows Vista, Windows XP или Windows 2000 Professional.</p> | 
| <p><strong>Server</strong></p> | <p>требуется Windows server 2008, Windows server 2003 или сервер Windows 2000.</p> | 
| <p><strong>Header</strong></p> | <p>Объявлено в ESENT. h.</p> | 



### <a name="see-also"></a>См. также:

[JET_COLUMNID](./jet-columnid.md)  
[JET_ERR](./jet-err.md)  
[JET_ENUMCOLUMNID](./jet-enumcolumnid-structure.md)  
[JET_ENUMCOLUMNVALUE](./jet-enumcolumnvalue-structure.md)  
[жетенумератеколумнс](./jetenumeratecolumns-function.md)  
[realloc](/cpp/c-runtime-library/reference/realloc?view=vs-2019)
