---
description: 'Дополнительные сведения: структура JET_CONDITIONALCOLUMN'
title: Структура JET_CONDITIONALCOLUMN
TOCTitle: JET_CONDITIONALCOLUMN Structure
ms:assetid: 2ca6b4ba-0dc4-47d5-b072-324e5a381d0d
ms:mtpsurl: https://msdn.microsoft.com/library/Gg269214(v=EXCHG.10)
ms:contentKeyID: 32765517
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
ms.openlocfilehash: d7ca03c8c340c9c0b81ec46d0809f50a19e4d2f2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461120"
---
# <a name="jet_conditionalcolumn-structure"></a>Структура JET_CONDITIONALCOLUMN


_**Применимо к:** Windows | Windows Сервером_

## <a name="jet_conditionalcolumn-structure"></a>Структура JET_CONDITIONALCOLUMN

Структура **JET_CONDITIONALCOLUMN** определяет, как выполняется условное индексирование для данного индекса. Условный индекс содержит элемент индекса только для тех строк, которые соответствуют заданному условию. Однако условный столбец не является частью ключа индекса, он только управляет присутствием элемента индекса.

```cpp
    typedef struct tagJET_CONDITIONALCOLUMN {
      unsigned long cbStruct;
      tchar* szColumnName;
      JET_GRBIT grbit;
    } JET_CONDITIONALCOLUMN;
```

### <a name="members"></a>Элементы

**кбструкт**

Это поле должно быть инициализировано в sizeof (JET_CONDITIONALCOLUMN) в байтах.

**сзколумннаме**

Имя столбца, содержащего данные, на которых ядро СУБД выполняет условное индексирование строки.

**грбит** Группа битов, которая предоставляет параметры для условного индекса. Передача нулевых или логических значений (**или** ED) недопустима для **JET_CONDITIONALCOLUMN**. Битовое поле должно быть ровно одним из следующих:


| <p>Значение</p> | <p>Значение</p> | 
|--------------|----------------|
| <p>JET_bitIndexColumnMustBeNull</p> | <p>Столбец, указанный параметром <em>сзколумннаме</em> , должен иметь значение NULL для записи индекса, чтобы данная строка отображалась в этом индексе.</p> | 
| <p>JET_bitIndexColumnMustBeNonNull</p> | <p>Столбец, указанный параметром <em>сзколумннаме</em> , должен иметь значение, отличное от NULL, для записи индекса, чтобы данная строка отображалась в этом индексе.</p> | 



### <a name="remarks"></a>Remarks

Условный индекс содержит элемент индекса только для тех строк, которые соответствуют заданному условию. Например, столбец может называться "помечен", а если строка помечена, в столбце задается значение, отличное от NULL. В JET_bitIndexColumnMustBeNonNull условном индексе этого столбца будут показаны все отмеченные строки, а в условном индексе JET_bitIndexColumnMustBeNull будут показаны непомеченные строки. Это также удобный способ для удаления флагов и сбора мусора.

### <a name="requirements"></a>Требования


| Требование | Значение |
|------------|----------|
| <p><strong>Клиент</strong></p> | <p>требуется Windows Vista, Windows XP или Windows 2000 Professional.</p> | 
| <p><strong>Server</strong></p> | <p>требуется Windows server 2008, Windows server 2003 или сервер Windows 2000.</p> | 
| <p><strong>Header</strong></p> | <p>Объявлено в ESENT. h.</p> | 
| <p><strong>Юникод</strong></p> | <p>Реализуется как <strong>JET_CONDITIONALCOLUMN_W</strong> (Юникод) и <strong>JET_CONDITIONALCOLUMN_A</strong> (ANSI).</p> | 



### <a name="see-also"></a>См. также:

[JET_GRBIT](./jet-grbit.md)  
[JET_INDEXCREATE](./jet-indexcreate-structure.md)
