---
title: уианамеленгстулонг
description: уианамеленгстулонг
ms.assetid: 01AF3F1E-9A3F-48B4-8219-6E80BAFC82EE
keywords:
- Идентификатор UIA_NamePropertyId AutomationElement. NameProperty
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: eec235897680cde3b024a67745b923e989cfc68db3b154be260c9dcd3510ba10
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118993974"
---
# <a name="uianamelengthtoolong"></a>уианамеленгстулонг

## <a name="text"></a>Текст

Имя элемента не должно возвращать строку длиннее {0} символа

## <a name="type"></a>Тип

Error

## <a name="description"></a>Описание

Имя элемента содержит слишком много символов. Например, метод [**иуиаутоматионелемент:: куррентнаме**](/windows/desktop/api/UIAutomationClient/nf-uiautomationclient-iuiautomationelement-get_currentname) , используемый для получения имени UIA элемента, возвращает строку, превышающую ограничение.

Эта проблема вызывает проблемы для тех, кто полагается на средство чтения с экрана и клавиатуру для навигации, так как элемент может иметь непонятное имя, не являющееся интуитивно понятным.

## <a name="possible-causes"></a>Возможные причины

Элемент или его родитель имеет неправильно назначенное имя или подпись.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**UIA \_ намепропертид**](uiauto-automation-element-propids.md)
</dt> <dt>

[**Иуиаутоматионелемент:: Куррентнаме**](/windows/desktop/api/UIAutomationClient/nf-uiautomationclient-iuiautomationelement-get_currentname)
</dt> </dl>

 

 




