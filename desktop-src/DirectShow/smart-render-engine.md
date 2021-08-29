---
description: Модуль интеллектуального просмотра
ms.assetid: 279be879-9728-4fa1-bdf7-6b48485fc75f
title: Модуль интеллектуального просмотра
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b3472d096d1c3918a9bf1a45ae788a535fd65bfe4e4084c6b044516db01440d5
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119072558"
---
# <a name="smart-render-engine"></a>Модуль интеллектуального просмотра

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

Объект интеллектуального модуля отрисовки визуализирует выходные данные из временной шкалы. Чтобы создать этот объект, вызовите **CoCreateInstance**. Для несжатых выходных данных используйте базовый механизм визуализации. Идентификатор класса — CLSID \_ смартрендеренгине.

Модуль интеллектуального просмотра предоставляет следующие интерфейсы:

-   [**иамсетеррорлог**](iamseterrorlog.md)
-   **IObjectWithSite**
-   [**ирендеренгине**](irenderengine.md)
-   [**IRenderEngine2**](irenderengine2.md)
-   [**исмартрендеренгине**](ismartrenderengine.md)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Подготовка Project](rendering-a-project.md)
</dt> <dt>

[Базовый механизм визуализации](basic-render-engine.md)
</dt> </dl>

 

 



