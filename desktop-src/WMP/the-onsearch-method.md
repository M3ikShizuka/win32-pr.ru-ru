---
title: Метод onSearch
description: Метод onSearch
ms.assetid: 709bb428-1a5e-4b8d-8622-5fcc816f0a1a
keywords:
- проигрыватель Windows Media подключаемые модули, метод onsearch
- подключаемые модули, метод onSearch
- подключаемые модули пользовательского интерфейса, метод onSearch
- Подключаемые модули пользовательского интерфейса, метод onSearch
- Метод onSearch
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: de5c33af434028e6ee72c757c8d71def0d4109fd
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127568210"
---
# <a name="the-onsearch-method"></a>Метод onSearch

метод onsearch вызывается проигрыватель Windows Media при нажатии кнопки **поиска** . Этот метод извлекает текущий объект **мультимедиа** и передает его методу лаунчпаже.

Для реализации этого метода используется следующий код:


```C++
LRESULT OnSearch(WORD wNotifyCode, WORD wID, HWND hwndCtl, BOOL& fHandled)
{
    HRESULT hr;
    CComPtr<IWMPMedia> spMedia;

    if( m_pPlugin && m_pPlugin->m_spCore )
    {
        // Get a pointer to the current media item.
        hr = m_pPlugin->m_spCore->get_currentMedia(&spMedia);
        if (SUCCEEDED(hr) && spMedia)
        {
            LaunchPage(spMedia);
        }
    else
        {
            MessageBox(_T("There is no media loaded."), _T("Warn"), MB_OK | MB_ICONWARNING);
        }
    }
    return 0;
}

```



## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[**Реализация Кплугинвиндов**](implementing-cpluginwindow.md)
</dt> </dl>

 

 




