---
description: Класс Кбасемедиафилтер реализует интерфейс Имедиафилтер.
ms.assetid: 45c8973b-d0b3-4aeb-96e7-be47f8d7f4a7
title: Класс Кбасемедиафилтер (Амфилтер. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CBaseMediaFilter
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 4e594fd941fffecc836af26bd3d70cced82ddcaa
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127273219"
---
# <a name="cbasemediafilter-class"></a>Класс Кбасемедиафилтер

![кбасемедиафилтер](images/filter05.png)

`CBaseMediaFilter`Класс реализует интерфейс [**имедиафилтер**](/windows/desktop/api/Strmif/nn-strmif-imediafilter) . Используйте этот класс для распространителей подключаемых модулей или других объектов, которым требуется поддержка **имедиафилтер** без поддержки интерфейса [**ибасефилтер**](/windows/desktop/api/Strmif/nn-strmif-ibasefilter) . Не используйте этот класс для фильтров. Вместо этого используйте класс [**кбасефилтер**](cbasefilter.md) или базовый класс, производный от **кбасефилтер**.



| Защищенные переменные членов                                       | Описание                                                  |
|------------------------------------------------------------------|--------------------------------------------------------------|
| [**\_штат m**](cbasemediafilter-m-state.md)                     | Текущее состояние объекта.                                 |
| [**m \_ пклокк**](cbasemediafilter-m-pclock.md)                   | Указатель на время обращения к объекту.                     |
| [**m \_ тстарт**](cbasemediafilter-m-tstart.md)                   | Справочное время, соответствующее времени потока 0.            |
| [**m \_ CLSID**](cbasemediafilter-m-clsid.md)                     | Идентификатор класса (CLSID) объекта.                      |
| [**m \_ плокк**](cbasemediafilter-m-plock.md)                     | Указатель на критическую секцию.                               |
| Открытые методы                                                   | Описание                                                  |
| [**кбасемедиафилтер**](cbasemediafilter-cbasemediafilter.md)    | Метод конструктора.                                          |
| [**~ Кбасемедиафилтер**](cbasemediafilter--cbasemediafilter.md) | Метод деструктора. Виртуализаци.                                  |
| [**стреамтиме**](cbasemediafilter-streamtime.md)                | Извлекает текущее время потока. Виртуализаци.                  |
| [**IsActive**](cbasemediafilter-isactive.md)                    | Определяет, является ли объект активным (запущен или приостановлен). |
| Методы IPersist                                                 | Описание                                                  |
| [**GetClassID**](cbasemediafilter-getclassid.md)                | Получает идентификатор класса.                              |
| Методы Имедиафилтер                                             | Описание                                                  |
| [**GetState**](cbasemediafilter-getstate.md)                    | Получает состояние объекта (запущен, остановлен или приостановлен).  |
| [**сетсинксаурце**](cbasemediafilter-setsyncsource.md)          | Задает время ссылки для объекта.                       |
| [**жетсинксаурце**](cbasemediafilter-getsyncsource.md)          | Извлекает ссылочное время, которое использует объект.      |
| [**Остановить**](cbasemediafilter-stop.md)                            | Останавливает объект.                                            |
| [**Пауза**](cbasemediafilter-pause.md)                          | Приостанавливает работу объекта.                                           |
| [**Выполнить**](cbasemediafilter-run.md)                              | Запускает объект.                                             |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>амфилтер. h (включает Потоки. h)</dt> </dl>                                                                                  |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



 

 




