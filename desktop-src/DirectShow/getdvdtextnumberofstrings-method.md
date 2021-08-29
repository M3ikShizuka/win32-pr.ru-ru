---
description: Метод Жетдвдтекстнумберофстрингс извлекает количество текстовых строк, доступных для указанного языка.
ms.assetid: 84d2b5b7-b474-48a4-9058-ea9da8109398
title: Метод Жетдвдтекстнумберофстрингс
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5be6818d447ad244ec59be029f21119ef89024477edc7811de94372c3825fa25
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119537054"
---
# <a name="getdvdtextnumberofstrings-method"></a>Метод Жетдвдтекстнумберофстрингс

> [!Note]  
> этот компонент доступен для использования в операционных системах Microsoft Windows 2000, Windows XP и Windows Server 2003. В последующих версиях он может быть изменен или недоступен.

 

`GetDVDTextNumberOfStrings`Метод получает количество текстовых строк, доступных для указанного языка.

``` syntax
[ iStrings = ] MSWebDVD.GetDVDTextNumberOfStrings(iLangIndex)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="iLangIndex"></span><span id="ilangindex"></span><span id="ILANGINDEX"></span>*илангиндекс*
</dt> <dd>

Задает язык в виде целого числа. Значение должно находиться в диапазоне от нуля до значения, возвращенного [**жетдвдтекстнумберофлангуажес**](getdvdtextnumberoflanguages-method.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает целочисленное значение, указывающее, сколько строк содержит диск на указанном языке.

## <a name="see-also"></a>См. также

<dl> <dt>

[Объект Мсвебдвд](mswebdvd-object.md)
</dt> </dl>

 

 



