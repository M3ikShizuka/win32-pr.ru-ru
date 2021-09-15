---
title: Динамический API аннотации
description: Динамический API Аннотации — это расширение Microsoft Active Accessibility, которое позволяет разработчикам настраивать существующую поддержку IAccessible без использования подверженных ошибкам методов подклассов или оболочек.
ms.assetid: 2daf0e76-b300-47e7-994b-d1d00d0dca4d
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d7f73c1da79784fdd86652128b572fd81904023c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458160"
---
# <a name="dynamic-annotation-api"></a>Динамический API аннотации

Динамический API Аннотации — это расширение Microsoft Active Accessibility, которое позволяет разработчикам настраивать существующую поддержку [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) без использования подверженных ошибкам методов подклассов или оболочек. Этот механизм также позволяет разработчикам передавать подсказки или другую полезную информацию в Oleacc.dll прокси-серверы.

Динамическая Аннотация обычно используется для исправления или уточнения неточного экземпляра объекта [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) , предоставляемого существующим Oleacc.dll прокси. Например, его можно использовать для переопределения свойств [**имени**](name-property.md) и [**роли**](role-property.md) , предоставляемых прокси-сервером по умолчанию, а также для предоставления свойств [**Description**](description-property.md) и [**Help**](help-property.md) (которые могут не предоставляться прокси-сервером по умолчанию).

с Windows 7 разработчики могут использовать динамический API аннотации, чтобы закомментировать свойства автоматизации пользовательского интерфейса майкрософт, а также свойства microsoft Active Accessibility прокси-объектов, которые Oleacc.dll создаются для стандартных элементов управления Windows. Oleacc.dll прокси-объекты служат для клиентов Microsoft Active Accessibility и автоматизации пользовательского интерфейса.

## <a name="in-this-section"></a>Содержание раздела

-   [Основные сведения](background-information.md)
-   [Альтернативы динамической аннотации](alternatives-to-dynamic-annotation.md)
-   [Типы динамических заметок](types-of-dynamic-annotation.md)
-   [Непосредственная Аннотация](direct-annotation.md)
-   [Аннотация схемы значений](value-map-annotation.md)
-   [Заметки сервера](server-annotation.md)
-   [Проблемы и ограничения](issues-and-limitations.md)

 

 




