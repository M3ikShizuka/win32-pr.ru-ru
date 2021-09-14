---
title: Загрузка и регистрация библиотеки типов
description: Библиотека динамической компоновки службы автоматизации, Oleaut32.dll, предоставляет несколько функций, которые можно вызывать для загрузки и регистрации библиотеки типов. Вызов Лоадтипелибекс, как показано в следующем примере, обе загружают библиотеку и создает записи реестра.
ms.assetid: b7404919-fa0a-4de8-8c85-41b7bc7c5a52
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c5d533225913d6bcfbb74df3ac42bd00b18b00e4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127249268"
---
# <a name="loading-and-registering-a-type-library"></a>Загрузка и регистрация библиотеки типов

Библиотека динамической компоновки службы автоматизации, Oleaut32.dll, предоставляет несколько функций, которые можно вызывать для загрузки и регистрации библиотеки типов. Вызов [лоадтипелибекс](/windows/win32/api/oleauto/nf-oleauto-loadtypelibex), как показано в следующем примере, обе загружают библиотеку и создает записи реестра.

## <a name="example"></a>Пример

``` syntax
ITypeLib *pTypeLib;
HRESULT hr;
hr = LoadTypeLibEx("example.tlb", REGKIND_REGISTER, &pTypeLib);
if(SUCCEEDED(hr))
{
    pTypeLib->Release();
} else {
    exit(0); // Handle errors here.
}
```

 

 