---
description: Свойство Датабасекэйс только для чтения объекта Error Возвращает коллекцию строк, содержащую первичные ключи строки базы данных, вызвавшей ошибку. В коллекции имеется один ключ для каждой записи.
ms.assetid: 416a6cef-4c70-4c06-a8d2-801c9440e25a
title: Ошибка. свойство Датабасекэйс (Мержемод. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Error.DatabaseKeys
- IMsmError.get_DatabaseKeys
api_type:
- COM
api_location:
- Mergemod.dll
ms.openlocfilehash: c0de387c0101e7b79e64486089abcbd49f5d60d9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127141621"
---
# <a name="errordatabasekeys-property"></a>Ошибка. Датабасекэйс, свойство

Свойство **датабасекэйс** только для чтения объекта [**Error**](error-object.md) Возвращает коллекцию строк, содержащую первичные ключи строки базы данных, вызвавшей ошибку. В коллекции имеется один ключ для каждой записи.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Error.DatabaseKeys
```



## <a name="property-value"></a>Значение свойства

## <a name="remarks"></a>Remarks

Клиент несет ответственность за освобождение коллекции строк, когда она больше не нужна.

Если значения не применяются к типу ошибки, коллекция пуста. Тип ошибки можно определить, вызвав свойство [**Type**](error-type.md) объекта [**Error**](error-object.md) .

### <a name="c"></a>C++

См. раздел [**Получение функции \_ датабасекэйс**](/windows/win32/api/mergemod/nf-mergemod-imsmerror-get_databasekeys) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Версия<br/> | Mergemod.dll 1,0 или более поздней версии<br/>                                                    |
| Заголовок<br/>  | <dl> <dt>Мержемод. h</dt> </dl>   |
| DLL<br/>     | <dl> <dt>Mergemod.dll</dt> </dl> |



 

