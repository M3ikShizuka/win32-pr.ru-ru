---
title: Поддержка элементов обратного вызова
description: В этом разделе показано, как обеспечить поддержку элементов обратного вызова.
ms.assetid: BD32666F-9445-4871-AE21-5DC9F5FC9C1B
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 056f64c086aeda94ccf928d93ae2c5db5e2187a4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127166963"
---
# <a name="how-to-support-callback-items"></a>Поддержка элементов обратного вызова

В этом разделе показано, как обеспечить поддержку элементов обратного вызова.

## <a name="what-you-need-to-know"></a>Это важно знать

### <a name="technologies"></a>Технологии

-   [Windows Элементы управления](window-controls.md)

### <a name="prerequisites"></a>Предварительные требования

-   C/C++
-   Windows Программирование пользовательского интерфейса

## <a name="instructions"></a>Instructions


Если приложение будет использовать элементы обратного вызова в элементе управления ComboBoxEx, необходимо подготовиться к обработке кода уведомления [ \_ жетдиспинфо кбен](cben-getdispinfo.md) . Элемент управления ComboBoxEx отправляет это уведомление каждый раз, когда ему нужен владелец для предоставления конкретных сведений об элементе. Дополнительные сведения об элементах обратного вызова см. в разделе [элементы обратного](comboboxex-controls.md)вызова.

Следующая определяемая приложением функция обрабатывает [кбен \_ жетдиспинфо](cben-getdispinfo.md) , предоставляя атрибуты для данного элемента. Обратите внимание, что он устанавливает для элемента **маски** входящей [**КОМБОБОКСЕКСИТЕМ**](/windows/win32/api/commctrl/ns-commctrl-comboboxexitema) структуры значение кбеиф \_ di \_ сетитем. Если задать **маску** для этого значения, элемент управления будет хранить сведения об элементе, чтобы не запрашивать эти сведения еще раз.

## <a name="complete-example"></a>Полный пример


```C++
// DoItemCallback - Processes CBEN_GETDISPINFO by providing item
// attributes for a given callback item.

void WINAPI DoItemCallback(PNMCOMBOBOXEX pNMCBex)
{
    DWORD dwMask = pNMCBex->ceItem.mask;

    if(dwMask & CBEIF_TEXT)
    {
            // Insert code to provide item text.
    }

    if(dwMask & CBEIF_IMAGE) 
    {
        // Insert code to provide an item image index.
    }

    // Insert code to provide other callback information as desired.

    // Make the ComboBoxEx control hold onto the item information.
    pNMCBex->ceItem.mask = CBEIF_DI_SETITEM;
}
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Сведения об элементах управления ComboBoxEx](comboboxex-controls.md)
</dt> <dt>

[Справочник по элементу управления ComboBoxEx](bumper-comboboxex-comboboxex-control-reference.md)
</dt> <dt>

[Использование элементов управления ComboBoxEx](/windows/desktop/Controls/using-comboboxex)
</dt> <dt>

[ComboBoxEx](comboboxex-control-reference.md)
</dt> </dl>

 

 