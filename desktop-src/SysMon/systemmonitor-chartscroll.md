---
title: Системмонитор. Чартскролл, свойство
description: Возвращает или задает значение, определяющее, прокручивается ли линейный график в представлении.
ms.assetid: df4806be-dfd3-4ff7-985d-b46c00bb19f8
keywords:
- Сисмон свойство Чартскролл
- Свойство Чартскролл Сисмон, объект Системмонитор
- Сисмон объекта Системмонитор, свойство Чартскролл
topic_type:
- apiref
api_name:
- SystemMonitor.ChartScroll
api_location:
- Sysmon.ocx
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 51288af710e5ae94baf46acf0d2ed91732a1d310
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056784"
---
# <a name="systemmonitorchartscroll-property"></a>Системмонитор. Чартскролл, свойство

Возвращает или задает значение, определяющее, прокручивается ли линейный график в представлении.

## <a name="syntax"></a>Синтаксис


```VB
Property ChartScroll As Boolean
```



## <a name="property-value"></a>Значение свойства

Значение true, если линейный график непрерывно прокручивается справа налево; в противном случае значение false, если линейный график рисуется слева направо и заключает себя в представление. Значение по умолчанию — false.

## <a name="remarks"></a>Комментарии

Это значение игнорируется, если [**системмонитор. дисплайтипе**](systemmonitor-displaytype.md) не является [**дисплайтипеконстантс. сисмонлинеграф**](/windows/win32/api/isysmon/ne-isysmon-displaytypeconstants).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| DLL<br/>                      | <dl> <dt>Сисмон. ocx</dt> </dl> |



 

 





