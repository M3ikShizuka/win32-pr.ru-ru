---
description: Класс Кмедиаевент предоставляет реализацию базового класса для методов IDispatch сдвоенного интерфейса Имедиаевент. Он оставляет чисто виртуальные свойства и методы интерфейса Имедиаевент.
ms.assetid: 849e08ac-8d1b-4c86-94eb-ab5c4f10d68a
title: Класс Кмедиаевент
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CMediaEvent
api_type:
- COM
api_location: ''
ms.openlocfilehash: 927e561fa557ac33b1669ca7353377f7814ca448
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054715"
---
# <a name="cmediaevent-class"></a>Класс Кмедиаевент

![Иерархия классов кмедиаевент](images/cutil03.png)

`CMediaEvent`Класс предоставляет реализацию базового класса для методов **IDispatch** сдвоенного интерфейса [**имедиаевент**](/windows/desktop/api/Control/nn-control-imediaevent). Он оставляет чисто виртуальные свойства и методы интерфейса **имедиаевент** .

`CMediaEvent`Класс также предоставляет реализацию базового класса интерфейса [**имедиаевентекс**](/windows/desktop/api/Control/nn-control-imediaeventex) , производного от [**имедиаевент**](/windows/desktop/api/Control/nn-control-imediaevent).

Функции-члены [**кмедиаевент:: GetIdsOfNames**](cmediaevent-getidsofnames.md), [**Кмедиаевент:: GetTypeInfo**](cmediaevent-gettypeinfo.md), [**Кмедиаевент:: Жеттипеинфокаунт**](cmediaevent-gettypeinfocount.md)и [**кмедиаевент:: Invoke**](cmediaevent-invoke.md) являются стандартными реализациями интерфейса **IDispatch** с помощью класса [**кбаседиспатч**](cbasedispatch.md) (и библиотеки типов) для анализа команд и передачи их в чистые виртуальные методы интерфейса [**имедиаевент**](/windows/desktop/api/Control/nn-control-imediaevent) .



| Функции элементов                                         | Описание                                                                                                                                                                                   |
|----------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**кмедиаевент**](cmediaevent-cmediaevent.md)           | Конструирует объект **кмедиаевент** .                                                                                                                                                          |
| Методы IDispatch                                        | Описание                                                                                                                                                                                   |
| [**GetIDsOfNames**](cmediaevent-getidsofnames.md)       | Карты один элемент и необязательный набор параметров в соответствующий набор целочисленных идентификаторов диспетчеризации, которые можно использовать при последующих вызовах метода **IDispatch:: Invoke** . |
| [**GetTypeInfo**](cmediaevent-gettypeinfo.md)           | Извлекает объект сведений о типе, который извлекает сведения о типе для интерфейса.                                                                                                   |
| [**жеттипеинфокаунт**](cmediaevent-gettypeinfocount.md) | Извлекает количество интерфейсов типа данных, предоставленных объектом.                                                                                                                    |
| [**Invoke**](cmediaevent-invoke.md)                     | Предоставляет доступ к открытым свойствам и методам объекта.                                                                                                                               |



 

 

 



