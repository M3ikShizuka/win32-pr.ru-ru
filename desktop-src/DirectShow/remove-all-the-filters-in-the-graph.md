---
description: Удалите все фильтры в Graph
ms.assetid: a11af581-c331-4607-be8b-5f65961bd422
title: Удалите все фильтры в Graph
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 67d414ef7e532eaf5df9143a6b601a57e4a8bd45
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127348919"
---
# <a name="remove-all-the-filters-in-the-graph"></a>Удалите все фильтры в Graph

самый простой способ удалить все фильтры в графе фильтра — это просто освободить фильтр Graph Manager и создать новый. обязательно выпустите все указатели, которые ваше приложение будет использовать с любыми интерфейсами в фильтре Graph диспетчеры, а также указатели на объекты в графе, включая фильтры, пин-коды, контрольные часы и т. д.

Кроме того, можно удалить фильтры по одному с помощью метода [**ифилтерграф:: ремовефилтер**](/windows/desktop/api/Strmif/nf-strmif-ifiltergraph-removefilter) :


```C++
// Stop the graph.
pControl->Stop();

// Enumerate the filters in the graph.
IEnumFilters *pEnum = NULL;
HRESULT hr = pGraph->EnumFilters(&pEnum);
if (SUCCEEDED(hr))
{
    IBaseFilter *pFilter = NULL;
    while (S_OK == pEnum->Next(1, &pFilter, NULL))
     {
         // Remove the filter.
         pGraph->RemoveFilter(pFilter);
         // Reset the enumerator.
         pEnum->Reset();
         pFilter->Release();
    }
    pEnum->Release();
}
```



В этом примере используется метод [**ифилтерграф:: енумфилтерс**](/windows/desktop/api/Strmif/nf-strmif-ifiltergraph-enumfilters) для перечисления фильтров в графе. Удаление фильтра приводит к тому, что объект перечислителя становится несинхронизированным с графом. Чтобы сбросить перечислитель, используйте метод [**иенумфилтерс:: Reset**](/windows/desktop/api/Strmif/nf-strmif-ienumfilters-reset) . В противном случае любой последующий вызов метода [**иенумфилтерс:: Next**](/windows/desktop/api/Strmif/nf-strmif-ienumfilters-next) завершится ошибкой.

 

 



