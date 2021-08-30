---
description: 'Дополнительные сведения: структура JET_RSTINFO'
title: Структура JET_RSTINFO
TOCTitle: JET_RSTINFO Structure
ms:assetid: 2f144d68-dcd9-4d0d-9d9e-a7d2a5c350fe
ms:mtpsurl: https://msdn.microsoft.com/library/Gg269216(v=EXCHG.10)
ms:contentKeyID: 32765519
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
ms.openlocfilehash: 05e2a96eba5be3e9d10ac167e122c12f3d08d885
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122478460"
---
# <a name="jet_rstinfo-structure"></a>Структура JET_RSTINFO


_**Применимо к:** Windows | Windows Сервером_

## <a name="jet_rstinfo-structure"></a>Структура JET_RSTINFO

Структура **JET_RSTINFO** содержит управляющие данные для процесса восстановления, такие как сведения о перерасположении базы данных, а также возможность управления остановкой восстановления.

**Windows Vista:** структура **JET_RSTINFO** появилась в Windows Vista.

```cpp
    typedef struct {
      unsigned long cbStruct;
      JET_RSTMAP* rgrstmap;
      long crstmap;
      JET_LGPOS lgposStop;
      JET_LOGTIME logtimeStop;
      JET_PFNSTATUS pfnStatus;
    } JET_RSTINFO;
```

### <a name="members"></a>Элементы

**кбструкт**

Размер структуры.

**ргрстмап**

Структура, описывающая старый и новый пути к восстановленной базе данных.

**крстмап**

Число записей массива в ргрстмап.

**лгпосстоп**

Позиция журнала для отмены восстановления в. Отмена не будет выполнена.

**логтиместоп**

Зарезервировано для последующего использования.

**пфнстатус**

Функция состояния для создания отчета о состоянии восстановления.

### <a name="requirements"></a>Требования


| | | <p><strong>Клиент</strong></p> | <p>требуется Windows Vista, Windows XP или Windows 2000 Professional.</p> | | <p><strong>Сервер</strong></p> | <p>требуется Windows server 2008, Windows server 2003 или сервер Windows 2000.</p> | | <p><strong>Header</strong></p> | <p>Объявлено в ESENT. h.</p> | | <p><strong>Юникод</strong></p> | <p>Реализуется как <strong>JET_RSTINFO_W</strong> (Юникод) и <strong>JET_RSTINFO_A</strong> (ANSI).</p> | 



### <a name="see-also"></a>См. также:

[JetInit3](./jetinit3-function.md)
