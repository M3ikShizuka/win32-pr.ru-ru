---
title: Оператор характеристик
description: Определяет сведения о ресурсе, который может использоваться инструментами, считывающими и записывающими файлы определения ресурсов.
ms.assetid: 07834b02-a36e-40cc-8907-bff6631842f3
keywords:
- Меню операторов характеристик и другие ресурсы
topic_type:
- apiref
api_name:
- CHARACTERISTICS
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: de681785fa2ec815b1edbdda913dd8032f8feb8e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127343702"
---
# <a name="characteristics-statement"></a>Оператор характеристик

Определяет сведения о ресурсе, который может использоваться инструментами, считывающими и записывающими файлы определения ресурсов. Указанное значение **DWORD** отображается вместе с ресурсом в файле Compiled. Res. Однако значение не сохраняется в исполняемом файле и не имеет значимости для системы.

Оператор **характеристик** отображается перед началом тела описания [**ускорителей**](accelerators-resource.md), [**диалогового окна**](dialog-resource.md), [**меню**](menu-resource.md), [**RCDATA**](rcdata-resource.md)или определения ресурса [**STRINGTABLE**](stringtable-resource.md) . Указанное значение применяется только к этому ресурсу.

``` syntax
CHARACTERISTICS dword
```

<dl> <dt>

<span id="dword"></span><span id="DWORD"></span>*DWORD*
</dt> <dd>

Определяемое пользователем значение **DWORD** .

</dd> </dl>

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Accelerator**](accelerators-resource.md)
</dt> <dt>

[**Откроется**](dialog-resource.md)
</dt> <dt>

[**ЯЗЫКЕ**](language-statement.md)
</dt> <dt>

[**МЕНЮ**](menu-resource.md)
</dt> <dt>

[**RCDATA**](rcdata-resource.md)
</dt> <dt>

[**STRINGTABLE**](stringtable-resource.md)
</dt> </dl>

 

 




