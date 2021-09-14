---
title: Расположение джойстика
description: Расположение джойстика
ms.assetid: db0d1125-e39f-445b-bd65-373633cad578
keywords:
- Джойстики, расположение
- Джойстики, кнопки
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6bcdc187cfba244bb2b8c28c37e3677593f99870
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246202"
---
# <a name="joystick-position"></a>Расположение джойстика

Вы можете запросить в джойстике сведения о положении и кнопке с помощью функции [**жойжетпос**](/windows/win32/api/joystickapi/nf-joystickapi-joygetpos) . Например, приложение может отправлять запросы к джойстику для значений расположения базовых показателей. Страница свойств панели управления джойстика использует этот метод при калибровке джойстика.

Вы также можете запросить джойстик или другое устройство с расширенными возможностями с помощью функции [**жойжетпосекс**](/windows/win32/api/joystickapi/nf-joystickapi-joygetposex) .

 

 