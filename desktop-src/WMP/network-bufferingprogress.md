---
title: Network. Буфферингпрогресс
description: Свойство Буфферингпрогресс извлекает процент завершенной буферизации.
ms.assetid: d604159b-7c42-47f8-8085-53f859f24703
keywords:
- проигрыватель Windows Media Network. буфферингпрогресс
topic_type:
- apiref
api_name:
- Network.bufferingProgress
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e9e3a4f37f8f6b8ffe8ff93ca72b0c9551d7e314
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462526"
---
# <a name="networkbufferingprogress"></a>Network. Буфферингпрогресс

Свойство **буфферингпрогресс** извлекает процент завершенной буферизации.

## <a name="syntax"></a>Синтаксис

*проигрыватель*. *сеть*. **буфферингпрогресс**

## <a name="possible-values"></a>Возможные значения

Это свойство является **числом** только для чтения (**длинное целое**).

## <a name="remarks"></a>Remarks

Каждый раз, когда воспроизведение останавливается и перезапускается, это свойство устанавливается в нулевое значение. Если воспроизведение приостановлено, оно не сбрасывается.

Буферизация применяется только к потоковой передаче содержимого. Это свойство возвращает действительные сведения только во время выполнения, когда *игрок*. Задано свойство **URL-адреса** .

Чтобы определить время запуска или остановки буферизации, используйте событие *Player*. * * * * буферизация * * * *.

## <a name="examples"></a>Примеры

в следующем примере JScript используется *сеть*. **буфферингпрогресс** для вывода процента завершения буферизации. Сведения отображаются в HTML-элементе DIV, созданном с помощью ID = BP. В примере для обновления экрана используется таймер с интервалом в 1 секунду. Объект **Player** создан с идентификатором "Player".


```JScript
<!-- Create an event handler for buffering. -->
<SCRIPT FOR = Player EVENT = buffering(Start)>
   var idI; // Variable for the interval id.

   // Test whether buffering has started or stopped.
   if (true == Start){ 
      // Start the timer. Call the function to update the display every second.
      idI = window.setInterval("UpdateBP()", 1000);
   }

   else{
      // Buffering is complete. Stop the timer.
      window.clearInterval(idI);
   }
</SCRIPT>

<!-- Put the function to update the display in a separate code block. -->
<SCRIPT>
function UpdateBP(){
   BP.innerHTML = "";
   BP.innerHTML = "Buffering progress: " + Player.network.bufferingProgress;
   BP.innerHTML += " percent complete";
}
</SCRIPT>

```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Сетевой объект**](network-object.md)
</dt> <dt>

[**Событие проигрывателя. буферизация**](player-player-buffering.md)
</dt> <dt>

[**Player. URL**](player-url.md)
</dt> </dl>

 

 





