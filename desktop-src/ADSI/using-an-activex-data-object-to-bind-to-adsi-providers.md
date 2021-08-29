---
title: использование объекта данных ActiveX для привязки к поставщикам ADSI
description: так как ADSI также является поставщиком OLE DB, для подключения к поставщикам ADSI можно использовать объект данных ActiveX (ADO).
ms.assetid: b42d804b-f1eb-4085-88aa-015a92309ee8
ms.tgt_platform: multiple
keywords:
- ActiveX ADSI для объектов данных
- ActiveX объектов data ADSI с помощью ADO для привязки к поставщикам ADSI
- поставщики услуг ADSI, использование ActiveX объекта данных для привязки
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 4f9c34e026fabe34e52bcfbd9182cca935cf7e019b1fd1c3c8f97fd2f88be48c
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119637534"
---
# <a name="using-an-activex-data-object-to-bind-to-adsi-providers"></a>использование объекта данных ActiveX для привязки к поставщикам ADSI

так как ADSI также является поставщиком OLE DB, для подключения к поставщикам ADSI можно использовать объект данных ActiveX (ADO). Как и в случае с другими поставщиками ADO, для подключения к поставщику OLE DB необходимо создать новый объект соединения и, при необходимости, указать учетные данные. Имя поставщика OLE DB ADSI — **адсдсубжект**.

Например:


```VB
Dim con As New Connection 
'VBScript use: con = CreateObject("ADODB.Connection")
con.Provider = "ADsDSOObject"
con.Open "YourDescriptionHere"
```



В предыдущем примере вы подключены от имени текущего пользователя. Чтобы указать другие учетные данные, используйте свойства соединения:


```VB
con.Provider = "ADsDSOObject"
con.Properties("User ID") = "jeffsmith"
con.Properties("Password") = "guesswhat?"
con.Properties("Encrypt Password") = True
con.Open "YourDescriptionHere"
```



ADSI OLE DB определяет следующие свойства соединения.



| Свойство           | Тип данных   | По умолчанию   |
|--------------------|-------------|-----------|
| "Идентификатор пользователя"          | **ОСВОБОЖДАЕМОЙ**    | **NULL**  |
| "Пароль".         | **ОСВОБОЖДАЕМОЙ**    | **NULL**  |
| "Зашифровать пароль" | **ЛОГИЧЕСКАЯ** | **FALSE** |
| "Флаг ADSI"        | **Long**    | 0         |



 

С помощью OLE DB ADO невозможно выполнить привязку к определенному объекту. Однако можно запросить конкретный объект и возвратить результирующий набор. Только поставщики ADSI, которые поддерживают [**IDirectorySearch**](/windows/desktop/api/Iads/nn-iads-idirectorysearch) , имеют преимущества от использования ADO в качестве модели программирования.

Свойство флага ADSI используется для указания параметра проверки подлинности привязки. Это свойство может быть сочетанием флагов из перечисления [**объявлений \_ проверки \_ подлинности**](/windows/win32/api/iads/ne-iads-ads_authentication_enum) .

 

 




