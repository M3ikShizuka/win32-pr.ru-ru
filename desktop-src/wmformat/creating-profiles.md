---
title: Создание профилей
description: Создание профилей
ms.assetid: af4a8efe-d797-4d19-961d-b917e4c7c81a
keywords:
- Windows Пакет SDK для формата мультимедиа, профили
- профили, создание
- профили, интерфейс Ивмпрофилеманажер
- Ивмпрофилеманажер, создание профилей
- профили, функция Вмкреатепрофилеманажер
- вмкреатепрофилеманажер
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 45eeca9e99e09bd709b7e9fdf1aeffe8d35ca14a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570247"
---
# <a name="creating-profiles"></a>Создание профилей

Во многих случаях потребуется создать пустой профиль для настройки. В других случаях проще изменить существующий профиль, например системный профиль. Дополнительные сведения об использовании системных профилей см. [в разделе Использование системных профилей](using-system-profiles.md).

Создание пустого профиля, готового для настройки, требует наличия объекта диспетчера профилей. Чтобы получить интерфейс [**ивмпрофилеманажер**](/previous-versions/windows/desktop/api/wmsdkidl/nn-wmsdkidl-iwmprofilemanager) объекта диспетчера профилей, вызовите функцию [**вмкреатепрофилеманажер**](/previous-versions/windows/desktop/api/Wmsdkidl/nf-wmsdkidl-wmcreateprofilemanager) .

Чтобы создать пустой профиль, вызовите метод [**ивмпрофилеманажер:: креатимптипрофиле**](/previous-versions/windows/desktop/api/Wmsdkidl/nf-wmsdkidl-iwmprofilemanager-createemptyprofile). при создании пустого профиля задается только версия пакета SDK Windows Media Format, который соответствует профилю. Если нет особой необходимости использовать предыдущую версию, следует всегда использовать последнюю версию. Версия определяет структуру профиля; предыдущие версии не поддерживали некоторые свойства.

В следующем примере кода показано, как создать новый профиль. Чтобы скомпилировать этот код в приложении, включите stdio. h. Дополнительные сведения об использовании этого кода см. [в разделе Использование примеров кода](using-the-code-examples.md).


```C++
HRESULT CreateProfile(IWMProfileManager* pProfileMgr, IWMProfile** ppProfile)
{
    HRESULT hr = S_OK;

    // Create the empty profile.
    hr = pProfileMgr->CreateEmptyProfile(WMT_VER_9_0, ppProfile);
    if(FAILED(hr))
    {
        printf("Could not create the profile.\n");
        return hr;
    }

    return S_OK;
}
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**Интерфейс Ивмпрофиле**](iwmprofile.md)
</dt> <dt>

[**Интерфейс Ивмпрофилеманажер**](/previous-versions/windows/desktop/api/wmsdkidl/nn-wmsdkidl-iwmprofilemanager)
</dt> <dt>

[**Работа с профилями**](working-with-profiles.md)
</dt> </dl>

 

 




