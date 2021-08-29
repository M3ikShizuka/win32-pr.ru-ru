---
title: Недопустимый тип ресурса D1106
ms.assetid: 79a618cb-1d05-4895-b801-7663890b456a
description: Данный ресурс имеет тип, отличный от ожидаемого.
keywords:
- Недопустимый тип ресурса D1106 Direct2D
topic_type:
- apiref
api_name:
- D1106 Resource Is Wrong Type
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.custom: seodec18
ms.openlocfilehash: 1bbfd6d58eeb155002fbf5e7dbe243bd8d942ddaf4fa7d7715c6211523015476
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119911194"
---
# <a name="d1106-resource-is-wrong-type"></a>D1106: недопустимый тип ресурса

Указанный ресурс ресурса \[  \] не имеет ожидаемого типа.

## <a name="placeholders"></a>Заполнители

<dl> <dt>

<span id="resource"></span><span id="RESOURCE"></span>*ресурсов*
</dt> <dd>

Адрес ресурса.

</dd> </dl> 




 

## <a name="possible-causes"></a>Возможные причины

Интерфейс был неправильно приведен и использован в качестве параметра для метода или функции.

## <a name="examples"></a>Примеры

В следующем примере объект [**ID2D1SolidColorBrush**](/windows/win32/api/d2d1/nn-d2d1-id2d1solidcolorbrush) передается, когда ожидается [**ID2D1Geometry**](/windows/win32/api/d2d1/nn-d2d1-id2d1geometry) .


```C++
        m_pRenderTarget->FillGeometry(
            (ID2D1Geometry*)m_pYellowGreenBrush,
            m_pYellowGreenBrush
            );
```



В этом примере создается следующее сообщение отладки:

``` syntax
DEBUG ERROR - The given resource[003A2C98] is not of an expected type
```

## <a name="fixes"></a>Исправления

Используйте тип, требуемый для метода.

 

 
