---
title: Оператор STYLE
description: Определяет стиль окна для диалогового окна. Стиль окна определяет, является ли поле всплывающим или дочерним окном.
ms.assetid: 5ede57ad-5fa5-414c-9823-e66994826027
keywords:
- Меню инструкций стилей и другие ресурсы
topic_type:
- apiref
api_name:
- STYLE
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 88d74ced35b6b5a2f6c04004fbd2e161df7ba16ff5111577835b93363291c114
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119886772"
---
# <a name="style-statement"></a>Оператор STYLE

Определяет стиль окна для диалогового окна. Стиль окна определяет, является ли поле всплывающим или дочерним окном.

``` syntax
STYLE style
```

<dl> <dt>

<span id="style"></span><span id="STYLE"></span>*стиль*
</dt> <dd>

Стиль окна. Этот параметр может быть целым числом или сочетанием значений стиля окна (например, **WS \_ Caption** и **WS \_ сисмену**) и значениями стиля диалогового окна (например, **\_ центра DS**).

</dd> </dl>

Список стилей окна см. в разделе [стили окон](/windows/desktop/winmsg/window-styles). Список стилей диалоговых окон см. в разделе [стили шаблонов диалоговых окон](../dlgbox/about-dialog-boxes.md). при использовании значений стиля окна или диалогового окна необходимо включить Windows. h.

 

 