---
title: метод завершения (устаревшие функции Windows среды)
description: Метод Stop
ms.assetid: 68372f72-db9c-447c-a3e4-488940c730d7
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 20192634c197559ca54bb8af3d8a29f37beb53e2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127459467"
---
# <a name="stop-method-legacy-windows-environment-features"></a>метод завершения (устаревшие функции Windows среды)

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

<dl> <dt>

<span id="Description"></span><span id="description"></span><span id="DESCRIPTION"></span>**Nописание**
</dt> <dd>

Останавливает анимацию для указанного символа.

</dd> <dt>

<span id="Syntax"></span><span id="syntax"></span><span id="SYNTAX"></span>**Syntax**
</dt> <dd>

*Агент ***. Символы ("**_чарактерид_*_")._ *  \[ *Запрос* на завершение\]



| Часть      | Описание                                                                                   |
|-----------|-----------------------------------------------------------------------------------------------|
| *Запрос* | Необязательный параметр. Объект [**запроса**](/windows/desktop/lwef/the-request-object) , указывающий конкретный вызов анимации. |



 

</dd> </dl>

## <a name="remarks"></a>Комментарии

Чтобы указать параметр запроса, необходимо создать переменную и назначить запрос анимации, который нужно присвоить. Если параметр **запроса** не задан, сервер останавливает все анимации для символа, включая вызовы [**Get**](get-method.md) , помещенные в очередь, и очищает ее очередь анимации, если этот символ в данный момент не содержит **скрытую** анимацию или не **отображает** ее. Этот метод не останавливает вызовы **Get** , не входящие в очередь.

Чтобы отменить определенную анимацию или вызов [**Get**](get-method.md) , объявите объектную переменную и назначьте запрос анимации этой переменной:


```
   Dim MyRequest
   Dim Genie

   Agent1.Characters.Load "Genie", "https://agent.microsoft.com/characters/v2/genie/genie.acf"

   Set Genie = Agent1.Characters ("Genie")

   Genie.Get "state", "Showing"
   Genie.Get "animation", "Greet, GreetReturn"

   Genie.Show
   
   'This animation will never play
   Set MyRequest = Genie.Play ("Greet")
   
   Genie.Stop MyRequest
```



Этот метод не создаст объект [**запроса**](/windows/desktop/lwef/the-request-object) .

## <a name="see-also"></a>См. также:

[**Метод Стопалл**](stopall-method.md)


 

 
