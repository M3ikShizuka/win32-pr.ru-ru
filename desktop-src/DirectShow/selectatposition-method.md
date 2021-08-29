---
description: Метод Селектатпоситион выбирает кнопку меню с заданными координатами указателя мыши.
ms.assetid: 005ec550-e04c-4dae-aa5d-d79afefe48ed
title: Метод Селектатпоситион
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e83cd45bc0d0a532531658a7cd55b6b1fa9a450726f1a00cf358c2db44b3e5f2
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119072658"
---
# <a name="selectatposition-method"></a>Метод Селектатпоситион

> [!Note]  
> этот компонент доступен для использования в операционных системах Microsoft Windows 2000, Windows XP и Windows Server 2003. В последующих версиях он может быть изменен или недоступен.

 

`SelectAtPosition`Метод выбирает кнопку меню с заданными координатами указателя мыши.

``` syntax
MSWebDVD.SelectAtPosition(xPos, yPos)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="xPos"></span><span id="xpos"></span><span id="XPOS"></span>*кспос*
</dt> <dd>

Задает координату x в виде целого числа.

</dd> <dt>

<span id="yPos"></span><span id="ypos"></span><span id="YPOS"></span>*ипос*
</dt> <dd>

Задает координату y в виде целого числа.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Remarks

Используйте этот метод при реализации пользовательской обработки мыши после установки для [**дисаблеаутомаусепроцессинг**](disableautomouseprocessing-property.md) значения **true**.

При выборе команды просто выделяется кнопка. Чтобы отправить команду, связанную с выбранной кнопкой, вызовите [**активатебуттон**](activatebutton-method.md).

## <a name="see-also"></a>См. также

<dl> <dt>

[**буттонсаваилабле**](buttonsavailable-property.md)
</dt> <dt>

[**куррентбуттон**](currentbutton-property.md)
</dt> <dt>

[**жетбуттонатпоситион**](getbuttonatposition-method.md)
</dt> <dt>

[**жетбуттонрект**](getbuttonrect-method.md)
</dt> <dt>

[**селектандактиватебуттон**](selectandactivatebutton-method.md)
</dt> </dl>

 

 



