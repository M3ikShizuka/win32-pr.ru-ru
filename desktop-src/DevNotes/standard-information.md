---
description: Содержит стандартный атрибут сведений. Этот атрибут имеется в каждой записи базового файла и должен быть резидентным.
ms.assetid: 8e668309-2722-4115-923d-bf0aa78d24f1
title: Структура STANDARD_INFORMATION
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- STANDARD_INFORMATION
api_type:
- NA
api_location: ''
ms.openlocfilehash: d0ddba05eee5d822020cfbb2e4b30976bb3c7570e1613f457ee3fd373494e0da
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119984064"
---
# <a name="standard_information-structure"></a>Стандартная \_ информационная структура

\[Эта структура допустима только для томов NTFS версии 3; Он может быть изменен в будущих версиях.\]

Содержит стандартный атрибут сведений. Этот атрибут имеется в каждой записи базового файла и должен быть резидентным.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _STANDARD_INFORMATION {
  UCHAR Reserved[0x30];
  ULONG OwnerId;
  ULONG SecurityId;
} STANDARD_INFORMATION, *PSTANDARD_INFORMATION;
```



## <a name="members"></a>Члены

<dl> <dt>

**Reserved**
</dt> <dd>

Зарезервировано.

</dd> <dt>

**OwnerId**
</dt> <dd>

Идентификатор владельца файла из индекса безопасности.

</dd> <dt>

**секуритид**
</dt> <dd>

Идентификатор безопасности для файла.

</dd> </dl>

## <a name="remarks"></a>Remarks

Обратите внимание, что для этой структуры нет связанного файла заголовка.

Это определение структуры допустимо только для основной версии 3 и дополнительной версии 0 или 1, как сообщается [**фсктл \_ Получение \_ \_ \_ данных тома NTFS**](/windows/win32/api/winioctl/ni-winioctl-fsctl_get_ntfs_volume_data).

## <a name="see-also"></a>См. также

<dl> <dt>

[Основная таблица файлов](master-file-table.md)
</dt> </dl>

 

 
