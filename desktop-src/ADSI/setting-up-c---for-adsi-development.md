---
title: Настройка Visual C++ 6,0 для разработки с интерфейсом ADSI
description: в этом разделе показано, как настроить C++ в Visual Studio, чтобы можно было разрабатывать приложение ADSI.
ms.assetid: 6f1ab3eb-2e0b-4f3e-b93c-e24c8b3b1a27
ms.tgt_platform: multiple
keywords:
- Настройка C++ для разработки с интерфейсом ADSI
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 77f2350b88402c921d014b0c93756759a1d0f744
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172139"
---
# <a name="setting-up-visual-c-60-for-adsi-development"></a>Настройка Visual C++ 6,0 для разработки с интерфейсом ADSI

систему разработки Microsoft Visual C++ 6,0 можно использовать для разработки корпоративных приложений. Чтобы настроить среду Visual C++ 6,0 для разработки приложения ADSI, выполните следующие действия.

**настройка среды разработки Microsoft Visual C++ 6,0**

1.  Укажите каталог include и Library. Выберите **Сервис \| Параметры**. Перейдите на вкладку **Каталог** и укажите путь к ФАЙЛАМ заголовка ADSI.
2.  Включите в проект файл Активедс. h.
3.  Добавьте файлы Активедс. lib и Адсиид. lib в входные данные компоновщика для вашего проекта.
4.  Начните программировать с помощью ADSI.

войдите в домен Windows. Кроме того, необходимо иметь разрешение на изменение данных в Active Directory. По умолчанию эта привилегия есть у администратора. Чтобы ввести этот пример кода, сделайте следующее:

**Пример Visual C++ приложения: создание пользователя в домене**

1.  Запустите Visual C++ 6,0.
2.  Создайте автономный исполняемый проект. Это может быть либо MFC, ATL, либо консольное приложение.
3.  Выполните описанные выше действия, чтобы настроить проект.
4.  Введите следующий пример кода. Замените строку "LDAP://кН = Users, DC = Fabrikam, DC = com" на значение ADsPath контейнера в вашем домене. Необходимо также заменить имя пользователя "жеффсмис" уникальным именем пользователя в домене.

    ```C++
    #include "stdafx.h"
    #include "activeds.h"

    int main(int argc, char* argv[])
    {
        HRESULT hr;
        IADsContainer *pCont;
        IDispatch *pDisp=NULL;
        IADs *pUser;

         // Initialize COM before calling any ADSI functions or interfaces.
         CoInitialize(NULL);

        hr = ADsGetObject( L"LDAP://CN=users,DC=fabrikam,DC=com", 
                                   IID_IADsContainer, 
                                   (void**) &pCont );
        
        if ( !SUCCEEDED(hr) )
        {
            return 0;
        }

        //-----------------
        // Create a user
        //-----------------
        
        hr = pCont->Create(CComBSTR("user"), CComBSTR("cn=jeffsmith"), &pDisp );
        
        // Release the container object.    
        pCont->Release();
        
        if ( !SUCCEEDED(hr) )
        {
            return 0;
        }

        hr = pDisp->QueryInterface( IID_IADs, (void**) &pUser );

        // Release the dispatch interface.
        pDisp->Release();

        if ( !SUCCEEDED(hr) )
        {    
            return 0;
        }

        // Commit the object data to the directory.
        pUser->SetInfo();

        // Release the object.
        pUser->Release();

        CoUninitialize();
    }
    ```

    

5.  Создайте и запустите приложение. Чтобы убедиться, что пользователь создан, используйте средство управления Active Directory пользователи и компьютеры.

 

 




