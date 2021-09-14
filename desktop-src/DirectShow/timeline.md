---
description: Сроки
ms.assetid: 6cc36034-224c-4126-873b-0cfeceec9781
title: Сроки
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 10d1f802f12df6ca3469b8283bd4fe8b27e22412
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126891645"
---
# <a name="timeline"></a>Сроки

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

Объект временной шкалы управляет всеми объектами в проекте редактирования видео. Чтобы создать этот объект, вызовите **CoCreateInstance**. Идентификатор класса — CLSID \_ амтимелине.

для чтения Windows файлов мультимедиа™, приложение должно предоставить сертификат программного обеспечения, также называемый ключом. Зарегистрируйте приложение в качестве поставщика ключей через интерфейс **IObjectWithSite** временной шкалы. дополнительные сведения см. [в разделе разблокировка пакета SDK для Windows Media Format](unlocking-the-windows-media-format-sdk.md).

Объект временной шкалы предоставляет следующие интерфейсы:

-   [**иамсетеррорлог**](iamseterrorlog.md)
-   [**иамтимелине**](iamtimeline.md)
-   **IObjectWithSite**
-   **IPersistStream**

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Модель временной шкалы](the-timeline-model.md)
</dt> <dt>

[Создание временной шкалы](constructing-a-timeline.md)
</dt> </dl>

 

 



