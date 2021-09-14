---
title: Запись данных с помощью канала DVC
description: Запись данных канала с помощью динамического виртуального канала (DVC) является симметричным для сервера узла сеансов удаленный рабочий стол (узла сеансов удаленных рабочих столов) и клиента.
ms.assetid: 33bacbf0-c558-497a-a08a-95eb398fad97
ms.tgt_platform: multiple
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4fd6f26e926958ceba5418a72849b75a66b11d2d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064478"
---
# <a name="writing-data-by-using-a-dvc-channel"></a>Запись данных с помощью канала DVC

Запись данных канала с помощью динамического виртуального канала (DVC) является симметричным для сервера узла сеансов удаленный рабочий стол (узла сеансов удаленных рабочих столов) и клиента. Запись данных канала реализуется методом [**Write**](/windows/desktop/api/TsVirtualChannels/nf-tsvirtualchannels-iwtsvirtualchannel-write) интерфейса [**ивтсвиртуалчаннел**](/windows/desktop/api/TsVirtualChannels/nn-tsvirtualchannels-iwtsvirtualchannel) .

На следующем рисунке показана отправка и получение пакета данных между клиентом и сервером DVC (подключаемым модулем DVC).

![Отправка и получение пакета данных между клиентом и сервером DVC](images/writedvcchannel.png)

 

 




