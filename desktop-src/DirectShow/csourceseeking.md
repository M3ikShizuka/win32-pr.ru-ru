---
description: Класс Ксаурцесикинг является абстрактным классом для реализации поиска в фильтрах источников с одним выходным закреплением.
ms.assetid: 46e711e1-78d4-4e83-9df1-06032edeba6a
title: Класс Ксаурцесикинг (Ктлутил. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CSourceSeeking
api_type:
- COM
api_location:
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
ms.openlocfilehash: 475d8b58decac9297b9e02ebf8116ea5c86d224fc534626937fbed7daf5b2c4f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119907843"
---
# <a name="csourceseeking-class"></a>Класс Ксаурцесикинг

![Иерархия классов ксаурцесикинг](images/cutil15.png)

Класс **ксаурцесикинг** является абстрактным классом для реализации поиска в фильтрах источников с одним выходным закреплением.

Этот класс поддерживает интерфейс [**имедиасикинг**](/windows/desktop/api/Strmif/nn-strmif-imediaseeking) . Он предоставляет реализации по умолчанию для всех методов **имедиасикинг** . Защищенные переменные членов хранят время начала, время окончания и текущую скорость. По умолчанию в качестве формата времени, поддерживаемого классом, используется **\_ Формат времени \_ носителя \_** (100-наносекундных единиц). Дополнительные сведения см. в разделе "Примечания".



| Защищенные переменные членов                                          | Описание                                                                                 |
|---------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
| [**m \_ ртдуратион**](csourceseeking-m-rtduration.md)                | Длительность потока.                                                                     |
| [**m \_ ртстарт**](csourceseeking-m-rtstart.md)                      | Время начала.                                                                                 |
| [**m \_ ртстоп**](csourceseeking-m-rtstop.md)                        | Время окончания.                                                                                  |
| [**m \_ дратесикинг**](csourceseeking-m-drateseeking.md)            | Скорость воспроизведения.                                                                              |
| [**m \_ двсикингкапс**](csourceseeking-m-dwseekingcaps.md)          | Поиск возможностей.                                                                       |
| [**m \_ плокк**](csourceseeking-m-plock.md)                          | Указатель на объект критической секции для блокировки.                                           |
| Защищенные методы                                                   | Описание                                                                                 |
| [**ксаурцесикинг**](csourceseeking-csourceseeking.md)             | Метод конструктора.                                                                         |
| Чистые виртуальные методы                                                | Описание                                                                                 |
| [**чанжерате**](csourceseeking-changerate.md)                     | Вызывается при изменении частоты воспроизведения.                                                      |
| [**чанжестарт**](csourceseeking-changestart.md)                   | Вызывается при изменении начальной должности.                                                     |
| [**чанжестоп**](csourceseeking-changestop.md)                     | Вызывается при изменении позиции окончания.                                                      |
| Методы Имедиасикинг                                               | Описание                                                                                 |
| [**исформатсуппортед**](csourceseeking-isformatsupported.md)       | Определяет, поддерживается ли указанный формат времени.                                    |
| [**куерипреферредформат**](csourceseeking-querypreferredformat.md) | Возвращает предпочтительный формат времени объекта.                                               |
| [**сеттимеформат**](csourceseeking-settimeformat.md)               | Задает формат времени.                                                                       |
| [**исусингтимеформат**](csourceseeking-isusingtimeformat.md)       | Определяет, является ли указанный формат времени используемым в данный момент форматом.                  |
| [**жеттимеформат**](csourceseeking-gettimeformat.md)               | Извлекает текущий формат времени.                                                          |
| [**Длительное время**](csourceseeking-getduration.md)                   | Возвращает длительность потока.                                                       |
| [**жетстоппоситион**](csourceseeking-getstopposition.md)           | Возвращает время, когда воспроизведение будет прервано относительно длительности потока. |
| [**жеткуррентпоситион**](csourceseeking-getcurrentposition.md)     | Извлекает текущую координату относительно общей продолжительности потока.               |
| [**GetCapabilities**](csourceseeking-getcapabilities.md)           | Извлекает все возможности поиска в потоке.                                       |
| [**чекккапабилитиес**](csourceseeking-checkcapabilities.md)       | Запрашивает, имеет ли поток указанные возможности поиска.                              |
| [**конверттимеформат**](csourceseeking-converttimeformat.md)       | Преобразует из одного формата времени в другой.                                                   |
| [**сетпоситионс**](csourceseeking-setpositions.md)                 | Установка текущей позиции и позиции окончания.                                            |
| [**Выстановки**](csourceseeking-getpositions.md)                 | Извлекает текущую и заданную позиции.                                       |
| [**Доступность**](csourceseeking-getavailable.md)                 | Извлекает диапазон времени, в течение которого поиск является эффективным.                                 |
| [**сетрате**](csourceseeking-setrate.md)                           | Задает скорость воспроизведения.                                                                     |
| [**Коэффициент**](csourceseeking-getrate.md)                           | Возвращает скорость воспроизведения.                                                                |
| [**жетпреролл**](csourceseeking-getpreroll.md)                     | Извлекает время предвремени.                                                                 |



 

## <a name="remarks"></a>Remarks

При изменении начальной позиции, позиции окончания или скорости воспроизведения объект **ксаурцесикинг** вызывает соответствующий чистый виртуальный метод:

-   Начальное расположение: [ **ксаурцесикинг:: чанжестарт**](csourceseeking-changestart.md)
-   Позиция окончания: [ **ксаурцесикинг:: чанжестоп**](csourceseeking-changestop.md)
-   Скорость воспроизведения: [ **ксаурцесикинг:: чанжерате**](csourceseeking-changerate.md)

Производный класс должен реализовывать эти методы. После любой операции поиска фильтр должен выполнить следующие действия.

1.  Вызовите метод [**Ипин:: бегинфлуш**](/windows/desktop/api/Strmif/nf-strmif-ipin-beginflush) для входного контакта нисходящего входа.
2.  Остановите рабочий поток, который доставляет данные.
3.  Вызовите метод [**Ипин:: ендфлуш**](/windows/desktop/api/Strmif/nf-strmif-ipin-endflush) для входного ПИН-кода.
4.  Перезапустите рабочий поток.
5.  Вызовите метод [**Ипин:: невсегмент**](/windows/desktop/api/Strmif/nf-strmif-ipin-newsegment) для входного ПИН-кода.
6.  Задайте свойство ненепрерывности в первом примере. Вызовите метод [**имедиасампле:: сетдисконтинуити**](/windows/desktop/api/Strmif/nf-strmif-imediasample-setdiscontinuity) .

Вызов [**бегинфлуш**](/windows/desktop/api/Strmif/nf-strmif-ipin-beginflush) освобождает рабочий поток, если поток блокируется, ожидая доставки примера.

На шаге 2 Убедитесь, что поток остановил отправку данных. В зависимости от реализации может потребоваться подождать, пока поток завершит работу, или поток, чтобы передать ответ какого-либо типа. Если фильтр использует класс [**ксаурцестреам**](csourcestream.md) , метод [**ксаурцестреам::**](csourcestream-stop.md) End блокируется до тех пор, пока рабочий поток не ответит.

В идеале новый сегмент (шаг 5) должен быть доставлен из рабочего потока. Это также можно сделать с помощью объекта **ксаурцесикинг** , если фильтр сериализует его с помощью примеров.

В следующем примере показана возможная реализация. Предполагается, что выходной ПИН-код фильтра источника является производным от **ксаурцесикинг** и [**ксаурцестреам**](csourcestream.md). В этом примере определяется вспомогательный метод Упдатефромсик, который выполняет шаги 1 4. Метод [**ксаурцестреам:: онсреадстартплай**](csourcestream-onthreadstartplay.md) переопределен для отправки нового сегмента и для установки флага, указывающего на ненепрерывность. Рабочий поток выбирает этот флаг и вызывает метод [**имедиасампле:: сетдисконтинуити**](/windows/desktop/api/Strmif/nf-strmif-imediasample-setdiscontinuity) :


```C++
void CMyStream::UpdateFromSeek()
{
    if (ThreadExists()) 
    {
        DeliverBeginFlush();
        Stop();
        DeliverEndFlush();
        Run();
    }
}

HRESULT CMyStream::OnThreadStartPlay()
{
    m_bDiscontinuity = TRUE;
    return DeliverNewSegment(m_rtStart, m_rtStop, m_dRateSeeking);
}
```



### <a name="supporting-additional-time-formats"></a>Поддержка дополнительных форматов времени

По умолчанию этот класс поддерживает поиск только в единицах времени ссылки ( \_ Формат времени \_ носителя \_ ). Для поддержки дополнительных форматов времени Переопределите методы [**имедиасикинг**](/windows/desktop/api/Strmif/nn-strmif-imediaseeking) , которые работают с форматами времени:

-   [**Имедиасикинг:: Жеттимеформат**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-gettimeformat)
-   [**Имедиасикинг:: Жеттимеформат**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-gettimeformat)
-   [**Имедиасикинг:: Исусингтимеформат**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-isusingtimeformat)
-   [**Имедиасикинг:: Исусингтимеформат**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-isusingtimeformat)
-   [**Имедиасикинг:: Сеттимеформат**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-settimeformat)

Кроме того, переопределите оставшиеся методы [**имедиасикинг**](/windows/desktop/api/Strmif/nn-strmif-imediaseeking) , чтобы выполнить необходимые преобразования между форматами времени. После вызова метода [**сеттимеформат**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-settimeformat) все методы **имедиасикинг** должны обрабатывать входящие и исходящие параметры времени в новом формате времени. Например, если переменная *m \_ ртдуратион* представляет продолжительность в единицах времени ссылки, но текущий формат времени — frames [**, метод IsReference**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-getduration) должен возвращать значение *m \_ ртдуратион* , преобразованное в кадры. Например:


```
STDMETHODIMP GetDuration(LONGLONG *pDuration)
{
    HRESULT hr = CSourceSeeking::GetDuration(pDuration);
    if (SUCCEEDED(hr))
    {
        if (m_TimeFormat == TIME_FORMAT_FRAME)
        {
            // Convert from reference time to frames.
            *pDuration = TimeToFrame(*pDuration);  // Private method.
        }
    }
    return hr
} 
```



Кроме того, убедитесь в том, что в \_ \_ методе [**Имедиасикинг:: сетпоситионс**](/windows/desktop/api/Strmif/nf-strmif-imediaseeking-setpositions) установлен флаг "я искал ретурнтиме". Если этот флаг существует, при возврате значений позиций в вызывающий объект преобразуйте их в время ссылки.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>ктлутил. h (включает Потоки. h)</dt> </dl>                                                                                   |
| Библиотека<br/> | <dl> <dt>Стрмбасе. lib (розничные сборки); </dt> <dt>Стрмбасд. lib (отладочные сборки)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Поддержка поиска в фильтре источника](supporting-seeking-in-a-source-filter.md)
</dt> </dl>

 

 




