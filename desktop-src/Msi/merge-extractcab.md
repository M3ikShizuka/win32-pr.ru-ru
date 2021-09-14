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
ms.openlocfilehash: d0bdc79fb0087456d035bf732faca384b35b2a9f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127067853"
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

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Версия<br/> | Mergemod.dll 1,0 или более поздней версии<br/>                                                    |
| Заголовок<br/>  | <dl> <dt>Мержемод. h</dt> </dl>   |
| DLL<br/>     | <dl> <dt>Mergemod.dll</dt> </dl> |



 

 
