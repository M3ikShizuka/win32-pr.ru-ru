---
description: Свойство Дефаултаудиолангуажеекст извлекает расширение языка DVD-звука по умолчанию.
ms.assetid: 628af2aa-e528-4689-953b-558e13e1d513
title: Дефаултаудиолангуажеекст, свойство
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 03423e6dda19563b55845662f7af5b21df00802726b279068a40c847aa6fc5e2
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118953113"
---
# <a name="defaultaudiolanguageext-property"></a>Дефаултаудиолангуажеекст, свойство

> [!Note]  
> этот компонент доступен для использования в операционных системах Microsoft Windows 2000, Windows XP и Windows Server 2003. В последующих версиях он может быть изменен или недоступен.

 

`DefaultAudioLanguageExt`Свойство получает расширение языка DVD-звука по умолчанию.

``` syntax
[ iLangExt = ] MSWebDVD.DefaultAudioLanguageExt
```

## <a name="return-value"></a>Возвращаемое значение

Возвращает целочисленное значение, указывающее расширение языка звука по умолчанию. Возможные значения см. в разделе Примечания.

## <a name="remarks"></a>Remarks

Это свойство доступно только для чтения и не имеет значения по умолчанию. В следующей таблице приведены возможные значения для расширений языка DVD Audio.



| Значение | Описание       |
|-------|-------------------|
| 0     | NotSpecified      |
| 1     | Субтитры          |
| 2     | висуаллимпаиред  |
| 3     | DirectorComments1 |
| 4     | DirectorComments2 |



 

 

 



