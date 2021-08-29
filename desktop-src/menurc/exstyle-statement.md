---
title: ОПЕРАТОРЕ EXSTYLE, инструкция
description: Определяет расширенные стили окна для диалогового окна. В определении ресурса инструкция ОПЕРАТОРЕ EXSTYLE помещается с необязательными инструкциями перед началом тела определения ресурса.
ms.assetid: 5dc74bab-e385-457c-80c4-5e04eed589b5
keywords:
- Меню инструкций ОПЕРАТОРЕ EXSTYLE и другие ресурсы
topic_type:
- apiref
api_name:
- EXSTYLE
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5b0d09d577a829350cb7df5179dbbb85e867648ab809c84d66f4eafaecad1da5
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119663054"
---
# <a name="exstyle-statement"></a>ОПЕРАТОРЕ EXSTYLE, инструкция

Определяет расширенные стили окна для диалогового окна. В определении ресурса инструкция **операторе EXSTYLE** помещается с необязательными инструкциями перед началом тела определения ресурса.

``` syntax
EXSTYLE extended-style
```

<dl> <dt>

<span id="extended-style"></span><span id="EXTENDED-STYLE"></span>*Расширенный стиль*
</dt> <dd>

Расширенный стиль окна для диалогового окна или элемента управления. Список расширенных стилей окон см. в разделе [**Расширенные стили окон**](/windows/desktop/winmsg/extended-window-styles).

</dd> </dl>

## <a name="remarks"></a>Remarks

Для элементов управления расширенные стили задаются после параметра *Style* в операторе Control Resource-Definition. Дополнительные сведения см. в описании инструкции Resource-Definition для отдельного элемента управления.

## <a name="see-also"></a>См. также

<dl> <dt>

[**Accelerator**](accelerators-resource.md)
</dt> <dt>

[**ЭЛЕМЕНТА**](control-control.md)
</dt> <dt>

[**Откроется**](dialog-resource.md)
</dt> <dt>

[**МЕНЮ**](menu-resource.md)
</dt> <dt>

[**ПОДСКАЗКИ**](popup-resource.md)
</dt> <dt>

[**RCDATA**](rcdata-resource.md)
</dt> <dt>

[**STRINGTABLE**](stringtable-resource.md)
</dt> <dt>

[Определяемый пользователем ресурс](user-defined-resource.md)
</dt> </dl>

 

 