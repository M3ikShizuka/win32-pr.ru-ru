---
description: Метод Екстракткаб объекта Merge извлекает внедренный файл .cab из модуля и сохраняет его как указанный файл. Установщик создаст этот файл, если он еще не существует, и перезаписал его, если он существует.
ms.assetid: a6fe8b69-8f4a-45f7-b7e6-7620a00500bb
title: Метод Merge. Екстракткаб (Мержемод. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Merge.ExtractCAB
- IMsmMerge.ExtractCAB
api_type:
- COM
api_location:
- Mergemod.dll
ms.openlocfilehash: e14f1163c16d7b12ea223baa533f3953cd22d88ec6e3cc617f5ffe72adb5075c
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119926634"
---
# <a name="mergeextractcab-method"></a>Метод Merge. Екстракткаб

Метод **екстракткаб** объекта [**Merge**](merge-object.md) извлекает внедренный файл .cab из модуля и сохраняет его как указанный файл. Установщик создаст этот файл, если он еще не существует, и перезаписал его, если он существует.

## <a name="syntax"></a>Синтаксис


```JScript
Merge.ExtractCAB(
  FileName
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*FileName* 
</dt> <dd>

Полный файл назначения.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="c"></a>C++

См. раздел Функция [**екстракткаб**](/windows/win32/api/mergemod/nf-mergemod-imsmmerge-extractcab) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Версия<br/> | Mergemod.dll 1,0 или более поздней версии<br/>                                                    |
| Заголовок<br/>  | <dl> <dt>Мержемод. h</dt> </dl>   |
| DLL<br/>     | <dl> <dt>Mergemod.dll</dt> </dl> |



 

 
