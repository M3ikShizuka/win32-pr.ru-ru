---
description: Дополнительные сведения о функции Жетресетсессионконтекст
title: Функция Жетресетсессионконтекст
TOCTitle: JetResetSessionContext Function
ms:assetid: 537a4753-b804-457a-9a13-53e8d1056eab
ms:mtpsurl: https://msdn.microsoft.com/library/Gg269250(v=EXCHG.10)
ms:contentKeyID: 32765552
ms.date: 04/11/2016
ms.topic: reference
api_name:
- JetResetSessionContext
topic_type:
- apiref
- kbArticle
api_type:
- DLLExport
- COM
api_location:
- ESENT.DLL
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 9a58b4085c5879af8f161ed78455250e30833978
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126962765"
---
# <a name="jetresetsessioncontext-function"></a>Функция Жетресетсессионконтекст


_**Применимо к:** Windows | Windows Сервером_

## <a name="jetresetsessioncontext-function"></a>Функция Жетресетсессионконтекст

Функция **жетресетсессионконтекст** отменяет связь между сеансом и текущим потоком.

```cpp
    JET_ERR JET_API JetResetSessionContext(
      __in          JET_SESID sesid
    );
```

### <a name="parameters"></a>Параметры

*сесид*

Сеанс, используемый для этого вызова.

### <a name="return-value"></a>Возвращаемое значение

Эта функция возвращает [JET_ERR](./jet-err.md) DataType с одним из следующих кодов возврата. дополнительные сведения о возможных ошибках подсистемы ESE см. в разделе [ошибки расширенных служба хранилища Engine](./extensible-storage-engine-errors.md) и [параметры обработки ошибок](./error-handling-parameters.md).


| <p>Код возврата</p> | <p>Описание</p> | 
|--------------------|--------------------|
| <p>JET_errSuccess</p> | <p>Операция выполнена успешно.</p> | 
| <p>JET_errInstanceUnavailable</p> | <p>Невозможно выполнить операцию, поскольку экземпляр, связанный с сеансом, обнаружил неустранимую ошибку, которая требует, чтобы доступ ко всем данным был отозван для защиты целостности этих данных.</p><p>эта ошибка будет возвращена только Windows XP и более поздних выпусках.</p> | 
| <p>JET_errNotInitialized</p> | <p>Невозможно выполнить операцию, так как экземпляр, связанный с сеансом, еще не инициализирован.</p> | 
| <p>JET_errRestoreInProgress</p> | <p>Невозможно выполнить операцию, так как в экземпляре, связанном с сеансом, выполняется операция восстановления.</p> | 
| <p>JET_errSessionContextNotSetByThisThread</p> | <p>Не удалось разосопоставить сеанс с текущим потоком, так как он связан с другим потоком.</p> | 
| <p>JET_errTermInProgress</p> | <p>Невозможно выполнить операцию, так как выполняется завершение работы экземпляра, связанного с сеансом.</p> | 



При успешном выполнении сеанс будет несвязанным с текущим потоком. Изменение состояния базы данных не выполняется.

В случае сбоя состояние сеанса останется неизменным. Изменение состояния базы данных не выполняется.

#### <a name="remarks"></a>Комментарии

**Жетресетсессионконтекст** должен вызываться в том же потоке, который вызвал [жетсетсессионконтекст](./jetsetsessioncontext-function.md) для данного сеанса.

#### <a name="requirements"></a>Требования


| Требование | Значение |
|------------|----------|
| <p><strong>Клиент</strong></p> | <p>требуется Windows Vista, Windows XP или Windows 2000 Professional.</p> | 
| <p><strong>Server</strong></p> | <p>требуется Windows server 2008, Windows server 2003 или сервер Windows 2000.</p> | 
| <p><strong>Header</strong></p> | <p>Объявлено в ESENT. h.</p> | 
| <p><strong>Библиотека</strong></p> | <p>Используйте ESENT. lib.</p> | 
| <p><strong>DLL</strong></p> | <p>Требуется ESENT.dll.</p> | 



#### <a name="see-also"></a>См. также:

[JET_API_PTR](./jet-api-ptr.md)  
[JET_ERR](./jet-err.md)  
[JET_SESID](./jet-sesid.md)  
[жетсетсессионконтекст](./jetsetsessioncontext-function.md)
