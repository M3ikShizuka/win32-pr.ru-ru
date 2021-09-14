---
description: API датчика может предоставлять уведомления о событиях.
ms.assetid: 2400619c-ee9c-4662-ae57-6d4bc317e730
title: Сведения о событиях API датчика
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: e941dca86d5b7ec3aa9922220c1232b10429f60a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127067023"
---
# <a name="about-sensor-api-events"></a>Сведения о событиях API датчика

API датчика может предоставлять уведомления о событиях.

При регистрации для получения событий с помощью [**исенсор:: сетевентсинк**](/windows/win32/api/sensorsapi/nf-sensorsapi-isensor-seteventsink) или [**Исенсорманажер:: сетевентсинк**](/windows/win32/api/sensorsapi/nf-sensorsapi-isensormanager-seteventsink)необходимо предоставить указатель на интерфейс обратного вызова. В коде необходимо реализовать методы интерфейса обратного вызова. API датчика определяет следующие интерфейсы обратного вызова:

-   [**Исенсоревентс**](/windows/desktop/api/sensorsapi/nn-sensorsapi-isensorevents). Реализуйте этот интерфейс для получения событий от датчиков. Датчики могут уведомлять ваше приложение о новых данных, изменениях состояния датчика, отключении датчика и пользовательских событиях, определенных производителем датчика.
-   [**Исенсорманажеревентс**](/windows/desktop/api/sensorsapi/nn-sensorsapi-isensormanagerevents). Реализуйте этот интерфейс для получения событий от диспетчера датчиков. Диспетчер датчиков может уведомлять приложение при подключении датчика и, следовательно, может быть доступным для использования.

Вы можете отменить уведомления о событиях, вызвав [**сетевентсинк**](/windows/win32/api/sensorsapi/nf-sensorsapi-isensor-seteventsink) еще раз. это время передает значение **null** через параметр.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Использование событий API датчика](using-sensor-api-events.md)
</dt> </dl>

 

 
