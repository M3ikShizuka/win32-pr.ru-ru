---
title: начало работы с ASP для ADSI
description: Интерфейсы ADSI можно использовать для доступа к данным каталога с помощью страницы ASP. Это может быть удобным способом выполнения задач администрирования и запросов с веб-страницы или предоставления сведений сотрудникам в интрасети.
ms.assetid: 2007257c-6c4e-415e-9ab5-e65d8d9e5dd4
ms.tgt_platform: multiple
keywords:
- ASP ADSI
- ADSI, страницы ASP
- ADSI, страницы ASP, пример кода ASP
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: f17c5d32fea196d77b8fb54463231e1bc1bc165c6bd48e49dffb351a9d6d45dd
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119082568"
---
# <a name="getting-started-with-asp-for-adsi"></a>начало работы с ASP для ADSI

Интерфейсы ADSI можно использовать для доступа к данным каталога с помощью страницы ASP. Это может быть удобным способом выполнения задач администрирования и запросов с веб-страницы или предоставления сведений сотрудникам в интрасети.

одним из преимуществ использования ADSI с ASP является то, что вы можете создавать более широкие возможности для пользователей, поскольку вы можете использовать Visual Basic, чтобы создать приложение ADSI и предложить его пользователю через стандартную веб-страницу. Например, можно создать веб-страницу, которая позволяет сотрудникам ввести фамилию сотрудника и возвратить номер телефона для этого сотрудника, или создать форму, позволяющую сотрудникам обновлять персональные данные в базе данных отдела кадров компании.

Код ASP начинается с "<%" и заканчивается на "% >". Можно добавить код ADSI в качестве VBScript или Visual Basic.

чтобы создать страницу ASP, можно использовать редактор веб-страниц, Блокнот или другой текстовый редактор или Microsoft Visual Studio систему разработки .net.

Перед запуском страницы ASP настройте приложение или сервер IIS в соответствии с инструкциями в статье [проблемы проверки подлинности для ADSI с ASP](authentication-issues-for-adsi-with-asp.md).

## <a name="a-simple-asp-sample-enumerating-objects-in-a-container"></a>Простой пример ASP: перечисление объектов в контейнере

С помощью редактора веб-страниц создайте новую HTML-страницу, которая принимает различающееся имя объекта контейнера. Введите следующий пример кода.


```HTML
<html>
<body>

<form method="POST" action="https://localhost/Enum.asp" ID="Form1">
<p>Distinguished name of container:<input type="text" name="inpContainer" size="100" ID="Text2"></p>
<p><input type="SUBMIT" value="GO" ID="Submit1" NAME="Submit1"></p>
</form>

</body>
</html>
```



Теперь эта страница может принять имя контейнера, которое ему передается, и использовать ADSI для перечисления объектов в контейнере.

Создайте новую ASP-страницу с именем Enum. ASP и введите следующий пример кода. Сохраните эту страницу в корне локального веб-сервера.


```VB
<%@ Language=VBScript %>
<%
' Get the inputs.
containerName = Request.Form("inpContainer")
' Validate compName before using.

If Not ("" = containerName) Then
  ' Bind to the object.
  adsPath = "LDAP://" & containerName
  Set comp = GetObject(adsPath)

  ' Write the ADsPath of each of the child objects.
  Response.Write("<p>Enumeration:</p>")
  For Each obj in comp
    Response.Write(obj.ADsPath + "<BR>")
  Next
End If
%>
```



 

 




