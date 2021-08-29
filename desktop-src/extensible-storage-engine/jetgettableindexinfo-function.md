---
description: Дополнительные сведения о функции Жетжеттаблеиндексинфо
title: Функция JetGetTableIndexInfo
TOCTitle: JetGetTableIndexInfo Function
ms:assetid: d250d254-2b10-4fe7-bbb1-72bb967f22dd
ms:mtpsurl: https://msdn.microsoft.com/library/Gg294102(v=EXCHG.10)
ms:contentKeyID: 32765717
ms.date: 04/11/2016
ms.topic: reference
api_name:
- JetGetTableIndexInfoW
- JetGetTableIndexInfoA
- JetGetTableIndexInfo
topic_type:
- apiref
- kbArticle
api_type:
- COM
- DLLExport
api_location:
- ESENT.DLL
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 9cde923ea822ed3bf62dcb5e7cdc65447ce60347
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122477560"
---
# <a name="jetgettableindexinfo-function"></a>Функция JetGetTableIndexInfo


_**Применимо к:** Windows | Windows Сервером_

## <a name="jetgettableindexinfo-function"></a>Функция JetGetTableIndexInfo

Функция **жетжеттаблеиндексинфо** получает сведения о индексе.

```cpp
    JET_ERR JET_API JetGetTableIndexInfo(
      __in          JET_SESID sesid,
      __in          JET_TABLEID tableid,
      __in          const tchar* szIndexName,
      __out         void* pvResult,
      __in          unsigned long cbResult,
      __in          unsigned long InfoLevel
    );
```

### <a name="parameters"></a>Параметры

*сесид*

Контекст сеанса базы данных, используемый для вызова API.

*TableID*

Таблица базы данных, содержащая индекс, в котором содержатся необходимые сведения.

*сзиндекснаме*

Имя индекса, содержащего сведения, которые будут получены.

*пвресулт*

Указатель на буфер, который будет принимать сведения. Буфер должен быть согласован, чтобы вместить требуемый тип. Тип буфера зависит от параметра *инфолевел* .

*кбресулт*

Размер буфера (в байтах), переданного в параметре *пвресулт* .

*инфолевел*

Указывает, какие сведения будут храниться в *пвресулт*. Допустимые значения:


| <p>Значение</p> | <p>Значение</p> | 
|--------------|----------------|
| <p>JET_IdxInfo</p> | <p><em>пвресулт</em> интерпретируется как структура <a href="gg269185(v=exchg.10).md">JET_INDEXLIST</a> . При успешном выполнении структура <a href="gg269185(v=exchg.10).md">JET_INDEXLIST</a> получает сведения об индексе. При сбое содержимое <em>пвбуффер</em> не определено.</p> | 
| <p>JET_IdxInfoLCID</p> | <p><em>пвресулт</em> интерпретируется как LCID. При успешном выполнении код LCID содержит идентификатор локали индекса. При сбое содержимое <em>пвбуффер</em> не определено.</p> | 
| <p>JET_IdxInfoList</p> | <p><em>пвресулт</em> интерпретируется как структура <a href="gg269185(v=exchg.10).md">JET_INDEXLIST</a> . При успешном выполнении структура <a href="gg269185(v=exchg.10).md">JET_INDEXLIST</a> получает сведения об индексе. При сбое содержимое <em>пвбуффер</em> не определено.</p> | 
| <p>JET_IdxInfoOLC</p> | <p>JET_IdxInfoOLC устарел.</p> | 
| <p>JET_IdxInfoResetOLC</p> | <p>JET_IdxInfoResetOLC устарел.</p> | 
| <p>JET_IdxInfoSpaceAlloc</p> | <p><em>пвресулт</em> интерпретируется как ULong. При успешном выполнении в ULONG содержится место использования индекса. При сбое содержимое <em>пвбуффер</em> не определено.</p> | 
| <p>JET_IdxInfoSysTabCursor</p> | <p>JET_IdxInfoSysTabCursor устарел.</p> | 
| <p>JET_IdxInfoLangid</p> | <p>JET_IdxInfoLangid не рекомендуется к использованию. Вместо этого используйте JET_IdxInfoLCID и макрос <a href="/windows/win32/api/winnt/nf-winnt-langidfromlcid">лангидфромлЦид</a> .</p> | 
| <p>JET_IdxInfoCount</p> | <p><em>пвресулт</em> интерпретируется как ULong. В случае успеха ULONG содержит количество индексов в указанной таблице. <em>сзиндекснаме</em> игнорируется. При сбое содержимое <em>пвбуффер</em> не определено.</p> | 
| <p>JET_IdxInfoVarSegMac</p> | <p><em>пвресулт</em> интерпретируется как ushort. При успешном выполнении объект USHORT содержит значение <em>кбварсегмак</em> , используемое при создании индекса. Описание <em>кбварсегмак</em>см. в разделе <a href="gg269186(v=exchg.10).md">JET_INDEXCREATE</a> . При сбое содержимое <em>пвбуффер</em> не определено.</p> | 
| <p>JET_IdxInfoIndexId</p> | <p><em>пвресулт</em> интерпретируется как <a href="gg269327(v=exchg.10).md">JET_INDEXID</a>. При успешном выполнении структура <a href="gg269327(v=exchg.10).md">JET_INDEXID</a> получает сведения об индексе. При сбое содержимое <em>пвбуффер</em> не определено.</p> | 
| <p>JET_IdxInfoKeyMost</p> | <p><em>пвресулт</em> интерпретируется как ushort. При успешном выполнении объект USHORT содержит значение Кбкэймост, используемое при создании индекса. Описание Кбкэймост см. в разделе Структура <a href="gg269186(v=exchg.10).md">JET_INDEXCREATE</a> . При сбое содержимое <em>пвбуффер</em> не определено.</p> | 
| <p>JET_IdxInfoCreateIndex</p> | <p><em>пвресулт</em> интерпретируется как структура <a href="gg269186(v=exchg.10).md">JET_INDEXCREATE</a> . При сбое содержимое <em>пвбуффер</em> не определено.</p><p><strong>Windows 7:</strong> JET_IdxInfoCreateIndex представлен в Windows 7.</p> | 
| <p>JET_IdxInfoCreateIndex2</p> | <p><em>пвресулт</em> интерпретируется как структура <a href="gg294082(v=exchg.10).md">JET_INDEXCREATE2</a> . При сбое содержимое <em>пвбуффер</em> не определено.</p><p><strong>Windows 7:</strong> JET_IdxInfoCreateIndex2 представлен в Windows 7.</p> | 



