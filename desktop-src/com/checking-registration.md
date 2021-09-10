---
title: Проверка регистрации
description: Проверка регистрации
ms.assetid: 7df63955-d838-4518-8473-0c1a24e90f69
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ee215fd052ffc242900eead069a8b72fd25b31d5
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369674"
---
# <a name="checking-registration"></a>Проверка регистрации

При каждой загрузке приложения необходимо проверить его регистрацию, чтобы определить следующее:

-   Содержатся ли в реестре идентификаторы CLSID. Если они отсутствуют, приложение должно зарегистрироваться в качестве исходной установки.
-   Имеются ли в регистре CLSID приложения, но не имеющие в них сведений, относящихся к OLE 2. В этом случае приложение должно зарегистрироваться в качестве исходной установки.
-   Указывает, указывают ли путь, содержащий записи сервера ([локалсервер](localserver.md) и [LocalServer32](localserver32.md), [Инпроксервер](inprocserver.md) и [InprocServer32](inprocserver32.md), и [дефаултикон](defaulticon.md)), на расположение, в котором приложение в настоящий момент установлено. Если путь не имеет, перепишите записи пути, чтобы они указывали на текущее расположение.

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Регистрация приложений COM](registering-com-applications.md)
</dt> </dl>

 

 




