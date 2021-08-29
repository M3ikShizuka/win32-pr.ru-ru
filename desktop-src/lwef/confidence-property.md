---
title: Свойство достоверности
description: Свойство достоверности
ms.assetid: 28a57970-4649-4a9a-9fb2-bf3f0b2f54ce
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f446136ce9711d17adf133dd205741c7812ef1360526a0a2c1c6c86442f13aac
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119716524"
---
# <a name="confidence-property"></a>Свойство достоверности

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

<dl> <dt>

<span id="Description"></span><span id="description"></span><span id="DESCRIPTION"></span>**Nописание**
</dt> <dd>

Возвращает или задает значение, указывающее, отображается ли **достоверность** клиента в Tip прослушивания.

</dd> <dt>

<span id="Syntax"></span><span id="syntax"></span><span id="SYNTAX"></span>**Syntax**
</dt> <dd>

*Агент ***. Символы ("**_чарактерид_*_"). Команды ("_*_имя_*_")_*. * * достоверное* *  \[  =  *число*\]



| Часть     | Описание                                                                                                                        |
|----------|------------------------------------------------------------------------------------------------------------------------------------|
| *Число* | Числовое выражение, результатом которого является длинное целое число, идентифицирующее значение достоверности для [**команды**](/windows/desktop/lwef/the-command-object). |



 

</dd> </dl>

## <a name="remarks"></a>Remarks

Если возвращенное значение достоверности наилучшего соответствия (UserInput. достоверность) не превышает значение, заданное для свойства **достоверности** , то текст, указанный в [**конфиденцетекст**](confidencetext-property.md) , отображается в подсказке прослушивания.

 

 