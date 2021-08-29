---
title: Конфиденцетекст, свойство
description: Конфиденцетекст, свойство
ms.assetid: ff856af7-c5ad-4970-8778-b59a76c5e276
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 0b6612d4ade657748674fb4dd7391f447849691dcd756f2320f590c00ac33430
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119963154"
---
# <a name="confidencetext-property"></a>Конфиденцетекст, свойство

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

<dl> <dt>

<span id="Description"></span><span id="description"></span><span id="DESCRIPTION"></span>**Nописание**
</dt> <dd>

Возвращает или задает **конфиденцетекст** клиента, который отображается в Tip прослушивания.

</dd> <dt>

<span id="Syntax"></span><span id="syntax"></span><span id="SYNTAX"></span>**Syntax**
</dt> <dd>

*Агент ***. Символы ("**_чарактерид_*_"). Команды ("_*_имя_*_")_*.  \[ Конфиденцетекст  =  *строка*\]



| Часть     | Описание                                                                                                           |
|----------|-----------------------------------------------------------------------------------------------------------------------|
| *строка* | Строковое выражение, результатом которого является текст для **Конфиденцетекст** [**команды**](/windows/desktop/lwef/the-command-object). |



 

</dd> </dl>

## <a name="remarks"></a>Remarks

Если возвращенное значение достоверности наилучшего соответствия (UserInput. достоверность) не превышает параметр [**достоверности**](confidence-property.md) , сервер отображает текст, указанный в **конфиденцетекст** , в подсказке прослушивания.

 

 