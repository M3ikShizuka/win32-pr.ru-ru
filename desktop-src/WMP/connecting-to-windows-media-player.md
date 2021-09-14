---
title: подключение к проигрыватель Windows Media
description: подключение к проигрыватель Windows Media
ms.assetid: c6afbd95-bcf8-438a-b854-776c543a5d51
keywords:
- подключаемые модули проигрыватель Windows Media, записи реестра
- подключаемые модули, записи реестра
- подключаемые модули проигрыватель Windows Media, подключение
- подключаемые модули, подключение
- подключаемые модули обработки цифровых сигналов, подключение
- Подключаемые модули DSP, подключение
- подключаемые модули обработки цифровых сигналов, записи реестра
- Подключаемые модули DSP, записи реестра
- реестр, подключаемые модули DSP
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d8fa0851e271631e2c37bf716c427b5af34ade14
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967746"
---
# <a name="connecting-to-windows-media-player"></a>подключение к проигрыватель Windows Media

проигрыватель Windows Media автоматически подключается к подключаемым модулям DSP, которые были установлены и должным образом зарегистрированы. подключаемые модули DSP должны вызывать [ивмпмедиаплугинрегистрар:: вмпрегистерплайерплугин](/previous-versions/windows/desktop/api/wmpservices/nf-wmpservices-iwmpmediapluginregistrar-wmpregisterplayerplugin) , чтобы создать записи реестра, необходимые для того, чтобы проигрыватель Windows Media распознать подключаемый модуль и вывести его на вкладку **подключаемые** модули диалогового окна параметры. Чтобы удалить записи реестра, созданные с помощью **ивмпмедиаплугинрегистрар:: вмпрегистерплайерплугин**, подключаемый модуль вызывает [Ивмпмедиаплугинрегистрар:: вмпунрегистерплайерплугин](/previous-versions/windows/desktop/api/wmpservices/nf-wmpservices-iwmpmediapluginregistrar-wmpunregisterplayerplugin).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Обзор подключаемого модуля DSP**](dsp-plug-in-developer-overview.md)
</dt> </dl>

 

 




