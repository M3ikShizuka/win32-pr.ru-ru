---
title: Network. Саурцепротокол
description: Свойство Саурцепротокол получает исходный протокол, используемый для получения данных.
ms.assetid: f09bbcd0-9c34-49d1-8080-247aed2548d5
keywords:
- проигрыватель Windows Media Network. саурцепротокол
topic_type:
- apiref
api_name:
- Network.sourceProtocol
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 29e3f0ad63827605eb79a89325877e4bb83bfc62
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967417"
---
# <a name="networksourceprotocol"></a>Network. Саурцепротокол

Свойство **саурцепротокол** получает исходный протокол, используемый для получения данных.

## <a name="syntax"></a>Синтаксис

*проигрыватель*. *сеть*. **саурцепротокол**

## <a name="possible-values"></a>Возможные значения

Это свойство является **строкой**, доступная только для чтения.

## <a name="remarks"></a>Комментарии

Это свойство имеет значение "" (пустая строка) при воспроизведении мультимедиа с компакт-диска или DVD-диска.

## <a name="examples"></a>Примеры

в следующем примере JScript используется *сеть*. **саурцепротокол** для вывода исходного протокола, используемого для получения данных. Сведения отображаются в HTML-элементе DIV, созданном с помощью ID = "SP". Объект **Player** создан с идентификатором "Player".


```JScript
<!-- Create an event handler for play state change. -->
<SCRIPT FOR = Player EVENT = PlayStateChange(NewState)>
   if (3 == NewState){
     SP.innerHTML = "Source protocol: " + Player.network.sourceProtocol;
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
</dt> </dl>

 

 





