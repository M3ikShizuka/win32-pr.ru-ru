---
description: Международный вывод текста
ms.assetid: e6cc5169-1a6e-40f8-b616-e76ec919195c
title: Международный вывод текста
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: ee8ba7eb6f1a043bb642945e178f3545bcd51738
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127274752"
---
# <a name="international-text-display"></a>Международный вывод текста

Существует четыре возможных варианта отображения международного текста, что также влечет за собой вывод сложных наборов символов:

-   вызов api Windows текста
-   создание экземпляра Windows стандартных элементов управления "изменить"
-   Создание экземпляров элементов управления Rich Edit
-   Вызов Uniscribe

Описание и преимущества каждого из этих параметров см. в разделе [Параметры отображения текста](https://msdn.microsoft.com/globalization/mt662335) . Затем вы решаете выбрать оптимальный вариант для вашего приложения, основываясь на сложности приложения и его функциях проектирования.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**TextOut**](/windows/win32/api/wingdi/nf-wingdi-textouta)
</dt> <dt>

[**ExtTextOut**](/windows/win32/api/wingdi/nf-wingdi-exttextouta)
</dt> <dt>

[**таббедтекстаут**](/windows/win32/api/winuser/nf-winuser-tabbedtextouta)
</dt> <dt>

[**DrawText**](/windows/win32/api/winuser/nf-winuser-drawtext)
</dt> <dt>

[**жеттаббедтекстекстент**](/windows/win32/api/winuser/nf-winuser-gettabbedtextextenta)
</dt> <dt>

[**GetTextExtentPoint32**](/windows/win32/api/wingdi/nf-wingdi-gettextextentpoint32a)
</dt> <dt>

[**жеттекстекстентекспоинт**](/windows/win32/api/wingdi/nf-wingdi-gettextextentexpointa)
</dt> <dt>

[**Элемент управления "Поле ввода"**](../msi/edit-control.md)
</dt> <dt>

[Расширенное редактирование](../controls/about-rich-edit-controls.md)
</dt> <dt>

[Uniscribe](uniscribe.md)
</dt> </dl>

 

 
