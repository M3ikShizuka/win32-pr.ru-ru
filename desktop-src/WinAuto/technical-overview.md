---
title: Технический обзор
description: Microsoft Active Accessibility улучшает возможности специальных возможностей (специализированные программы, которые помогают людям с ограниченными возможностями использовать компьютеры более эффективно), работают с приложениями, работающими на Microsoft Windows.
ms.assetid: d71ef40e-4c58-4ee6-8909-04ff4f8d20d3
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 69f3931c6a69e9b8caed849942424039178a7884
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127567342"
---
# <a name="technical-overview"></a>Технический обзор

Microsoft Active Accessibility улучшает возможности специальных возможностей (специализированные программы, которые помогают людям с ограниченными возможностями использовать компьютеры более эффективно), работают с приложениями, работающими на Microsoft Windows.

Microsoft Active Accessibility основан на модели COM, разработанной корпорацией Майкрософт и является отраслевым стандартом, который определяет общий способ обмена данными между приложениями и операционными системами. Microsoft Active Accessibility состоит из следующих компонентов:

-   COM-интерфейс [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible), который предоставляет сведения об элементах пользовательского интерфейса. **IAccessible** также имеет свойства и методы для получения сведений об этом элементе пользовательского интерфейса и управления им.
-   Виневентс — система событий, которая позволяет серверам уведомлять клиентов при изменении объекта со специальными возможностями.
-   Oleacc.dll, поддержка или библиотека DLL времени выполнения.

Библиотека Microsoft Active Accessibility DLL, Oleacc.dll, состоит из следующих компонентов:

-   Функции, которые позволяют клиентам запрашивать указатель интерфейса [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) (например, [**акцессиблеобжектфромвиндов**](/windows/desktop/api/Oleacc/nf-oleacc-accessibleobjectfromwindow)).
-   Функции, которые позволяют серверам возвращать указатель интерфейса [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) клиенту (например, [**функции lresultfromobject**](/windows/desktop/api/Oleacc/nf-oleacc-lresultfromobject)).
-   Функции для получения локализованного текста для кода роли и состояния (например, [**жетролетекст**](/windows/desktop/api/Oleacc/nf-oleacc-getroletexta) и [**жетстатетекст**](/windows/desktop/api/Oleacc/nf-oleacc-getstatetexta)).
-   Некоторые вспомогательные функции ([**акцессиблечилдрен**](/windows/desktop/api/Oleacc/nf-oleacc-accessiblechildren)).
-   Код, предоставляющий реализацию класса [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) по умолчанию для стандартных элементов управления User и комктл. Поскольку они реализуют **IAccessible** от имени системных элементов управления, они называются *прокси-серверами*.

## <a name="in-this-section"></a>Содержание раздела

-   [Как работает Active Accessibility](how-active-accessibility-works.md)
-   [Основы Active Accessibility](active-accessibility-basics.md)
-   [Рекомендации по серверам](server-guidelines.md)
-   [Рекомендации для клиентов](client-guidelines.md)
-   [Рекомендации по COM и Юникод](com-and-unicode-guidelines.md)

 

 




