---
description: Метод Сетклипвидеорект позволяет увеличить изображение экрана до указанного подпрямоугольника.
ms.assetid: 3940a382-8d53-4ff9-b024-38de1aa00f54
title: Метод Сетклипвидеорект
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4ff7f4b003ef20b82f1e783ebf074e8bbd5cc793
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053858"
---
# <a name="setclipvideorect-method"></a>Метод Сетклипвидеорект

> [!Note]  
> этот компонент доступен для использования в операционных системах Microsoft Windows 2000, Windows XP и Windows Server 2003. В последующих версиях он может быть изменен или недоступен.

 

`SetClipVideoRect`Метод позволяет увеличить изображение экрана до указанного подпрямоугольника.

``` syntax
MSWebDVD.SetClipVideoRect(oRect)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="oRect"></span><span id="orect"></span><span id="ORECT"></span>*орект*
</dt> <dd>

Задает объект [двдрект](dvdrect-object.md) , который содержит прямоугольник обрезки.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Нет возвращаемого значения.

## <a name="remarks"></a>Комментарии

При установке нового прямоугольника обрезки объект увеличивает эту область в соответствии с общими отображаемыми размерами приложения. Это приведет к уменьшению масштаба в определенной области экрана. Чтобы указать прямоугольник, создайте новый объект [двдрект](dvdrect-object.md) и заполните его свойства.

Наиболее распространенный прямоугольник для экрана видео — 720 x 540.

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**жетклипвидеорект**](getclipvideorect-method.md)
</dt> </dl>

 

 



