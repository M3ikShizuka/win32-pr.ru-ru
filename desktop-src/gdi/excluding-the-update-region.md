---
description: Функция Ексклудеупдатергн исключает область обновления из области обрезки для контекста устройства дисплея.
ms.assetid: e652122b-a3b7-4d1b-8afd-9648d5ee3d42
title: Исключение региона обновления
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d1551990c1da985240ee606223177eb3e84118a7083c459e3991451cd313f3c9
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120092944"
---
# <a name="excluding-the-update-region"></a>Исключение региона обновления

Функция [**ексклудеупдатергн**](/windows/desktop/api/Winuser/nf-winuser-excludeupdatergn) исключает область обновления из области обрезки для контекста устройства дисплея. Эта функция полезна при рисовании в окне, отличном от, когда \_ обрабатывается сообщение WM Paint. Он не позволяет рисовать в областях, которые будут обновляться во время следующего \_ сообщения WM Paint.

 

 



