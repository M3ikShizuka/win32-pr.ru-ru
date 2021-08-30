---
description: Свойство Модулекэйс только для чтения объекта Error возвращает указатель на коллекцию строк, содержащую первичные ключи строки в модуле, вызвавшей ошибку, по одному ключу на запись в коллекции.
ms.assetid: b02b609b-4682-4228-b29a-364f079e863c
title: Ошибка. свойство Модулекэйс (Мержемод. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Error.ModuleKeys
- IMsmError.get_ModuleKeys
api_type:
- COM
api_location:
- Mergemod.dll
ms.openlocfilehash: 9d33b546bea909700cc1a737043947d980006764daa86771820740570adf7f80
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120044604"
---
# <a name="errormodulekeys-property"></a>Ошибка. Модулекэйс, свойство

Свойство **модулекэйс** только для чтения объекта [**Error**](error-object.md) возвращает указатель на коллекцию строк, содержащую первичные ключи строки в модуле, вызвавшей ошибку, по одному ключу на запись в коллекции.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```JScript
propVal = Error.ModuleKeys
```



## <a name="property-value"></a>Значение свойства

## <a name="remarks"></a>Remarks

Клиент несет ответственность за освобождение коллекции строк, когда она больше не нужна.

Если значения не применяются к типу ошибки, коллекция пуста. Тип ошибки можно определить, вызвав свойство [**Type**](error-type.md) объекта [**Error**](error-object.md) .

### <a name="c"></a>C++

См. раздел [**Получение функции \_ модулекэйс**](/windows/win32/api/mergemod/nf-mergemod-imsmerror-get_modulekeys) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Версия<br/> | Mergemod.dll 1,0 или более поздней версии<br/>                                                    |
| Заголовок<br/>  | <dl> <dt>Мержемод. h</dt> </dl>   |
| DLL<br/>     | <dl> <dt>Mergemod.dll</dt> </dl> |



 

