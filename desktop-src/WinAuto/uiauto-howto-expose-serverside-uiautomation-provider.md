---
title: Как предоставить поставщик автоматизации пользовательского интерфейса Server-Side
description: Этот раздел содержит пример кода, показывающий, как предоставить поставщик автоматизации пользовательского интерфейса Майкрософт на стороне сервера для пользовательского элемента управления.
ms.assetid: 68bf16c7-fbab-478a-97be-47d1195028f3
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c5af3fa9e663bc737df95015db94cdedc1073ab9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127058469"
---
# <a name="how-to-expose-a-server-side-ui-automation-provider"></a>Как предоставить поставщик автоматизации пользовательского интерфейса Server-Side

Этот раздел содержит пример кода, показывающий, как предоставить поставщик автоматизации пользовательского интерфейса Майкрософт на стороне сервера для пользовательского элемента управления.

Служба автоматизации пользовательского интерфейса Майкрософт отправляет сообщение [**WM \_ GetObject**](wm-getobject.md) в приложение поставщика для получения сведений о доступном объекте, поддерживаемом поставщиком. Автоматизация пользовательского интерфейса **отправляет \_ объект WM GetObject** , когда клиент [**вызывает иуиаутоматион:: Елементфромхандле**](/windows/desktop/api/UIAutomationClient/nf-uiautomationclient-iuiautomation-elementfromhandle), [**елементфромпоинт**](/windows/desktop/api/UIAutomationClient/nf-uiautomationclient-iuiautomation-elementfrompoint)и [**GetFocusedElement**](/windows/desktop/api/UIAutomationClient/nf-uiautomationclient-iuiautomation-getfocusedelement), а также при обработке событий, для которых зарегистрирован клиент.

Когда поставщик получает сообщение [**WM \_ GetObject**](wm-getobject.md) , он должен проверить, равен ли параметр *lParam* значению **уиарутобжектид**. Если это так, поставщик должен вернуть интерфейс [**иравелементпровидерсимпле**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-irawelementprovidersimple) объекта. Поставщик возвращает интерфейс путем вызова функции [**уиаретурнравелементпровидер**](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-uiareturnrawelementprovider) .

В следующем примере показано, как реагировать на [**WM \_ GetObject**](wm-getobject.md).


```C++
    // Expose the custom button's server-side provider to UI Automation.
    case WM_GETOBJECT:
        {
            // If lParam matches UiaRootObjectId, return IRawElementProviderSimple.
            if (static_cast<long>(lParam) == static_cast<long>(UiaRootObjectId))
            {
                // Retrieve the pointer to the custom button object from the
                // window data.
                CustomButton* pControl = reinterpret_cast<CustomButton*>(
                    GetWindowLongPtr(hwnd, GWLP_USERDATA));

                // Call an application-defined method to get the
                // IRawElementProviderSimple pointer.
                IRawElementProviderSimple* pRootProvider = 
                    pControl->GetUIAutomationProvider(hwnd);

                // Return the IRawElementProviderSimple pointer to UI Automation.
                return UiaReturnRawElementProvider(hwnd, wParam, lParam, 
                    pRootProvider);
            }
            return 0;
        }
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

**Основные понятия**
</dt> <dt>

[Реализация поставщика автоматизации пользовательского интерфейса Server-Side](uiauto-serversideprovider.md)
</dt> <dt>

[Сообщение WM \_ GetObject](the-wm-getobject-message.md)
</dt> <dt>

[Разделы руководства для поставщиков автоматизации пользовательского интерфейса](uiauto-howto-topics-for-uiautomation-providers.md)
</dt> </dl>

 

 




