---
description: Дополнительные сведения о функции Жетресизедатабасе
title: Функция Жетресизедатабасе
TOCTitle: JetResizeDatabase Function
ms:assetid: b6420de7-acff-480e-838b-f0e5acc29c65
ms:mtpsurl: https://msdn.microsoft.com/library/JJ835047(v=EXCHG.10)
ms:contentKeyID: 49894669
ms.date: 04/11/2016
ms.topic: reference
dev_langs:
- c++
api_name:
- JetResizeDatabase
topic_type:
- apiref
- kbArticle
api_type:
- DLLExport
api_location:
- ESENT.DLL
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: f12fc06b915f5462c9209416cf54436ef3d7239b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126962761"
---
# <a name="jetresizedatabase-function"></a>Функция Жетресизедатабасе


_**Применимо к:** Windows | Windows Сервером_

Функция **жетресизедатабасе** расширяет или сжимает размер открытой в данный момент базы данных.

функция **жетресизедатабасе** была введена в операционной системе Windows 8.

``` c++
JET_ERR JET_API JetResizeDatabase(
  __in          JET_SESID sesid,
  __in          JET_DBID dbid,
  __in          unsigned long cpg,
  __out         unsigned long* pcpgActual,
  __in          const JET_GRBIT grbit
);
```

### <a name="parameters"></a>Параметры

*сесид*

Контекст сеанса базы данных, используемый для вызова API.

*DBID*

База данных, которая будет расширена.

*CPG*

Запрошенный размер базы данных на страницах.

*пкпгактуал*

Указатель на число, которое получает размер базы данных на страницах после вызова API. В случае сбоя вызова API содержимое параметра *пкпгактуал* не определено.

*грбит*

Группа битов, которая указывает ноль или более значений, перечисленных в следующей таблице.


| <p>Значение</p> | <p>Значение</p> | 
|--------------|----------------|
| <p>JET_bitResizeDatabaseOnlyGrow</p> | <p>Увеличивать только базу данных. Если при вызове изменения размера база данных будет сжата, ничего делать не нужно.</p> | 



### <a name="return-value"></a>Возвращаемое значение

Эта функция возвращает [JET_ERR](./jet-err.md) DataType с одним из кодов возврата, перечисленных в следующей таблице. дополнительные сведения о служба хранилища возможных ошибках ESE см. в разделе [ошибки расширяемых](./extensible-storage-engine-errors.md) подсистемы служба хранилища и [параметры обработки ошибок](./error-handling-parameters.md).


| <p>Код возврата</p> | <p>Описание</p> | 
|--------------------|--------------------|
| <p>JET_errSuccess</p> | <p>Операция выполнена успешно.</p> | 
| <p>JET_errDiskFull</p> | <p>Недостаточно свободного места на томе для выполнения операции увеличения.</p> | 
| <p>JET_errDiskIO</p> | <p>Функция <a href="gg269242(v=exchg.10).md">жетсетдатабасесизе</a> вернула ошибку, связанную с файлом. Дополнительные сведения о других ошибках, связанных с файлами, которые могут быть возвращены, см. в разделе <a href="gg269242(v=exchg.10).md">жетсетдатабасесизе</a>.</p> | 



#### <a name="remarks"></a>Комментарии

Если функция **жетресизедатабасе** вызывается до вставки больших объемов данных, файл базы данных будет увеличен за одну операцию. Это снизит вероятность того, что файл базы данных станет фрагментированным на уровне файловой системы, а также сократит число попыток увеличения размера файла базы данных. Увеличение файла базы данных выполняется один раз быстрее, чем в несколько раз.

Сведения о том, как задать размер открытой базы данных, см. в разделе [жетсетдатабасесизе](./jetsetdatabasesize-function.md).

Размер файла может не совпадать с количеством страниц, возвращаемых в параметре *пкпгреал* . В параметре *пкпгреал* могут не учитываться две дополнительные зарезервированные страницы.

#### <a name="requirements"></a>Требования


| Требование | Значение |
|------------|----------|
| <p><strong>Клиент</strong></p> | <p>Требуется Windows 8.</p> | 
| <p><strong>Server</strong></p> | <p>Требуется Windows Server 2012.</p> | 
| <p><strong>Header</strong></p> | <p>Объявлено в ESENT. h.</p> | 
| <p><strong>Библиотека</strong></p> | <p>Используйте ESENT. lib.</p> | 
| <p><strong>DLL</strong></p> | <p>Требуется ESENT.dll.</p> | 



#### <a name="see-also"></a>См. также:

[JET_ERR](./jet-err.md)  
[JET_GRBIT](./jet-grbit.md)  
[JET_SESID](./jet-sesid.md)  
[JET_TABLEID](./jet-tableid.md)  
[JET_OBJECTINFO](./jet-objectinfo-structure.md)  
[JET_OBJECTLIST](./jet-objectlist-structure.md)  
[жетсетдатабасесизе](./jetsetdatabasesize-function.md)
