---
title: Защита от повторного входа в функции-ловушки
description: Пока функция-обработчик обрабатывает событие, могут быть активированы дополнительные события, что может привести к повторному вводу функции-обработчика до завершения обработки исходного события.
ms.assetid: 2382e7a4-82df-423a-8479-66e28baf8105
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 74e2b0dc6f8951bf48ce3fecabd3a81bd345388d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127568535"
---
# <a name="guarding-against-reentrancy-in-hook-functions"></a>Защита от повторного входа в функции-ловушки

Пока функция-обработчик обрабатывает событие, могут быть активированы дополнительные события, что может привести к повторному вводу функции-обработчика до завершения обработки исходного события. Проблема с повторным входом в функции-ловушки заключается в том, что события выполняются вне последовательности, если только функция-обработчик не обрабатывает эту ситуацию.

Например, рассмотрим случай, когда функция-ловушка в программе чтения с экрана обрабатывает событие [**\_ \_ валуечанже объекта Event**](event-constants.md) для элемента управления Edit. Если при обработке события изменения первого значения функция-обработчик повторно введена для обработки последующего события изменения значения, второе событие завершается перед первым событием. В этом случае средство чтения с экрана передает пользователю неточные сведения.

Поскольку обработка событий прервана, дополнительные события могут быть получены каждый раз, когда функция-обработчик вызывает функцию, которая вызывает проверку очереди сообщений владеющего потока. Это происходит, когда в функции-обработчике вызывается любой из следующих функций:

-   функции Windows [**SendMessage**](/windows/desktop/api/winuser/nf-winuser-sendmessage), [](/windows/desktop/api/winuser/nf-winuser-getmessage) [**PeekMessage**](/windows/desktop/api/winuser/nf-winuser-peekmessagea), [**диалогбокс**](/windows/desktop/api/winuser/nf-winuser-dialogboxa)или [**MessageBox**](/windows/desktop/api/winuser/nf-winuser-messagebox)
-   Функции Microsoft Active Accessibility [**акцессиблеобжектфромевент**](/windows/desktop/api/Oleacc/nf-oleacc-accessibleobjectfromevent), [**акцессиблеобжектфромвиндов**](/windows/desktop/api/Oleacc/nf-oleacc-accessibleobjectfromwindow), [**акцессиблеобжектфромпоинт**](/windows/desktop/api/Oleacc/nf-oleacc-accessibleobjectfrompoint)
-   Интерфейс [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) или другое свойство или метод объектной модели компонента (com), пересекающие границы процесса

Поскольку функции-обработчики вызывают свойства и методы [**акцессиблеобжектфромевент**](/windows/desktop/api/Oleacc/nf-oleacc-accessibleobjectfromevent) и [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) , невозможно предотвратить повторный вход. Единственным решением является добавление кода в функцию-обработчик, которая обнаруживает повторный вход и принимает соответствующее действие при повторном вводе функции-обработчика.

 

 