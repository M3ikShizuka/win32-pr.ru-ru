---
description: 'Дополнительные сведения: структура JET_SETSYSPARAM'
title: Структура JET_SETSYSPARAM
TOCTitle: JET_SETSYSPARAM Structure
ms:assetid: 3c0fdd28-99bd-4026-b64b-6859ef9dc91b
ms:mtpsurl: https://msdn.microsoft.com/library/Gg269230(v=EXCHG.10)
ms:contentKeyID: 32765532
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
ms.openlocfilehash: 7309d803421d4bf9221ba1d968d5034f940b016f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126962813"
---
# <a name="jet_setsysparam-structure"></a>Структура JET_SETSYSPARAM


_**Применимо к:** Windows | Windows Сервером_

## <a name="jet_setsysparam-structure"></a>Структура JET_SETSYSPARAM

Массив структур **JET_SETSYSPARAM** указывает конкретный набор глобальных системных параметров, которые задаются в качестве аргумента при использовании функции [жетенаблемултиинстанце](./jetenablemultiinstance-function.md) .

**Windows XP:** эта структура появилась в Windows XP.

```cpp
    typedef struct {
      unsigned long paramid;
      JET_API_PTR lParam;
      const tchar* sz;
      JET_ERR err;
    } JET_SETSYSPARAM;
```

### <a name="members"></a>Элементы

**paramid**

Идентификатор системного параметра, который будет установлен.

полный список системных параметров и их свойств см. в разделе [расширенные параметры системы служба хранилища Engine](./extensible-storage-engine-system-parameters.md) .

**lParam**

Необязательное значение, устанавливаемое для выбранного системного параметра, если этот системный параметр имеет целочисленный тип.

**SZ**

Необязательное значение, устанавливаемое для выбранного системного параметра, если этот системный параметр имеет строковый тип.

**Err**

Ошибка, полученная в результате вызова метода [жетсетсистемпараметер](./jetsetsystemparameter-function.md) с указанными ранее параметрами.

### <a name="requirements"></a>Требования


| Требование | Значение |
|------------|----------|
| <p><strong>Клиент</strong></p> | <p>требуется Windows Vista, Windows XP или Windows 2000 Professional.</p> | 
| <p><strong>Server</strong></p> | <p>требуется Windows server 2008, Windows server 2003 или сервер Windows 2000.</p> | 
| <p><strong>Header</strong></p> | <p>Объявлено в ESENT. h.</p> | 
| <p><strong>Юникод</strong></p> | <p>Реализуется как <strong>JET_ SETSYSPARAM_W</strong> (Юникод) и <strong>JET_ SETSYSPARAM_A</strong> (ANSI).</p> | 



### <a name="see-also"></a>См. также:

[расширяемые параметры системы служба хранилища Engine](./extensible-storage-engine-system-parameters.md)  
[JET_API_PTR](./jet-api-ptr.md)  
[JET_ERR](./jet-err.md)  
[жетенаблемултиинстанце](./jetenablemultiinstance-function.md)  
[жетсетсистемпараметер](./jetsetsystemparameter-function.md)
