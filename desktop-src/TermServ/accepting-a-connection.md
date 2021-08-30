---
title: Принятие подключения (службы удаленных рабочих столов)
description: В некоторый момент времени клиент динамического виртуального канала (DVC) запрашивает подключение к прослушивателю DVC.
ms.assetid: eab17aa9-590c-4da2-a1a9-6e50a11d1de7
ms.tgt_platform: multiple
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: df1747354f540db8b50aff23fa5dc8ad23289b11c7a003e8281b72c8f8c174fa
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120099662"
---
# <a name="accepting-a-connection-remote-desktop-services"></a>Принятие подключения (службы удаленных рабочих столов)

В некоторый момент времени клиент динамического виртуального канала (DVC) запрашивает подключение к прослушивателю DVC. В этом случае прослушиватель может создать уникальный коммуникационный канал для клиента, который обрабатывается методом [**Онневчаннелконнектион**](/windows/desktop/api/TsVirtualChannels/nf-tsvirtualchannels-iwtslistenercallback-onnewchannelconnection) [**ивтслистенеркаллбакк**](/windows/desktop/api/TsVirtualChannels/nn-tsvirtualchannels-iwtsvirtualchannelcallback). Пример см. в описании реализации **кдвксамплеплугин:: онневчаннелконнектион** в примере кода [подключаемого модуля клиента DVC](dvc-client-plug-in-example.md) .

На следующем рисунке показана последовательность событий для установления соединения DVC. Затененные объекты предоставляются пользователем (DVC Application/Service и [**ивтслистенеркаллбакк**](/windows/desktop/api/TsVirtualChannels/nn-tsvirtualchannels-iwtslistenercallback)), а незатененные объекты являются частью платформы (удаленный рабочий стол узла сеансов (узел сеансов удаленных рабочих столов), прослушиватель и [**ивтсвиртуалчаннел**](/windows/desktop/api/TsVirtualChannels/nn-tsvirtualchannels-iwtsvirtualchannel)).

![последовательность событий для установления соединения DVC](images/acceptingconnection.png)

> [!Note]  
> На этом рисунке предполагается, что объект прослушивателя был создан с помощью вызова [**креателистенер**](/windows/desktop/api/TsVirtualChannels/nf-tsvirtualchannels-iwtsvirtualchannelmanager-createlistener) в [**ивтсвиртуалчаннелманажер**](/windows/desktop/api/TsVirtualChannels/nn-tsvirtualchannels-iwtsvirtualchannelmanager)и что подключаемый модуль указал [**ивтслистенеркаллбакк**](/windows/desktop/api/TsVirtualChannels/nn-tsvirtualchannels-iwtslistenercallback) в качестве параметра.

 

 

 




