---
title: Controls. Аудиолангуажекаунт
description: Свойство Аудиолангуажекаунт извлекает количество поддерживаемых аудио языков.
ms.assetid: a6dda8bf-db8c-4e97-9277-5a23dfa93156
keywords:
- controls. аудиолангуажекаунт проигрыватель Windows Media
topic_type:
- apiref
api_name:
- Controls.audioLanguageCount
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8e4bb89c9e9af4218daf1491b53c59f252d50931995da3df9d5f84ef8e8481b6
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118997563"
---
# <a name="controlsaudiolanguagecount"></a>Controls. Аудиолангуажекаунт

Свойство **аудиолангуажекаунт** извлекает количество поддерживаемых аудио языков.

``` syntax
player.controls.audioLanguageCount
      
```

## <a name="possible-values"></a>Возможные значения

Это свойство является **числом** только для чтения (**длинное целое**).

## <a name="remarks"></a>Remarks

для Windows содержимого на основе носителя свойства и методы, связанные с выбором языка, поддерживают только один выход.

**проигрыватель Windows Media 10 Mobile:** Это свойство всегда возвращает значение 1.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии.<br/>                                 |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект Controls**](controls-object.md)
</dt> <dt>

[**Controls. Куррентаудиолангуаже**](controls-currentaudiolanguage.md)
</dt> <dt>

[**Controls. Куррентаудиолангуажеиндекс**](controls-currentaudiolanguageindex.md)
</dt> <dt>

[**Controls. Жетаудиолангуажедескриптион**](controls-getaudiolanguagedescription.md)
</dt> <dt>

[**Controls. Жетаудиолангуажеид**](controls-getaudiolanguageid.md)
</dt> <dt>

[**Controls. Жетлангуаженаме**](controls-getlanguagename.md)
</dt> </dl>

 

 





