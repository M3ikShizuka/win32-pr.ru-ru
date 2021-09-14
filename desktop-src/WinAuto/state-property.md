---
title: Свойство State
description: Свойство State описывает состояние объекта в данный момент времени. Все объекты поддерживают свойство State.
ms.assetid: 6a56070f-7913-45b2-b693-3c0a8b7fa2f4
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d151f09fca6c31abaaa98a19139d3e22eb28ec90
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064080"
---
# <a name="state-property"></a>Свойство State

Свойство **State** описывает состояние объекта в данный момент времени. Все объекты поддерживают свойство **State** .

Свойство **State** извлекается путем вызова метода [**IAccessible:: Get \_ аккстате**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accstate).

Microsoft Active Accessibility предоставляет [константы состояния объектов](object-state-constants.md), определенные в олеакк. h, которые объединяются для определения состояния объекта. Рекомендуется, чтобы разработчики сервера использовали эти стандартные значения состояния. Если возвращаются стандартные значения состояния, клиенты используют [**жетстатетекст**](/windows/desktop/api/Oleacc/nf-oleacc-getstatetexta) для получения локализованной строки, описывающей состояние.

В графиках, которые иногда анимированы, свойство **State** должно иметь значение [**\_ \_ анимированная система состояния**](object-state-constants.md) , а свойство [**Role**](role-property.md) — [**\_ \_ график системы роли**](object-roles.md).

 

 




