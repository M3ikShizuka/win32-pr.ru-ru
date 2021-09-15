---
description: Метод Опенлог объекта Merge открывает файл журнала, который получает сведения о ходе выполнения и сообщениях об ошибках. Если файл журнала уже существует, установщик добавляет новые сообщения. Если файл журнала не существует, установщик создает файл журнала.
ms.assetid: 97d01ea3-43b6-4529-9706-97b3b0132d9c
title: Метод Merge. Опенлог (Мержемод. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Merge.OpenLog
- IMsmMerge.OpenLog
api_type:
- COM
api_location:
- Mergemod.dll
ms.openlocfilehash: 46dc029c88b44540817e93e1e559829d88b9f62b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461936"
---
# <a name="mergeopenlog-method"></a>Метод Merge. Опенлог

Метод **опенлог** объекта [**Merge**](merge-object.md) открывает файл журнала, который получает сведения о ходе выполнения и сообщениях об ошибках. Если файл журнала уже существует, установщик добавляет новые сообщения. Если файл журнала не существует, установщик создает файл журнала.

## <a name="syntax"></a>Синтаксис


```JScript
Merge.OpenLog(
  Filename
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Имя файла* 
</dt> <dd>

Полное имя файла, указывающее на файл, который нужно открыть или создать.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Клиенты могут отправить свои сообщения в этот файл журнала с помощью метода [**log**](merge-log.md) .

### <a name="c"></a>C++

См. раздел Функция [**опенлог**](/windows/win32/api/mergemod/nf-mergemod-imsmmerge-openlog) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Версия<br/> | Mergemod.dll 1,0 или более поздней версии<br/>                                                    |
| Заголовок<br/>  | <dl> <dt>Мержемод. h</dt> </dl>   |
| DLL<br/>     | <dl> <dt>Mergemod.dll</dt> </dl> |



 

 
