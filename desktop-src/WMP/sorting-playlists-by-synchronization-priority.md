---
title: Сортировка списков воспроизведения по приоритету синхронизации
description: Сортировка списков воспроизведения по приоритету синхронизации
ms.assetid: 0f7f1ed3-0639-47bf-bf8e-52ae0a1d7ab2
keywords:
- проигрыватель Windows Media, списки воспроизведения синхронизации
- объектная модель проигрыватель Windows Media, списки воспроизведения синхронизации
- Объектная модель, списки воспроизведения синхронизации
- проигрыватель Windows Media Мобильные устройства, списки синхронизации
- проигрыватель Windows Media ActiveX элемент управления, списки воспроизведения синхронизации
- проигрыватель Windows Media управление мобильными ActiveXми, списки воспроизведения синхронизации
- элемент управления ActiveX, списки воспроизведения синхронизации
- списки воспроизведения, синхронизация
- списки воспроизведения метафайлов, синхронизация
- Windows Списки воспроизведения мультимедийных метафайлов, синхронизация
- переносные устройства, сортировка списков воспроизведения синхронизации
- синхронизации списков воспроизведения, сортировка
- списки воспроизведения синхронизации, приоритеты
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f2460dd9a0046074aa1cc4e26cb32ef7179537ced623b28a3243eca4e8f99bbd
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119763444"
---
# <a name="sorting-playlists-by-synchronization-priority"></a>Сортировка списков воспроизведения по приоритету синхронизации

В следующем коде выполняется простая Сортировка списков воспроизведения. Вы можете увидеть, как эта функция используется в примере кода в разделе [Перечисление списков воспроизведения синхронизации](enumerating-synchronization-playlists.md). Функция принимает следующие параметры:

-   *пплайлист*. указатель на проигрыватель Windows Media список воспроизведения для сортировки. Элементы мультимедиа в списке воспроизведения должны указывать на другие списки воспроизведения, а не отдельные цифровые файлы мультимедиа.
-   *бстрсинкаттрибуте*. Значение типа BSTR, содержащее имя атрибута партнерства синхронизации для текущего устройства ("Sync01", "Sync02" и т. д.).
-   *плселектед*. Указатель на **длинную** переменную, которая получает число списков воспроизведения синхронизации.

Функция проверяет атрибут партнерства синхронизации для каждого элемента мультимедиа (представляющего список воспроизведения) в списке воспроизведения, указанном параметром *пплайлист*. Если атрибут имеет ненулевое значение, код перемещает элемент мультимедиа в начало списка воспроизведения и вставляет его в порядок приоритета.

По завершении функция возвращает количество элементов мультимедиа (списков воспроизведения синхронизации) с ненулевым значением для атрибута партнерства синхронизации.


```C++
STDMETHODIMP CSyncSettings::SortPlaylist(IWMPPlaylist *pPlaylist, BSTR bstrSyncAttribute, long *plSelected)
{
    HRESULT hr = S_OK;
    long lSyncItemCount = 0;

    ATLASSERT (pPlaylist);
    ATLASSERT (plSelected);

    // Local copies of the parameters.
    CComPtr<IWMPPlaylist> spPlaylist(pPlaylist);
    CComBSTR bstrAttribute(bstrSyncAttribute);

    ATLASSERT (bstrAttribute.Length());

    // Get the count of playlist media items.
    long lCount = 0;
    spPlaylist->get_count(&lCount);

    // Walk the playlist.
    for(long i = 0; i < lCount; i++)
    {
        CComPtr<IWMPMedia> spMedia;                 
        CComBSTR bstrVal;            
        long lPriority = 0;
        
        hr = spPlaylist->get_item(i, &spMedia);

        if(SUCCEEDED(hr) && spMedia)
        {      
            // Get the sync priority value as a string.
            hr = spMedia->getItemInfo(bstrAttribute, &bstrVal);
        }

        if(SUCCEEDED(hr) && spMedia)
        {
            // Convert sync priority to a long number.
            lPriority = _wtol(bstrVal);
        }

        // Sort the playlist.
        // Only move the current item if it has a
        // sync priority value.
        if(lPriority > 0)
        {
            lSyncItemCount++;

            // Walk down the list and insert the item
            // in ascending order.
            for(long j = 0; j < lCount; j++)
            {
                CComPtr<IWMPMedia> spMediaCompare;
                CComBSTR bstrValCompare;
                long lPriorityTest = 0;

                hr = spPlaylist->get_item(j, &spMediaCompare);

                if(SUCCEEDED(hr) && spMediaCompare.p)
                {
                    hr = spMediaCompare->getItemInfo(bstrAttribute, &bstrValCompare);
                }
                if(SUCCEEDED(hr) && spMediaCompare.p)
                {
                    lPriorityTest = _wtol(bstrValCompare);
                    
                    if(lPriority <= lPriorityTest || 
                        0 == lPriorityTest)
                    {
                        hr = spPlaylist->moveItem(i, j);
                        break;                            
                    }                        
                } 
            } // for j                       
        } // if(lPriority > 0)          
    } // for i  
  
    // Return the sync item count.
    *plSelected = lSyncItemCount;

    return hr;
}
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Ивмпмедиа:: getItemInfo**](/previous-versions/windows/desktop/api/wmp/nf-wmp-iwmpmedia-getiteminfo)
</dt> <dt>

[**Ивмпплайлист:: получение \_ элемента**](/previous-versions/windows/desktop/api/wmp/nf-wmp-iwmpplaylist-get_item)
</dt> <dt>

[**Ивмпплайлист:: Мовеитем**](/previous-versions/windows/desktop/api/wmp/nf-wmp-iwmpplaylist-moveitem)
</dt> <dt>

[**Управление списками воспроизведения синхронизации**](managing-synchronization-playlists.md)
</dt> <dt>

[**Атрибуты синхронизации**](sync-attributes.md)
</dt> </dl>

 

 




