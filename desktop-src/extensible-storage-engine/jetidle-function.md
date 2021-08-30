---
description: Дополнительные сведения о функции Жетидле
title: Функция Жетидле
TOCTitle: JetIdle Function
ms:assetid: 77e036eb-b894-4ff7-b14f-1564bf21873f
ms:mtpsurl: https://msdn.microsoft.com/library/Gg269301(v=EXCHG.10)
ms:contentKeyID: 32765593
ms.date: 04/11/2016
ms.topic: reference
api_name:
- JetIdle
topic_type:
- apiref
- kbArticle
api_type:
- COM
- DLLExport
api_location:
- ESENT.DLL
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 73a1fa613bd5dda8d64572b376b0e1fa792e56fb
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122471370"
---
# <a name="jetidle-function"></a>Функция Жетидле


_**Применимо к:** Windows | Windows Сервером_

## <a name="jetidle-function"></a>Функция Жетидле

Функция **жетидле** уничтожена, и ее следует использовать только в целях тестирования. **Жетидле** можно использовать для выполнения задач очистки после простоя или для проверки состояния хранилища версий в ESE.

```cpp
    JET_ERR JET_API JetIdle(
      __in          JET_SESID sesid,
      __in          JET_GRBIT grbit
    );
```

### <a name="parameters"></a>Параметры

*сесид*

Сеанс, который будет использоваться для этого вызова.

*грбит*

Группа битов, содержащая параметры, которые должны использоваться для этого вызова, включая ноль или более следующих битов:


| <p>Значение</p> | <p>Значение</p> | 
|--------------|----------------|
| <p>JET_bitIdleCompact</p> | <p>Запускает очистку хранилища версий.</p> | 
| <p>JET_bitIdleFlushBuffers</p> | <p>Зарезервировано для последующего использования. Если этот флаг указан, API возвратит JET_errInvalidgrbit.</p> | 
| <p>JET_bitIdleStatus</p> | <p>Возвращает JET_wrnIdleFull, если хранилище версий больше половины места.</p> | 



### <a name="return-value"></a>Возвращаемое значение

Эта функция возвращает [JET_ERR](./jet-err.md) DataType с одним из следующих кодов возврата. дополнительные сведения о возможных ошибках подсистемы ESE см. в разделе [ошибки расширенных служба хранилища Engine](./extensible-storage-engine-errors.md) и [параметры обработки ошибок](./error-handling-parameters.md).


| <p>Код возврата</p> | <p>Описание</p> | 
|--------------------|--------------------|
| <p>JET_errSuccess</p> | <p>Операция выполнена успешно.</p> | 
| <p>JET_errInvalidParameter</p> | <p>Недопустимый параметр <em>грбит</em> , предоставленный API.</p> | 



Если эта функция завершится с ошибкой, будет активирована соответствующая операция или код ошибки, указывающий, насколько заполнено хранилище версий в зависимости от предоставленной *грбит* .

Если эта функция завершается ошибкой, запрошенная операция не будет выполнена успешно.

#### <a name="remarks"></a>Комментарии

Хранилище версий поддерживает механизм изоляции моментальных снимков ESE. Если хранилище версий больше половины, программа может закрыть долго выполняющиеся транзакции. Если долго выполняющаяся транзакция приводит к исчерпанию хранилища версий, ESE прекращает разрешение операций записи в базу данных.

#### <a name="requirements"></a>Требования


| | | <p><strong>Клиент</strong></p> | <p>требуется Windows Vista, Windows XP или Windows 2000 Professional.</p> | | <p><strong>Сервер</strong></p> | <p>требуется Windows server 2008, Windows server 2003 или сервер Windows 2000.</p> | | <p><strong>Header</strong></p> | <p>Объявлено в ESENT. h.</p> | | <p><strong>Библиотека</strong></p> | <p>Используйте ESENT. lib.</p> | | <p><strong>КОМПОНОВКИ</strong></p> | <p>Требуется ESENT.dll.</p> | 



#### <a name="see-also"></a>См. также:

[JET_ERR](./jet-err.md)  
[JET_GRBIT](./jet-grbit.md)  
[JET_SESID](./jet-sesid.md)  
[жеткоммиттрансактион](./jetcommittransaction-function.md)
