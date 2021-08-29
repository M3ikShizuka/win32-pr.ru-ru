---
title: Controls. Куррентаудиолангуажеиндекс
description: Свойство Куррентаудиолангуажеиндекс указывает или получает Отсчитываемый от единицы индекс, соответствующий звуковому языку для воспроизведения.
ms.assetid: 9a1ae887-4e64-4758-a8a2-bf2e10a7a5c7
keywords:
- controls. куррентаудиолангуажеиндекс проигрыватель Windows Media
topic_type:
- apiref
api_name:
- Controls.currentAudioLanguageIndex
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e783d42b957df40320b7c26814f7f05e93b94030518f45dc4b40d76f9ed32bba
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119763874"
---
# <a name="controlscurrentaudiolanguageindex"></a>Controls. Куррентаудиолангуажеиндекс

Свойство **куррентаудиолангуажеиндекс** указывает или получает Отсчитываемый от единицы индекс, соответствующий звуковому языку для воспроизведения.

``` syntax
player.controls.currentAudioLanguageIndex
      
```

## <a name="possible-values"></a>Возможные значения

Это свойство имеет **номер** для чтения и записи (**Long**).

## <a name="remarks"></a>Remarks

для Windows содержимого на основе носителя свойства и методы, связанные с выбором языка, поддерживают только один выход.

Используйте свойство **аудиолангуажекаунт** , чтобы получить количество поддерживаемых аудио языков.

**проигрыватель Windows Media 10 Mobile:** Это свойство принимает или возвращает значение 0.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии.<br/>                                 |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Объект Controls**](controls-object.md)
</dt> <dt>

[**Controls. Аудиолангуажекаунт**](controls-audiolanguagecount.md)
</dt> <dt>

[**Controls. Куррентаудиолангуаже**](controls-currentaudiolanguage.md)
</dt> <dt>

[**Controls. Жетаудиолангуажедескриптион**](controls-getaudiolanguagedescription.md)
</dt> <dt>

[**Controls. Жетаудиолангуажеид**](controls-getaudiolanguageid.md)
</dt> <dt>

[**Controls. Жетлангуаженаме**](controls-getlanguagename.md)
</dt> </dl>

 

 





