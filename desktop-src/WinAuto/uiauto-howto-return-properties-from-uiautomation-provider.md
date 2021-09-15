---
title: Как вернуть свойства от поставщика автоматизации пользовательского интерфейса
description: Этот раздел содержит пример кода, демонстрирующий, как поставщик автоматизации пользовательского интерфейса Майкрософт возвращает свойства элемента пользовательского интерфейса клиентским приложениям.
ms.assetid: 6932de16-5548-4aa3-9f29-5daa57bb202b
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4133a53df3c59e6d5c93b1c9cd8e6aa942b4bd56
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127567278"
---
# <a name="how-to-return-properties-from-a-ui-automation-provider"></a>Как вернуть свойства от поставщика автоматизации пользовательского интерфейса

Этот раздел содержит пример кода, демонстрирующий, как поставщик автоматизации пользовательского интерфейса Майкрософт возвращает свойства элемента пользовательского интерфейса клиентским приложениям.

Чтобы получить значение свойства от поставщика, модель автоматизации пользовательского интерфейса вызывает реализацию метода [**иравелементпровидерсимпле:: жетпропертивалуе**](/windows/desktop/api/UIAutomationCore/nf-uiautomationcore-irawelementprovidersimple-getpropertyvalue) поставщика, передавая идентификатор получаемого свойства и указатель на структуру [**Variant**](/windows/win32/api/oaidl/ns-oaidl-variant) . Если поставщик поддерживает указанное свойство, он копирует тип данных и значение свойства в структуру **Variant** . Если свойство не поддерживается, поставщик устанавливает для элемента **VT** в структуре **Variant** значение VT \_ Empty.


```C++
IFACEMETHODIMP Provider::GetPropertyValue(PROPERTYID propertyId, VARIANT* pRetVal)
{
    // The Name property is typically the same as the Caption property of the 
    // control window, if it has one. Here, the Name is overridden for the 
    // sake of illustration. 
    if (propertyId == UIA_NamePropertyId) 
    {
        pRetVal->vt = VT_BSTR;
        pRetVal->bstrVal = SysAllocString(L"Custom button");
    }
    
    else if (propertyId == UIA_ControlTypePropertyId) 
    {
        pRetVal->vt = VT_I4;
        pRetVal->lVal = UIA_ButtonControlTypeId; 
    }

    else if (propertyId == UIA_IsContentElementPropertyId) 
    {
        pRetVal->vt = VT_BOOL;
        pRetVal->lVal = TRUE; 
    }

    else if (propertyId == UIA_IsControlElementPropertyId) 
    {
        pRetVal->vt = VT_BOOL;
        pRetVal->lVal = TRUE; 
    }

    //
    // Return other properties as appropriate for the control type. 
    //

    else
    {
        pRetVal->vt = VT_EMPTY;
        // UI Automation will attempt to get the property from the  
        // provider for window that hosts the control.
    }
    return S_OK;
}
```



## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

**Основные понятия**
</dt> <dt>

[Общие сведения о свойствах автоматизированного пользовательского интерфейса](uiauto-propertiesoverview.md)
</dt> <dt>

[Разделы руководства для поставщиков автоматизации пользовательского интерфейса](uiauto-howto-topics-for-uiautomation-providers.md)
</dt> </dl>

 

 