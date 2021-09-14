---
description: Метод Екстрактфилесекс объекта Merge извлекает внедренный файл .cab из модуля, а затем записывает эти файлы в целевой каталог.
ms.assetid: 8b063052-4f92-466a-9c52-bda26ed13d5c
title: Метод Merge. Екстрактфилесекс (Мержемод. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Merge.ExtractFilesEx
- IMsmMerge.ExtractFilesEx
api_type:
- COM
api_location:
- Mergemod.dll
ms.openlocfilehash: be6aa1001be0d3ecd6cbb9c4cd1d8c04b4649f10
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127067849"
---
# <a name="mergeextractfilesex-method"></a>Метод Merge. Екстрактфилесекс

Метод **екстрактфилесекс** объекта [**Merge**](merge-object.md) извлекает внедренный файл .cab из модуля, а затем записывает эти файлы в целевой каталог.

## <a name="syntax"></a>Синтаксис


```JScript
Merge.ExtractFilesEx(
  Path,
  fLongFileNames,
  pFilePaths
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Путь* 
</dt> <dd>

Полный каталог назначения.

</dd> <dt>

*флонгфиленамес* 
</dt> <dd>

Задайте, чтобы указать использование длинных имен файлов для сегментов пути и окончательных имен файлов.

</dd> <dt>

*пфилепасс* 
</dt> <dd>

Это список полных путей для файлов, которые были успешно извлечены.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Все файлы в целевом каталоге с тем же именем перезаписываются. Если путь еще не существует, он создается.

### <a name="c"></a>C++

См. раздел Функция [**екстрактфилесекс**](/windows/desktop/api/Mergemod/nf-mergemod-imsmmerge2-extractfilesex) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Версия<br/> | Mergemod.dll 2,0 или более поздней версии<br/>                                                    |
| Заголовок<br/>  | <dl> <dt>Мержемод. h</dt> </dl>   |
| DLL<br/>     | <dl> <dt>Mergemod.dll</dt> </dl> |



 

 




