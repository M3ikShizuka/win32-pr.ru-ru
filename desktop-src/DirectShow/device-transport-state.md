---
description: Состояние транспорта устройства
ms.assetid: 15edded0-207c-41e8-81fe-deb6335045eb
title: Состояние транспорта устройства
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 05f52ea846c79be6cb2d011b635da358f7ecd0a2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053475"
---
# <a name="device-transport-state"></a>Состояние транспорта устройства

Чтобы получить текущее состояние устройства, например воспроизведение, пауза или остановка, вызовите метод [**иамексттранспорт:: Get \_**](/windows/desktop/api/Strmif/nf-strmif-iamexttransport-get_mode) . Метод получает константу, которая указывает состояние устройства:



| Значение                    | Состояние устройства |
|--------------------------|--------------|
| \_Воспроизведение в режиме ED \_           | Воспроизведение         |
| \_точка в режиме ED \_           | Остановить         |
| \_заморозить режим ED \_         | Пауза        |
| ED, \_ режим \_ FF             | Перемотка вперед |
| ED \_ Mode \_ выгру            | Rewind       |
| \_запись в режиме ED \_         | Record       |
| \_закрепление записи в режиме ED \_ \_ | Запись — приостановка |



 

Следующий код проверяет состояние устройства:


```C++
LONG State;
hr = MyDevCap.pTransport->get_Mode(&State);
if (SUCCEEDED(hr))
{
    switch (State)
    {
        case ED_MODE_PLAY:
        // ... 
    }
}
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Управление видеокамерой](controlling-a-dv-camcorder.md)
</dt> </dl>

 

 



