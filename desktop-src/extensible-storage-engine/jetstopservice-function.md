---
description: Дополнительные сведения о функции Жетстопсервице
title: Функция JetStopService
TOCTitle: JetStopService Function
ms:assetid: 46aeb9ed-ee72-49cc-99e3-791a51a55b02
ms:mtpsurl: https://msdn.microsoft.com/library/Gg269240(v=EXCHG.10)
ms:contentKeyID: 32765542
ms.date: 04/11/2016
ms.topic: reference
api_name:
- JetStopService
topic_type:
- apiref
- kbArticle
api_type:
- COM
- DLLExport
api_location:
- ESENT.DLL
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 314750e8a01ea58e2d29ee7c2bd9ca29564f107c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127575039"
---
# <a name="jetstopservice-function"></a>Функция JetStopService


_**Применимо к:** Windows | Windows Сервером_

## <a name="jetstopservice-function"></a>Функция JetStopService

Функция **жетстопсервице** готовит экземпляр к завершению.

**Жетстопсервице** — это устаревший вызов, если разрешен только один экземпляр. В этом случае единственным активным экземпляром является тот, который подготавливается к завершению.

```cpp
    JET_ERR JET_API JetStopService(void);
```

### <a name="parameters"></a>Параметры

У этой функции нет параметров.

### <a name="return-value"></a>Возвращаемое значение

Эта функция возвращает [JET_ERR](./jet-err.md) DataType с одним из следующих кодов возврата. дополнительные сведения о возможных ошибках подсистемы ESE см. в разделе [ошибки расширенных служба хранилища Engine](./extensible-storage-engine-errors.md) и [параметры обработки ошибок](./error-handling-parameters.md).


| <p>Код возврата</p> | <p>Описание</p> | 
|--------------------|--------------------|
| <p>JET_errSuccess</p> | <p>Операция выполнена успешно.</p> | 
| <p>JET_errRunningInMultiInstanceMode</p> | <p>Не ясно, какой экземпляр подготавливается к завершению при использовании <strong>жетстопсервице</strong> в режиме с несколькими экземплярами.</p><p><strong>Windows XP:</strong>  это возвращаемое значение вводится в Windows XP.</p> | 



Если эта функция выполнена, она подготавливается к будущему завершению. Ниже приведены шаги, предпринимаемые для подготовки к завершению работы.

  - Останавливает оперативную дефрагментацию, если она запущена.

  - Запуск очистки хранилища версий.

  - Уменьшите глубину контрольной точки, начав с очистки «грязных» страниц в диспетчере буферов.

  - Предотвращение будущих вызовов большинства функций для этого экземпляра.

Если эта функция завершается ошибкой, не будет выполнен ни один из шагов подготовки к завершению работы экземпляра, поэтому изменение состояния экземпляра не выполняется.

#### <a name="remarks"></a>Комментарии

Эта функция сокращает работу, которую экземпляр будет выполнять при завершении, но не будет завершать экземпляр. В результате эта функция является просто оптимизацией и не является обязательной для использования. обратите внимание, что объем работы, выполненной в процессе подготовки, был меньше в Windows 2000 и Windows XP. После выполнения функции вызов функций, которые больше не разрешены, возвратит JET_errClientRequestToStopJetService. Функции, по-прежнему разрешенные после этого вызова: [жетроллбакк](./jetrollback-function.md), [жетклосетабле](./jetclosetable-function.md), [жетендсессион](./jetendsession-function.md), [жетклоседатабасе](./jetclosedatabase-function.md), [жетдетачдатабасе](./jetdetachdatabase-function.md) и [жетресетсессионконтекст](./jetresetsessioncontext-function.md).

#### <a name="requirements"></a>Требования


| Требование | Значение |
|------------|----------|
| <p><strong>Клиент</strong></p> | <p>требуется Windows Vista, Windows XP или Windows 2000 Professional.</p> | 
| <p><strong>Server</strong></p> | <p>требуется Windows server 2008, Windows server 2003 или сервер Windows 2000.</p> | 
| <p><strong>Header</strong></p> | <p>Объявлено в ESENT. h.</p> | 
| <p><strong>Библиотека</strong></p> | <p>Используйте ESENT. lib.</p> | 
| <p><strong>DLL</strong></p> | <p>Требуется ESENT.dll.</p> | 



#### <a name="see-also"></a>См. также:

[JET_ERR](./jet-err.md)  
[JET_INSTANCE](./jet-instance.md)  
[жетклоседатабасе](./jetclosedatabase-function.md)  
[жетклосетабле](./jetclosetable-function.md)  
[жетдетачдатабасе](./jetdetachdatabase-function.md)  
[жетендсессион](./jetendsession-function.md)  
[жетресетсессионконтекст](./jetresetsessioncontext-function.md)  
[жетроллбакк](./jetrollback-function.md)  
[жеттерм](./jetterm-function.md)  
[JetTerm2](./jetterm2-function.md)
