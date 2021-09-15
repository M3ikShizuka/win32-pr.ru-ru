---
title: Свойство Caption (объект Command)
description: Сведения о свойстве Caption объекта Command. не рекомендуется использовать Microsoft Agent на Windows 7.
ms.assetid: 8dcdf3e0-3111-438b-9d39-ba9a36437ad2
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a0eb41def3b183fe4185b9c66a9ca5cd172372fb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127567598"
---
# <a name="caption-property-command-object"></a>Свойство Caption (объект Command)

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

<dl> <dt>

<span id="Description"></span><span id="description"></span><span id="DESCRIPTION"></span>**Nописание**
</dt> <dd>

Определяет текст, отображаемый для [**команды**](/windows/desktop/lwef/the-command-object) во всплывающем меню указанного символа.

</dd> <dt>

<span id="Syntax"></span><span id="syntax"></span><span id="SYNTAX"></span>**Syntax**
</dt> <dd>

*Агент ***. Символы ("**_чарактерид_*_"). Команды ("_*_имя_*_")._ *  \[  =  *Строка* заголовка\]



| Часть     | Описание                                                                                  |
|----------|----------------------------------------------------------------------------------------------|
| *строка* | Строковое выражение, результатом которого является текст, отображаемый в качестве заголовка для **команды**. |



 

</dd> </dl>

## <a name="remarks"></a>Комментарии

Чтобы указать клавишу доступа (нелинованной) для **заголовка**, добавьте символ амперсанда (&) перед этим символом.

Если вы не определили **воицекаптион** для команды, будет использоваться параметр **Caption** .

 

 
