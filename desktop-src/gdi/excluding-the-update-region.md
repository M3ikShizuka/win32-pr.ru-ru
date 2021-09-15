---
description: Функция Ексклудеупдатергн исключает область обновления из области обрезки для контекста устройства дисплея.
ms.assetid: e652122b-a3b7-4d1b-8afd-9648d5ee3d42
title: Исключение региона обновления
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a7be39b948e61fc06c7f7005d15c1163cef0068f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127580491"
---
# <a name="excluding-the-update-region"></a>Исключение региона обновления

Функция [**ексклудеупдатергн**](/windows/desktop/api/Winuser/nf-winuser-excludeupdatergn) исключает область обновления из области обрезки для контекста устройства дисплея. Эта функция полезна при рисовании в окне, отличном от, когда \_ обрабатывается сообщение WM Paint. Он не позволяет рисовать в областях, которые будут обновляться во время следующего \_ сообщения WM Paint.

 

 