### <a name="return-value"></a>Возвращаемое значение

Эта функция возвращает [JET_ERR](./jet-err.md) DataType с одним из следующих кодов возврата. дополнительные сведения о возможных ошибках подсистемы ESE см. в разделе [ошибки расширенных служба хранилища Engine](./extensible-storage-engine-errors.md) и [параметры обработки ошибок](./error-handling-parameters.md).


| <p>Код возврата</p> | <p>Описание</p> | 
|--------------------|--------------------|
| <p>JET_errSuccess</p> | <p>Операция выполнена успешно.</p> | 
| <p>JET_errIndexNotFound</p> | <p>Указанный индекс не найден в указанной таблице.</p> | 
| <p>JET_wrnBufferTruncated</p> | <p>Буфер, переданный как <em>пвресулт</em> , слишком мал. Содержимое буфера не определено.</p> | 



#### <a name="remarks"></a>Комментарии

[Жетжетиндексинфо](./jetgetindexinfo-function.md) и **жетжеттаблеиндексинфо** извлекают идентичные сведения о индексе. Разница заключается в том, как указана таблица. [Жетжетиндексинфо](./jetgetindexinfo-function.md) ждет базу данных (*DBID*) и имя таблицы (*сзтабленаме*), а **жетжеттаблеиндексинфо** — идентификатор таблицы (*TableID*).

#### <a name="requirements"></a>Требования


| | | <p><strong>Клиент</strong></p> | <p>требуется Windows Vista, Windows XP или Windows 2000 Professional.</p> | | <p><strong>Сервер</strong></p> | <p>требуется Windows server 2008, Windows server 2003 или сервер Windows 2000.</p> | | <p><strong>Header</strong></p> | <p>Объявлено в ESENT. h.</p> | | <p><strong>Библиотека</strong></p> | <p>Используйте ESENT. lib.</p> | | <p><strong>КОМПОНОВКИ</strong></p> | <p>Требуется ESENT.dll.</p> | | <p><strong>Юникод</strong></p> | <p>Реализуется как <strong>жетжеттаблеиндексинфов</strong> (Юникод) и <strong>жетжеттаблеиндексинфоа</strong> (ANSI).</p> | 



#### <a name="see-also"></a>См. также:

[JET_COLUMNID](./jet-columnid.md)  
[JET_ERR](./jet-err.md)  
[JET_GRBIT](./jet-grbit.md)  
[JET_SESID](./jet-sesid.md)  
[JET_TABLEID](./jet-tableid.md)  
[JET_INDEXCREATE](./jet-indexcreate-structure.md)  
[JET_INDEXID](./jet-indexid-structure.md)  
[жетжетиндексинфо](./jetgetindexinfo-function.md)
