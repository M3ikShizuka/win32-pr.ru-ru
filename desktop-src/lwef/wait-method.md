---
title: Метод Wait
description: Метод Wait
ms.assetid: 968a3f19-6953-473b-ba98-0dc93696e703
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d81949957146756e989fcb577a1bdd5a0c9a2a6fd60932220e39950327ba3061
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119715714"
---
# <a name="wait-method"></a>Метод Wait

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

<dl> <dt>

<span id="Description"></span><span id="description"></span><span id="DESCRIPTION"></span>**Nописание**
</dt> <dd>

Заставляет очередь анимации для указанного символа ожидать завершения заданного запроса анимации.

</dd> <dt>

<span id="Syntax"></span><span id="syntax"></span><span id="SYNTAX"></span>**Syntax**
</dt> <dd>

*Агент ***. Символы ("**_чарактерид_*_"). Запрос на ожидание_ * 



| Часть      | Описание                                                                     |
|-----------|---------------------------------------------------------------------------------|
| *Запрос* | Объект [**запроса**](/windows/desktop/lwef/the-request-object) , указывающий определенную анимацию.. |



 

</dd> </dl>

## <a name="remarks"></a>Remarks

Этот метод следует использовать только в том случае, если поддерживается несколько (одновременных) символов и выполняется попытка последовательного взаимодействия символов. (Для одного символа каждый запрос анимации воспроизводится последовательно — по завершении предыдущего запроса.) Если у вас есть два символа и требуется, чтобы запрос анимации символа ожидал завершения анимации другого символа, задайте метод **ожидания** для объекта [**запроса**](/windows/desktop/lwef/the-request-object) анимации другого символа. Чтобы указать параметр запроса, необходимо создать переменную и назначить запрос анимации, который нужно прервать:


```
   Dim GenieRequest 
   Dim RobbyRequest 
   Dim Genie 
   Dim Robby 

   Sub window_Onload

   Agent1.Characters.Load "Genie", "https://agent.microsoft.com/characters/v2/genie/genie.acf"
   Agent1.Characters.Load "Robby", "https://agent.microsoft.com/characters/v2/robby/robby.acf"

   Set Genie = Agent1.Characters("Genie")
   Set Robby = Agent1.Characters("Robby")

   Genie.Get "State", "Showing"
   Robby.Get "State", "Showing"

   Genie.Get "Animation", "Announce, AnnounceReturn, Pleased, _ 
      PleasedReturn"
   
   Robby.Get "Animation", "Confused, ConfusedReturn, Sad, SadReturn"

   Set Genie = Agent1.Characters ("Genie")
   Set Robby = Agent1.Characters ("Robby")

   Genie.MoveTo 100,100
   Genie.Show

   Robby.MoveTo 250,100
   Robby.Show

   Genie.Play "Announce"
   Set GenieRequest = Genie.Speak ("Why did the chicken cross the road?")
   
   Robby.Wait GenieRequest
   Robby.Play "Confused"
   Set RobbyRequest = Robby.Speak ("I don't know. Why did the chicken _
      cross the road?")
   
   Genie.Wait RobbyRequest
   Genie.Play "Pleased"
   Set GenieRequest = Genie.Speak ("To get to the other side.")
   
   Robby.Wait GenieRequest
   Robby.Play "Sad"
   Robby.Speak "I never should have asked."

   End Sub
```



Можно также упростить код, просто вызвав **Wait** напрямую, используя конкретный запрос анимации.


```
   Robby.Wait Genie.Play "GestureRight"
```



Это позволяет избежать явного объявления объекта [**запроса**](/windows/desktop/lwef/the-request-object) .

 

 