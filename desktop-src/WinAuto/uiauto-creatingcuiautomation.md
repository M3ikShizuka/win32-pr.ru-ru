---
title: Создание объекта Куиаутоматион
description: В этом разделе описывается, как приступить к написанию клиентского приложения Microsoft UI Automation путем создания экземпляра объекта, реализующего Иуиаутоматион.
ms.assetid: 9b90da60-0204-48c1-bb16-ff4a843bac67
keywords:
- Клиенты, создание объекта Куиаутоматион
- Клиенты, объект Куиаутоматион
- Модель автоматизации пользовательского интерфейса, объект Куиаутоматион
- Модель автоматизации пользовательского интерфейса, создание объекта Куиаутоматион
- Создание объекта Куиаутоматион
- Объект Куиаутоматион
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 8162dac5276bbb22d00413276482cca34334fda5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064022"
---
# <a name="creating-the-cuiautomation-object"></a>Создание объекта Куиаутоматион

В этом разделе описывается, как приступить к написанию клиентского приложения Microsoft UI Automation путем создания экземпляра объекта, реализующего [**иуиаутоматион**](/windows/desktop/api/UIAutomationClient/nn-uiautomationclient-iuiautomation).

В этом разделе содержатся следующие подразделы.

-   [Объект Куиаутоматион](#the-cuiautomation-object)
-   [Создание объекта](#creating-the-object)
-   [Связанные темы](#related-topics)

## <a name="the-cuiautomation-object"></a>Объект Куиаутоматион

Первым шагом в использовании модели автоматизации пользовательского интерфейса является создание объекта класса [**куиаутоматион**](/previous-versions/windows/desktop/legacy/ff384838(v=vs.85)) . Этот объект предоставляет интерфейс [**иуиаутоматион**](/windows/desktop/api/UIAutomationClient/nn-uiautomationclient-iuiautomation) , который является шлюзом для всех других объектов и интерфейсов, используемых клиентскими приложениями. Помимо прочего, **иуиаутоматион** используется для следующих задач:

-   Подписка на события.
-   Создание условий. Условия — это объекты, используемые для ограничения области поиска элементов модели автоматизации пользовательского интерфейса.
-   Получение элементов автоматизации пользовательского интерфейса непосредственно с рабочего стола (корневого элемента) или из экранных координат или дескрипторов окна.
-   Создание объектов обхода дерева, которые можно использовать для навигации по иерархии элементов модели автоматизации пользовательского интерфейса.
-   Преобразование типов данных.

## <a name="creating-the-object"></a>Создание объекта

Чтобы приступить к использованию модели автоматизации пользовательского интерфейса в приложении, выполните следующие действия.

-   Включите UIAutomation. h в заголовки проекта. UIAutomation. h предоставляет другие заголовки, определяющие API.
-   Объявите указатель на [**иуиаутоматион**](/windows/desktop/api/UIAutomationClient/nn-uiautomationclient-iuiautomation).
-   Инициализация объектной модели компонента (COM).
-   Создайте экземпляр [**куиаутоматион**](/previous-versions/windows/desktop/legacy/ff384838(v=vs.85)) и извлеките интерфейс [**иуиаутоматион**](/windows/desktop/api/UIAutomationClient/nn-uiautomationclient-iuiautomation) в указатель.

Следующий пример функции инициализирует COM, а затем создает объект [**куиаутоматион**](/previous-versions/windows/desktop/legacy/ff384838(v=vs.85)) , получая интерфейс [**иуиаутоматион**](/windows/desktop/api/UIAutomationClient/nn-uiautomationclient-iuiautomation) в указателе *ппаутоматион* .


```C++
#include <uiautomation.h>

// CoInitialize must be called before calling this function, and the  
// caller must release the returned pointer when finished with it.
// 
HRESULT InitializeUIAutomation(IUIAutomation **ppAutomation)
{
    return CoCreateInstance(CLSID_CUIAutomation, NULL,
        CLSCTX_INPROC_SERVER, IID_IUIAutomation, 
        reinterpret_cast<void**>(ppAutomation));
}
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

**Основные понятия**
</dt> <dt>

[Обзор событий автоматизации пользовательского интерфейса](uiauto-eventsoverview.md)
</dt> <dt>

[Получение элементов автоматизации пользовательского интерфейса](uiauto-obtainingelements.md)
</dt> </dl>

 

 