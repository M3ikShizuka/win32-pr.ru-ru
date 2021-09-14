---
description: Объект параметров содержит список параметров для вызова методов поставщика при использовании типа вызова ExecMethod.
ms.assetid: 8cc65129-1698-4ada-b493-672772c94045
ms.tgt_platform: multiple
title: Построение объектов с параметрами
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: fbf9a351caec1ca7af3113bead4078670c88a5f3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458148"
---
# <a name="constructing-inparameters-objects"></a>Построение объектов с параметрами

Объект [**параметров**](swbemmethod-inparameters.md) содержит список параметров для вызова методов поставщика при использовании типа вызова **ExecMethod** . Для всех методов [**SWbemObject \_ . ExecMethod**](swbemobject-execmethod-.md), [**SWbemObject \_ . ексекмесодасинк**](swbemobject-execmethodasync-.md), [**SwbemServices. ExecMethod**](swbemservices-execmethod.md)и [**SwbemServices. ексекмесодасинк**](swbemservices-execmethodasync.md) требуется объект с **параметрами** .

Следующая процедура описывает, как создать объект с [**параметрами**](swbemmethod-inparameters.md) .

**Создание параметра *обжвбеминпарамс***

1.  Подключение WMI.
2.  Получите определение класса WMI, определяющего метод, который необходимо выполнить.
3.  Получите объект с [**параметрами**](swbemmethod-inparameters.md) , относящийся к методу класса WMI, который необходимо выполнить.

    ```VB
    Set objInParam = objShare.Methods_("Create"). _
        inParameters.SpawnInstance_()
    ```

    

4.  Задайте для свойств экземпляра значение, соответствующее значениям. Обязательно присвойте значения ключевым свойствам в классе WMI, содержащем метод, который необходимо выполнить.

    Например, если вы хотите задать входной параметр с именем минпутпарам в качестве значения "ABC" в экземпляре [**параметров**](swbemmethod-inparameters.md) , именуемых "inst", код будет выглядеть следующим образом.

    ```VB
    INST.Properties_.Add ("myinputparam").Value = "abc".
    ```

    

5.  Выполните метод и получите возвращаемое состояние выполняемого метода.

В следующем примере кода показана настройка объекта [**параметров**](swbemmethod-inparameters.md) для создания нового объекта WMI, представляющего общую папку. Дополнительные сведения об объекте [**Parameters**](swbemmethod-outparameters.md) см. в разделе [анализ объектов параметров](parsing-outparameters-objects.md). Этот пример возвращает успешно возвращенное значение (0), если имеется папка с именем "Share" в расположении "C:/Share". Этот пример позволяет предоставлять общий доступ к этой папке другим пользователям.


```VB
' Connect to WMI.
Set objServices = GetObject("winmgmts:root\cimv2")

' Obtain the definition of the WMI class that defines
' the method you want to execute.
Set objShare = objServices.Get("Win32_Share")

' Obtain an InParameters object specific
' to the WMI class method you want to execute.
Set objInParam = objShare.Methods_("Create"). _
    inParameters.SpawnInstance_()

' Set the properties of the instance to whatever
' values are appropriate.
objInParam.Properties_.Item("Access") = objSecDescriptor
objInParam.Properties_.Item("Description") = _
    "New share created by WMI script"
objInParam.Properties_.Item("Name") = "share"
objInParam.Properties_.Item("Path") = "C:\share"
objInParam.Properties_.Item("Type") = 0
'optional - default is 'max allowed'
objInParam.Properties_.Item("MaximumAllowed") = 100
'optional - default is no password
objInParam.Properties_.Item("Password") = "Password"

' Execute the method and obtain the return status. 
' The OutParameters object in objOutParams
' is created by the provider. 
Set objOutParams = objShare.ExecMethod_("Create", objInParam)    
wscript.echo objOutParams.ReturnValue
```



 

 



