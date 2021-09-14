---
title: Каунтеритем. Линестиле, свойство
description: Возвращает или задает стиль линии, используемый для отображения значения счетчика.
ms.assetid: 5801f0f8-37e5-4b15-a13f-24c71fea550d
keywords:
- Сисмон свойство Линестиле
- Линестиле Property Сисмон, класс Каунтеритем
- Класс Каунтеритем Сисмон, свойство Линестиле
topic_type:
- apiref
api_name:
- CounterItem.LineStyle
api_location:
- Sysmon.ocx
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: bbff1dd78c6fd65d72c28fe8f13f7bbf5603c75f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056840"
---
# <a name="counteritemlinestyle-property"></a>Каунтеритем. Линестиле, свойство

Возвращает или задает стиль линии, используемый для отображения значения счетчика.

Это свойство доступно для чтения и записи.

## <a name="syntax"></a>Синтаксис


```VB
Property LineStyle As Long
```



## <a name="property-value"></a>Значение свойства

Стиль линии, используемый для отображения значения счетчика. Значения соответствуют системным константам, приведенным в следующей таблице.



| Значение                                                                                                                                                                                                                                                                                                                                                                               | Значение                                                          |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------|
| <span id="System.Drawing.Drawing2D.DashStyle.Solid"></span><span id="system.drawing.drawing2d.dashstyle.solid"></span><span id="SYSTEM.DRAWING.DRAWING2D.DASHSTYLE.SOLID"></span><dl> <dt>**System. Drawing. Drawing2D. DashStyle. твердое**</dt> значение <dt>0</dt> </dl>                     | Сплошная линия. Это значение по умолчанию.<br/>                |
| <span id="System.Drawing.Drawing2D.DashStyle.Dash"></span><span id="system.drawing.drawing2d.dashstyle.dash"></span><span id="SYSTEM.DRAWING.DRAWING2D.DASHSTYLE.DASH"></span><dl> <dt>**System. Drawing. Drawing2D. DashStyle. тире**</dt> <dt>1</dt> </dl>                         | Пунктирная линия с длинными сегментами и узкими пробелами.<br/>     |
| <span id="System.Drawing.Drawing2D.DashStyle.Dot"></span><span id="system.drawing.drawing2d.dashstyle.dot"></span><span id="SYSTEM.DRAWING.DRAWING2D.DASHSTYLE.DOT"></span><dl> <dt>**System. Drawing. Drawing2D. DashStyle. dot**</dt> <dt>2</dt> </dl>                             | Пунктирная линия с равномерными сегментами и пробелами.<br/>         |
| <span id="System.Drawing.Drawing2D.DashStyle.DashDot"></span><span id="system.drawing.drawing2d.dashstyle.dashdot"></span><span id="SYSTEM.DRAWING.DRAWING2D.DASHSTYLE.DASHDOT"></span><dl> <dt>**System. Drawing. Drawing2D. DashStyle. дашдот**</dt> <dt>3</dt> </dl>             | Пунктирная линия с чередованием коротких и длинных сегментов.<br/> |
| <span id="System.Drawing.Drawing2D.DashStyle.DashDotDot"></span><span id="system.drawing.drawing2d.dashstyle.dashdotdot"></span><span id="SYSTEM.DRAWING.DRAWING2D.DASHSTYLE.DASHDOTDOT"></span><dl> <dt>**System. Drawing. Drawing2D. DashStyle. дашдотдот**</dt> <dt>4</dt> </dl> | Пунктирная линия с чередованием штрихов и двойными точками.<br/>  |



 

## <a name="exceptions"></a>Исключения



| Тип исключения               | Условие                              |
|------------------------------|----------------------------------------|
| **System.ArgumentException** | Указан недопустимый стиль линии. |



 

## <a name="remarks"></a>Комментарии

Чтобы указать значение, отличное от DashStyle. сплошной, [**каунтеритем. Width**](counteritem-width.md) должно иметь значение 1. Если ширина больше 1, СИСМОН игнорирует указанный стиль линии и использует DashStyle. сплошной.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                            |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                  |
| DLL<br/>                      | <dl> <dt>Сисмон. ocx</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**каунтеритем**](counteritem.md)
</dt> </dl>

 

 





