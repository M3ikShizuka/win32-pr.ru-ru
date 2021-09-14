---
title: Использование системного монитора
description: системный монитор (сисмон) можно включать в любое приложение, которое поддерживает ActiveX \ 174; элементы управления. например, можно включить сисмон в приложение Microsoft Visual Basic или в HTML-документ.
ms.assetid: 36931aae-b608-42d9-a3e3-09784e80f386
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: abd636c8b984f7c891c2222b4674dd8d0d7e747d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127243832"
---
# <a name="using-system-monitor"></a>Использование системного монитора

системный монитор (сисмон) можно включать в любое приложение, которое поддерживает ActiveX® элементов управления. например, можно включить сисмон в приложение Microsoft Visual Basic или в HTML-документ.

В следующем примере показано, как включить СИСМОН в HTML-документ. В примере используется сценарий VBScript для добавления счетчиков, значения которых извлекаются с локального компьютера, изменения некоторых свойств СИСМОН, управляющих отображением монитора, и обработки события Онкаунтерадд. В примере используется символ-шаблон ( \* ) для добавления всех экземпляров счетчика процесса.

``` syntax
<HTML>
<BODY BGCOLOR=#C0C0C0>

<SCRIPT LANGUAGE="VBScript">
  Sub Monitor_OnCounterAdded(index)
    Monitor.Counters.Item(1).Width = 8
  End Sub
</Script>
<OBJECT
  CLASSID="clsid:C4D2D8E0-D1DD-11CE-940F-008029004347"
  ID="Monitor"
  HEIGHT=80%
  WIDTH=100%>
</OBJECT>

<SCRIPT LANGUAGE="VBScript">
  Sub Window_OnLoad
    On Error Resume Next
    Monitor.ShowValueBar = False
    Monitor.ShowHorizontalGrid = True
    Monitor.Counters.Add("\Process(*)\% Processor Time")
    Monitor.DisplayType=sysmonLineGraph
    Monitor.GraphTitle="System Performance Overview"
  End Sub
</SCRIPT>

</BODY>
</HTML>
```

 

 




