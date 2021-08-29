---
description: Свойство примеры CursorType задает или получает текущий тип курсора.
ms.assetid: f362e790-a7c7-4fb6-86f3-7cd25f78fe0e
title: Примеры CursorType, свойство
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7fdbe34f2f400c9dd291201fd4a81a032ef2cd7f16adde98df8583b6c052a4f2
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120053124"
---
# <a name="cursortype-property"></a>Примеры CursorType, свойство

> [!Note]  
> этот компонент доступен для использования в операционных системах Microsoft Windows 2000, Windows XP и Windows Server 2003. В последующих версиях он может быть изменен или недоступен.

 

`CursorType`Свойство задает или получает текущий тип курсора.

``` syntax
[ iCursorType = ] MSWebDVD.CursorType
```

## <a name="return-value"></a>Возвращаемое значение

Возвращает целочисленное значение, представляющее тип курсора.

## <a name="remarks"></a>Remarks

Возможные значения этого свойства:



| Значение | Описание |
|-------|-------------|
| 0     | Стрелка       |
| 1     | Увеличить     |
| 2     | Уменьшить    |
| 3     | Правый        |
| –1    | Нет        |



 

Это свойство доступно для чтения и записи и имеет нулевое значение по умолчанию. Когда изображение масштабируется, параметр `CursorType` " **рука** " (0x3) переводит приложение в режим перетаскивания, позволяя пользователю перемещать изображение в область экрана.

 

 



