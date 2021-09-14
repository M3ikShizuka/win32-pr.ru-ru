---
description: Метод Екстрактфилес объекта Merge извлекает внедренный файл .cab из модуля, а затем записывает эти файлы в целевой каталог.
ms.assetid: 846355d6-32f2-4b04-91dc-acd60445fbd9
title: Метод Merge. Екстрактфилес (Адвпуб. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Merge.ExtractFiles
- IMsmMerge.ExtractFiles
api_type:
- COM
api_location:
- Mergemod.dll
ms.openlocfilehash: 3869dc37b841d386891eb70940054bd78805bf94
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065364"
---
# <a name="mergeextractfiles-method"></a>Метод Merge. Екстрактфилес

Метод **екстрактфилес** объекта [**Merge**](merge-object.md) извлекает внедренный файл .cab из модуля, а затем записывает эти файлы в целевой каталог.

## <a name="syntax"></a>Синтаксис


```JScript
Merge.ExtractFiles(
  Path
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Путь* 
</dt> <dd>

Полный каталог назначения.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Все файлы в целевом каталоге с тем же именем перезаписываются. Если путь еще не существует, он создается.

**Екстрактфилес** всегда извлекает файлы, используя короткие имена файлов для пути. Чтобы использовать длинные имена файлов для пути, используйте [**метод екстрактфилесекс**](merge-extractfilesex.md).

### <a name="c"></a>C++

См. раздел Функция [**екстрактфилес**](/windows/win32/api/mergemod/nf-mergemod-imsmmerge-extractfiles) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|----------------------------------------------------------------------------------------------------------|
| Версия<br/> | Mergemod.dll 1,0 или более поздней версии<br/>                                                                     |
| Заголовок<br/>  | <dl> <dt>Адвпуб. h (включение Мержемод. h)</dt> </dl> |
| DLL<br/>     | <dl> <dt>Mergemod.dll</dt> </dl>                  |



 

 
