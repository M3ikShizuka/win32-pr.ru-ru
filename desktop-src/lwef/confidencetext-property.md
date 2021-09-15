---
title: Конфиденцетекст, свойство
description: Конфиденцетекст, свойство
ms.assetid: ff856af7-c5ad-4970-8778-b59a76c5e276
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: eb30b5ac481b6011d3575ab99dbc389f426b085d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127567563"
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

## <a name="remarks"></a>Комментарии

Если возвращенное значение достоверности наилучшего соответствия (UserInput. достоверность) не превышает параметр [**достоверности**](confidence-property.md) , сервер отображает текст, указанный в **конфиденцетекст** , в подсказке прослушивания.

 

 