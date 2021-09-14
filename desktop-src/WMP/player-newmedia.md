---
title: Метод Player. Невмедиа
description: Метод Невмедиа создает новый объект мультимедиа.
ms.assetid: fccf1559-bac3-4edf-bd88-da2c72cdec21
keywords:
- проигрыватель Windows Media метода невмедиа
- метод невмедиа проигрыватель Windows Media, класс Player
- класс Player проигрыватель Windows Media, метод невмедиа
topic_type:
- apiref
api_name:
- Player.newMedia
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: aaafb97f836135aa9dd112372b1931c8561cb40b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127342802"
---
# <a name="playernewmedia-method"></a>Метод Player. Невмедиа

Метод **невмедиа** создает новый объект **мультимедиа** .

## <a name="syntax"></a>Синтаксис


```JScript
retVal = Player.newMedia(
  URL
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*URL-адрес* \[ окне\]
</dt> <dd>

**Строка** , содержащая URL-адрес файла цифрового мультимедиа, с которым создается объект **мультимедиа** .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает объект **мультимедиа** .

## <a name="remarks"></a>Remarks

Параметр *URL-адреса* не должен быть пустой строкой или иметь значение null.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии.<br/>                                 |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект Player**](player-object.md)
</dt> </dl>

 

 





