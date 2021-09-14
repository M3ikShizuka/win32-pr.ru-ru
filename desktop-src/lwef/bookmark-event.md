---
title: Событие закладки
description: Событие закладки
ms.assetid: 6733cd4e-2ba0-4cff-b68d-abfea284f748
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 0695ccd04f93eae46eaae66955c84fefb9e0c963
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065856"
---
# <a name="bookmark-event"></a>Событие закладки

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

<dl> <dt>

<span id="Description"></span><span id="description"></span><span id="DESCRIPTION"></span>**Nописание**
</dt> <dd>

Возникает при активации закладки в текстовой строке в речевом коде, заданной приложением.

</dd> <dt>

<span id="Syntax"></span><span id="syntax"></span><span id="SYNTAX"></span>**Syntax**
</dt> <dd>

 Закладка подпрограммы- *агента* \_  **(ByVal** *букмаркид * *)**



| Часть         | Описание                                     |
|--------------|-------------------------------------------------|
| *BookmarkID* | Длинное целое число, определяющее номер закладки. |



 

</dd> </dl>

### <a name="remarks"></a>Remarks

Чтобы указать событие закладки, используйте метод [**говорите**](speak-method.md) с тегом **МРК** в заданном тексте. Дополнительные сведения о тегах см. в разделе Теги вывода речи.

 

 




