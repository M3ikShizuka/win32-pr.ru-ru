---
title: Перечисление списков воспроизведения синхронизации
description: Перечисление списков воспроизведения синхронизации
ms.assetid: 830c3ea5-2937-48b5-b89f-ef68a6649ca3
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
- списки воспроизведения синхронизации, перечисление
- переносные устройства, перечисление
- перечисления, списки воспроизведения синхронизации
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 29679380cec1844e9a790ac4ff047bfa4bf05288
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127243250"
---
# <a name="enumerating-synchronization-playlists"></a>Перечисление списков воспроизведения синхронизации

В следующем примере кода создается функция, которая заполняет элемент управления ListView списками воспроизведения. Первыми отображаются списки воспроизведения синхронизации. Списки воспроизведения синхронизации для текущего выбранного устройства отмечены галочкой и сортируются в порядке приоритета синхронизации. Все остальные списки воспроизведения не отмечены флажками.

Элемент управления ListView настроен для выбора только одного элемента. Порядок списков воспроизведения в элементе управления ListView определяет приоритет синхронизации. Состояние проверки отдельного списка воспроизведения определяет, является ли он списком синхронизации для текущего выбранного устройства.

Параметр *лпсиндекс* указывает индекс партнерства для выбранного в данный момент портативного устройства.


```C++
STDMETHODIMP CSyncSettings::ShowPlaylists(long lPSIndex)
{ 
    HRESULT hr = S_OK; 
    ATLASSERT(m_pMainDlg);
   
    CComPtr<IWMPMediaCollection> spMediaCollection;
    CComPtr<IWMPPlaylist> spPlaylist; // Contains a playlist of all playlists.
    long lSyncItemCount= 0; // Count of items selected for synchronization. 

    ListView_DeleteAllItems(m_hPlView);

    m_spPlaylist.Release();
   
    if(lPSIndex == 0)
    {
        return S_OK;
    } 

    HCURSOR hCursor = LoadCursor(NULL, IDC_WAIT);
    HCURSOR hCursorOld = SetCursor(hCursor);

    if(SUCCEEDED(hr))
    {
        // Retrieve a pointer to IWMPMediaCollection.
        hr = m_spPlayer->get_mediaCollection(&spMediaCollection);
    }

    if(SUCCEEDED(hr) && spMediaCollection)
    {
        // Retrieve a playlist filled with IWMPMedia items.
        // Each IWMPMedia represents an individual playlist 
        // in the library.
        hr = spMediaCollection->getByAttribute(CComBSTR("MediaType"), CComBSTR("playlist"), &spPlaylist);
    }
 
    if(SUCCEEDED(hr) && spPlaylist)
    {  
        // Get the sync attribute name for the current device.
        CComBSTR bstrAttribute(g_szSyncAttributeNames[lPSIndex]);

        // Sort the playlist.
        // lSyncItemCount is the count of synchronization playlists.
        hr = SortPlaylist(spPlaylist, bstrAttribute, &lSyncItemCount);
     
        if(SUCCEEDED(hr))
        {
            m_spPlaylist = spPlaylist;  // Cache the playlist.

            long lCount = 0;
            spPlaylist->get_count(&lCount);
             
            // Fill the ListView control.
            for(long i = 0; i < lCount; i++)
            {
                CComPtr<IWMPMedia> spMedia;
                CComBSTR bstrPlaylistName;
                CComBSTR bstrVal; // Value of the SyncXX attribute.

                // Retrieve a playlist.
                hr = spPlaylist->get_item(i, &spMedia);

                if(SUCCEEDED(hr) && spMedia)
                {
                    // Get the name.
                    hr = spMedia->get_name(&bstrPlaylistName);
                }  
                if(SUCCEEDED(hr) && spMedia)
                {      
                    // Get the SyncXX attribute value.
                    hr = spMedia->getItemInfo(bstrAttribute, &bstrVal);
                }

                if(SUCCEEDED(hr) && bstrPlaylistName.Length())
                {
                    // Insert the item in the ListView control.
                    LVITEM lvI;
                    ZeroMemory(&lvI, sizeof(LVITEM));
                    lvI.mask = LVIF_TEXT; 
                    lvI.lParam = _wtol(bstrVal);
                    lvI.iItem = ListView_GetItemCount(m_hPlView);
                    lvI.pszText = "";
                    ListView_InsertItem(m_hPlView, &lvI);

                    // If this is a sync playlist, mark the check box.
                    if(i < lSyncItemCount)
                    {
                        ListView_SetCheckState(m_hPlView, i, TRUE);
                    }

                    // Display the playlist name.
                    lvI.iSubItem = 1;
                    lvI.pszText = COLE2T(bstrPlaylistName);
                    ListView_SetItem(m_hPlView, &lvI);
                }
            }
        }        
    }

    SetCursor(hCursorOld);
    return hr;
}
```



Сведения о реализации функции Сортплайлист см. в разделе [Сортировка списков воспроизведения по приоритету синхронизации](sorting-playlists-by-synchronization-priority.md).

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Ивмпмедиа:: getItemInfo**](/previous-versions/windows/desktop/api/wmp/nf-wmp-iwmpmedia-getiteminfo)
</dt> <dt>

[**Ивмпмедиаколлектион:: Жетбяттрибуте**](/previous-versions/windows/desktop/api/wmp/nf-wmp-iwmpmediacollection-getbyattribute)
</dt> <dt>

[**Управление списками воспроизведения синхронизации**](managing-synchronization-playlists.md)
</dt> <dt>

[**Атрибуты синхронизации**](sync-attributes.md)
</dt> </dl>

 

 




