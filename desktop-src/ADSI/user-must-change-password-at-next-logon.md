---
title: Пользователь должен сменить пароль при следующем входе в систему (поставщик LDAP)
description: Чтобы заставить пользователя Сменить пароль при следующем входе в систему, присвойте атрибуту pwdLastSet значение 0. Чтобы удалить это требование, присвойте атрибуту pwdLastSet значение-1. Атрибуту pwdLastSet не может быть присвоено любое другое значение, кроме системы.
ms.assetid: 0182151c-ddb7-4d08-98c6-c37e6e514cf0
ms.tgt_platform: multiple
keywords:
- Пользователь должен сменить пароль при следующем входе в систему ADSI, поставщик LDAP
- ADSI поставщика LDAP, примеры управления пользователями, пользователь должен сменить пароль при следующем входе в систему
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 784ee0defbe3c8ec9abe2d110c2532b8c9688019
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065821"
---
# <a name="user-must-change-password-at-next-logon-ldap-provider"></a>Пользователь должен сменить пароль при следующем входе в систему (поставщик LDAP)

Чтобы заставить пользователя Сменить пароль при следующем входе в систему, присвойте атрибуту **pwdLastSet** значение 0. Чтобы удалить это требование, присвойте атрибуту **pwdLastSet** значение-1. Атрибуту **pwdLastSet** не может быть присвоено любое другое значение, кроме системы.

В следующем примере кода показано, как задать параметр "Требовать смену пароля при следующем входе в систему".


```VB
Dim usr as IADs

Set usr = GetObject("LDAP://CN=Jeff Smith,OU=Sales,DC=Fabrikam,DC=Com")
usr.Put "pwdLastSet", CLng(0)
usr.SetInfo
```



В следующем примере кода показано, как задать параметр "Требовать смену пароля при следующем входе в систему".


```C++
/***************************************************************************

    SetUserMustChangePassword()

***************************************************************************/

HRESULT SetUserMustChangePassword(LPCWSTR pwszUserADsPath, 
                                  LPCWSTR pwszUsername, 
                                  LPCWSTR pwszPassword)
{
    IADs *pUser;
    HRESULT hr;

    hr = ADsOpenObject(pwszUserADsPath,
                        pwszUsername,
                        pwszPassword,
                        ADS_SECURE_AUTHENTICATION,
                        IID_IADs,
                        (void**)&pUser);

    if(SUCCEEDED(hr))
    {
        VARIANT var;
        VariantInit(&var);
        V_I4(&var) = 0;
        V_VT(&var) = VT_I4;
        hr = pUser->Put(CComBSTR("pwdLastSet"), var);
        hr = pUser->SetInfo();

        VariantClear(&var);
        pUser->Release();
    }

    return hr;
}
```



 

 




