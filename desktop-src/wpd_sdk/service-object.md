---
description: Объект службы
ms.assetid: 4ce4e7f7-579d-41a5-a4e1-935ba0afce83
title: Объект службы
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 7a3aabfc4e4366c54a5d30dbe5825f178378133d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572043"
---
# <a name="service-object"></a>Объект службы

Объект службы должен поддерживать следующие свойства.



| Имя свойства                                                                                                                      | Обязательный или необязательный                                                                  |
|------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------|
| [\_идентификатор объекта \_ WPD](/previous-versions/windows/hardware/drivers/ff597893(v=vs.85))                                                         | Обязательный элемент. .                                                                           |
| [\_ \_ идентификатор родительского объекта \_ WPD](/previous-versions/windows/hardware/drivers/ff597893(v=vs.85))                                   | Обязательный элемент.                                                                             |
| [\_имя объекта \_ WPD](/previous-versions/windows/hardware/drivers/ff597893(v=vs.85))                                                   | Обязательный элемент.                                                                             |
| [\_ \_ Постоянный \_ уникальный идентификатор объекта \_ WPD](/previous-versions/windows/hardware/drivers/ff597893(v=vs.85)) | Обязательный элемент.                                                                             |
| [\_объект WPD \_](/previous-versions/windows/hardware/drivers/ff597893(v=vs.85))                                       | Требуется, если объект службы не должен отображаться для пользователя.                       |
| [\_система объектов \_ WPD](/previous-versions/windows/hardware/drivers/ff597893(v=vs.85))                                       | Требуется, если объект является системным объектом (например, он представляет системный файл). |
| [\_Категория функционального \_ объекта WPD \_](/previous-versions/windows/hardware/drivers/ff597893(v=vs.85))     | Обязательный элемент. Представляет тип службы устройства, например Контакты службы.          |
| [\_версия службы \_ WPD](/previous-versions/windows/hardware/drivers/ff597893(v=vs.85))                                       | Обязательный элемент.                                                                             |
| [\_тип хранилища \_ WPD](/previous-versions/windows/hardware/drivers/ff597893(v=vs.85))                                                | Требуется, если служба используется для хранения объектов.                                     |
| [\_емкость хранилища \_ WPD](/previous-versions/windows/hardware/drivers/ff597865(v=vs.85))                                    | Требуется, если служба используется для хранения объектов.                                     |



 

## <a name="typical-resources"></a>Типичные ресурсы

Обычно эти объекты не размещают ресурсы.

## <a name="typical-formats"></a>Стандартные форматы

В следующем списке приведены типичные форматы, используемые объектом службы. Однако этот объект не ограничен этими форматами.

-   \_Формат объекта WPD не \_ \_ указан

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Требования к объектам**](requirements-for-objects.md)
</dt> </dl>

 

 
