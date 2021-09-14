---
title: Network. Буфферингкаунт
description: Свойство Буфферингкаунт извлекает количество попыток буферизации во время воспроизведения клипа.
ms.assetid: 25a58795-161e-4290-8ea7-51acca968ef9
keywords:
- проигрыватель Windows Media Network. буфферингкаунт
topic_type:
- apiref
api_name:
- Network.bufferingCount
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 524dc66c7f4ed1d413f264a91ae9385d458d632b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967425"
---
# <a name="networkbufferingcount"></a>Network. Буфферингкаунт

Свойство **буфферингкаунт** извлекает количество попыток буферизации во время воспроизведения клипа.

## <a name="syntax"></a>Синтаксис

*проигрыватель*. *сеть*. **буфферингкаунт**

## <a name="possible-values"></a>Возможные значения

Это свойство является **числом** только для чтения (**длинное целое**).

## <a name="remarks"></a>Комментарии

Каждый раз, когда воспроизведение останавливается и перезапускается, это свойство устанавливается в нулевое значение. Если воспроизведение приостановлено, оно не сбрасывается.

Буферизация применяется только к потоковой передаче содержимого. Это свойство возвращает действительные сведения только во время выполнения, когда *проигрыватель*. Задано свойство **URL-адреса** .

## <a name="examples"></a>Примеры

в следующем примере JScript используется *сеть*. **буфферингкаунт** для вывода количества попыток буферизации во время воспроизведения. Сведения отображаются в HTML-элементе DIV, созданном с помощью ID = "CB". Объект **Player** создан с идентификатором "Player".


```JScript
<!-- Create an event handler. -->
<SCRIPT FOR = Player EVENT = buffering(Start)>
   if (true == Start) 
      CB.innerHTML = "Buffering count: " + Player.network.bufferingCount;
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

[**Player. URL**](player-url.md)
</dt> </dl>

 

 





