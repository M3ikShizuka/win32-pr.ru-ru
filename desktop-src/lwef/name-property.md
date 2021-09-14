---
title: Свойство Name (объект characters)
description: Сведения о свойстве Name объекта Characters. не рекомендуется использовать Microsoft Agent на Windows 7.
ms.assetid: vs|msagent|~\pacontrol_2bxm.htm
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 7365550d5d4d4071cf4292e505f16e7047628cf1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127168260"
---
# <a name="name-property-characters-object"></a>Свойство Name (объект characters)

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

<dl> <dt>

<span id="Description"></span><span id="description"></span><span id="DESCRIPTION"></span>**Nописание**
</dt> <dd>

Возвращает или задает строку, указывающую имя по умолчанию указанного символа.

</dd> <dt>

<span id="Syntax"></span><span id="syntax"></span><span id="SYNTAX"></span>**Syntax**
</dt> <dd>

*Агент ***. Символы ("**_чарактерид_*_")._ *  \[  =  *Строка* имени\]



| Часть     | Описание                                                                             |
|----------|-----------------------------------------------------------------------------------------|
| *строка* | Строковое значение, соответствующее имени символа (в текущем параметре языка). |



 

</dd> </dl>

## <a name="remarks"></a>Remarks

**Имя** символа может зависеть от параметра [**LanguageID**](languageid-property.md) символа. Имя символа на одном языке может отличаться или использовать другие символы, чем в другом. **Имя** символа по умолчанию для конкретного языка определяется при компиляции символа с помощью редактора символов Microsoft Agent.

Избегайте переименования символа, особенно при его использовании в сценарии, где другие клиентские приложения могут использовать один и тот же символ. Кроме того, агент использует **имя** символа для автоматического создания команд для скрытия и отображения символа.

 

 




