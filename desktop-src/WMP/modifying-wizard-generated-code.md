---
title: Изменение кода, созданного мастером
description: Изменение кода, созданного мастером
ms.assetid: 391a7773-c3e2-499a-bb63-e5934537d963
keywords:
- проигрыватель Windows Media Мобильные устройства, подключаемые модули
- проигрыватель Windows Media Мобильные устройства, подключаемые модули пользовательского интерфейса
- проигрыватель Windows Media Подключаемые модули для мобильных устройств
- подключаемые модули, Пользовательский интерфейс
- подключаемые модули, проигрыватель Windows Media мобильные устройства
- подключаемые модули пользовательского интерфейса проигрыватель Windows Media мобильные устройства
- подключаемые модули пользовательского интерфейса, проигрыватель Windows Media мобильные устройства
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: a83bda7cb265d0c2e039ada6d9d827c6da3faf63
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127342818"
---
# <a name="modifying-wizard-generated-code"></a>Изменение кода, созданного мастером

в коде подключаемого модуля, созданном мастером, есть несколько мест, которые необходимо изменить, прежде чем подключаемый модуль будет работать с проигрыватель Windows Media 10 Mobile. Код, который необходимо изменить, выделяется полужирным шрифтом в следующих примерах.

## <a name="changes-to-wmpplugh"></a>Изменения в вмпплуг. h

методы ansi не поддерживаются на устройствах под управлением Windows CE, поэтому необходимо изменить следующий метод ANSI, созданный мастером в вмпплуг. h:


```C++
return( ::PostMessage( HWND_BROADCAST, ::RegisterWindowMessageA( "WMPlayer_PluginAddRemove" ), 0, 0 ) );
```



Измените его, как показано ниже, чтобы он стал методом Юникода:


```C++
return( ::PostMessage( HWND_BROADCAST, ::RegisterWindowMessageW( L"WMPlayer_PluginAddRemove" ), 0, 0 ) );
```



## <a name="changes-to-networkpluginh"></a>Изменения в Нетворкплугин. h

Найдите следующий код в Нетворкплугин. h:


```C++
BEGIN_COM_MAP(CNetworkPlugin)
    COM_INTERFACE(IWMPPluginUI)
END_COM_MAP()
```



Измените код так, чтобы он выглядел следующим образом:


```C++
BEGIN_COM_MAP(CNetworkPlugin)
    
COM_INTERFACE_ENTRY_IID(__uuidof(IWMPPluginUI), IWMPPluginUI)
END_COM_MAP()
```



## <a name="changes-to-networkplugindllcpp"></a>Изменения в Нетворкплугиндлл. cpp

Найдите функцию **DllMain** в нетворкплугиндлл. cpp:


```C++
extern "C" BOOL WINAPI DllMain(HINSTANCE hInstance, DWORD dwReason, LPVOID /*lpReserved*/)
{
    if (dwReason == DLL_PROCESS_ATTACH)
    {
        _Module.Init(ObjectMap, hInstance);
        DisableThreadLibraryCalls(hInstance);
    }
    else if (dwReason == DLL_PROCESS_DETACH)
        _Module.Term();
    return TRUE;    // ok
}
```



Измените код так, чтобы он выглядел следующим образом:


```C++
extern "C" BOOL WINAPI DllMain(HANDLE hInstance, DWORD dwReason, LPVOID /*lpReserved*/)
{
    if (dwReason == DLL_PROCESS_ATTACH)
    {
        _Module.Init(ObjectMap, (HINSTANCE)hInstance);
#ifndef UNDER_CE
        DisableThreadLibraryCalls((HINSTANCE)hInstance);
#endif
    }
    else if (dwReason == DLL_PROCESS_DETACH)
        _Module.Term();
    return TRUE;    // ok
}
```



## <a name="changes-to-networkplugincpp"></a>Изменения в Нетворкплугин. cpp

Найдите следующий код в Нетворкплугин. cpp:


```C++
hr = m_spCore->QueryInterface(&spConnectionContainer);
```



Измените код так, чтобы он выглядел следующим образом:


```C++
hr = m_spCore->QueryInterface(__uuidof(IConnectionPointContainer), (void**)&spConnectionContainer);
```



## <a name="change-the-threading-model"></a>Изменение потоковой модели

в отличие от atl для Windows, ATL для Windows CE не поддерживает модель потоков подразделений, так как модель подразделения требует больше ресурсов памяти, чем модели с одним потоком и свободными потоками. Поэтому необходимо найти все экземпляры потоков подразделений в файле StdAfx. h и Нетворкплугин. RGS и изменить их, чтобы они указывали на свободную потоковое взаимодействие.

кроме того, можно вызвать только мобильный элемент управления проигрыватель Windows Media 10 из потока, в котором он был создан.

## <a name="build-and-test-the-project"></a>Сборка и тестирование Project

После внесения этих изменений можно построить проект, чтобы убедиться, что он компилируется перед добавлением пользовательского кода.

1.  Задайте для параметра Активная конфигурация проекта значение Win32 (ВЦЕ ARMV4) Debug или Win32 (ВЦЕ ARMV4).
2.  задайте для активной платформы значение карманный ПК 2003.
3.  Щелкните элемент меню **Сборка** , а затем выберите **Сборка NetworkPlugin.dll**. Она должна компилироваться, скачиваться и регистрироваться на устройстве.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**создание подключаемого модуля пользовательского интерфейса для проигрыватель Windows Media 10 Mobile**](creating-a-user-interface-plug-in-for-windows-media-player-10-mobile.md)
</dt> </dl>

 

 




