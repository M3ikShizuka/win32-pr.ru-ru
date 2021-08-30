---
description: Дополнительные сведения о функции Жетосснапшотжетфризеинфо
title: Функция Жетосснапшотжетфризеинфо
TOCTitle: JetOSSnapshotGetFreezeInfo Function
ms:assetid: b94eaf91-7407-4c62-ab1e-3249ad076c1a
ms:mtpsurl: https://msdn.microsoft.com/library/Gg294070(v=EXCHG.10)
ms:contentKeyID: 32765685
ms.date: 04/11/2016
ms.topic: reference
api_name:
- JetOSSnapshotGetFreezeInfo
- JetOSSnapshotGetFreezeInfoA
- JetOSSnapshotGetFreezeInfoW
topic_type:
- apiref
- kbArticle
api_type:
- COM
- DLLExport
api_location:
- ESENT.DLL
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 56f2c5b4a7bcd2d81c75f90d723a59057ba5c8ce
ms.sourcegitcommit: 4665ebce0c106bdb52eef36e544280b496b6f50b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122982377"
---
# <a name="jetossnapshotgetfreezeinfo-function"></a>Функция Жетосснапшотжетфризеинфо


_**Применимо к:** Windows | Windows Сервером_

## <a name="jetossnapshotgetfreezeinfo-function"></a>Функция Жетосснапшотжетфризеинфо

Функция **жетосснапшотжетфризеинфо** извлекает список экземпляров и баз данных, которые являются частью сеанса моментального снимка, в любой момент времени.

**Windows vista:****жетосснапшотжетфризеинфо** появился в Windows Vista.  

```cpp
    JET_ERR JET_API JetOSSnapshotGetFreezeInfo(
      __in          const JET_OSSNAPID snapId,
      __out         unsigned long* pcInstanceInfo,
      __out         JET_INSTANCE_INFO** paInstanceInfo,
      __in          const JET_GRBIT grbit
    );
```

### <a name="parameters"></a>Параметры

*снапид*

Идентификатор сеанса моментального снимка, который необходимо запустить.

*пЦинстанцеинфо*

Количество выполняющихся в данный момент экземпляров, которые являются частью сеанса моментального снимка.

*паинстанцеинфо*

Массив структур, по одному для каждого выполняющегося экземпляра, описывающих экземпляр и базы данных, которые являются его частью.

*грбит*

Параметры для этого вызова. Этот параметр зарезервирован для использования в будущем. Единственное допустимое значение — 0 (ноль).

### <a name="return-value"></a>Возвращаемое значение

Эта функция возвращает [JET_ERR](./jet-err.md) DataType с одним из следующих кодов возврата. дополнительные сведения о возможных ошибках подсистемы ESE см. в разделе [ошибки расширенных служба хранилища Engine](./extensible-storage-engine-errors.md) и [параметры обработки ошибок](./error-handling-parameters.md).


| <p>Код возврата</p> | <p>Описание</p> | 
|--------------------|--------------------|
| <p>JET_errSuccess</p> | <p>Операция выполнена успешно.</p> | 
| <p>JET_errOutOfMemory</p> | <p>Ошибка при выполнении функции из-за нехватки памяти.</p> | 
| <p>JET_errInvalidParameter</p> | <p><em>пЦинстанцеинфо</em> или <em>Паинстанцеинфо</em> имеет <strong>значение NULL</strong>.</p> | 
| <p>JET_errOSSnapshotInvalidSnapId</p> | <p>Недопустимый идентификатор сеанса моментального снимка.</p> | 
| <p>JET_errOSSnapshotInvalidSequence</p> | <p>Сеанс моментального снимка не выполняется.</p> | 



Если эта функция выполнена успешно, сведения об экземпляре должны быть заполнены правильно, и их необходимо освободить позже путем вызова [жетфрибуффер](./jetfreebuffer-function.md) с указателем на возвращаемый массив сведений об экземпляре.

Если эта функция завершается неудачно, изменение состояния модуля не происходит.

#### <a name="requirements"></a>Требования


| Требование | Применение |
|------------|----------|
| <p><strong>Клиент</strong></p> | <p>требуется Windows Vista.</p> | 
| <p><strong>Server</strong></p> | <p>требуется Windows Server 2008.</p> | 
| <p><strong>Header</strong></p> | <p>Объявлено в ESENT. h.</p> | 
| <p><strong>Библиотека</strong></p> | <p>Используйте ESENT. lib.</p> | 
| <p><strong>КОМПОНОВКИ</strong></p> | <p>Требуется ESENT.dll.</p> | 
| <p><strong>Юникод</strong></p> | <p>Реализуется как <strong>жетосснапшотжетфризеинфов</strong> (Юникод) и <strong>жетосснапшотжетфризеинфоа</strong> (ANSI).</p> | 



#### <a name="see-also"></a>См. также:

[Параметры обработки ошибок](./error-handling-parameters.md)  
[ошибки расширенного обработчика служба хранилища](./extensible-storage-engine-errors.md)  
[JET_ERR](./jet-err.md)  
[жетфрибуффер](./jetfreebuffer-function.md)  
[жетосснапшотаборт](./jetossnapshotabort-function.md)  
[жетосснапшотфризе](./jetossnapshotfreeze-function.md)  
[жетосснапшотсав](./jetossnapshotthaw-function.md)
