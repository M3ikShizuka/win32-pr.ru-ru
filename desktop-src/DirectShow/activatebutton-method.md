---
description: Метод Активатебуттон активирует выбранную кнопку меню.
ms.assetid: 1da486a0-dadc-4c92-b3d3-83aeace01e39
title: Метод Активатебуттон
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c8a463a3aad1ee0dcabc0e5daaa4a4969efa37aa
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127162407"
---
# <a name="activatebutton-method"></a>Метод Активатебуттон

> [!Note]  
> этот компонент доступен для использования в операционных системах Microsoft Windows 2000, Windows XP и Windows Server 2003. В последующих версиях он может быть изменен или недоступен.

 

Метод Активатебуттон активирует выбранную кнопку меню.

``` syntax
        MSWebDVD.ActivateButton()
```

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Комментарии

Используйте этот метод при реализации пользовательской обработки мыши после установки для [**дисаблеаутомаусепроцессинг**](disableautomouseprocessing-property.md) значения **true**.

Этот метод используется для активации кнопки, выбранной с помощью метода [**селектлефтбуттон**](selectleftbutton-method.md), [**селектловербуттон**](selectlowerbutton-method.md), [**селектуппербуттон**](selectupperbutton-method.md)или [**селектригхтбуттон**](selectrightbutton-method.md) .

 

 



