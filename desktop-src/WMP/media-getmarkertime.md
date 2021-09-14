---
title: Метод Media. Жетмаркертиме
description: Метод Жетмаркертиме извлекает время маркера по указанному индексу.
ms.assetid: c3e6bead-2831-4d84-9d13-dcb865efe472
keywords:
- проигрыватель Windows Media метода жетмаркертиме
- проигрыватель Windows Media метода жетмаркертиме, класс мультимедиа
- класс мультимедиа проигрыватель Windows Media, метод жетмаркертиме
topic_type:
- apiref
api_name:
- Media.getMarkerTime
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4398f89055a1996acb3f921d33c7675e52100ddd
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056368"
---
# <a name="mediagetmarkertime-method"></a>Метод Media. Жетмаркертиме

Метод **жетмаркертиме** извлекает время маркера по указанному индексу.

## <a name="syntax"></a>Синтаксис


```JScript
retVal = Media.getMarkerTime(
  markerNum
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*маркернум* \[ окне\]
</dt> <dd>

**Число** (**длинное**), указывающее индекс маркера.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает **число** (**Double**), задающее положение маркера в секундах от начала клипа.

## <a name="remarks"></a>Комментарии

Этот метод возвращает **значение NULL** , если указанный маркер не существует.

Некоторые цифровые мультимедийные элементы не содержат маркеров. Используйте **маркеркаунт** , чтобы узнать, сколько маркеров находится в текущем клипе.

Номера индексов маркеров начинаются с 1.

Чтобы использовать этот метод, требуется доступ на чтение к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

## <a name="examples"></a>Примеры

в следующем примере JScript используется *носитель*. **жетмаркертиме** для заполнения HTML-элемента textarea с именем мтимес расположением каждого маркера. Объект **Player** создан с идентификатором "Player".


```JScript
// Get the number of markers in the current media item.
var mcount = Player.currentMedia.markerCount;

// Verify that at least one marker exists in the current media item.
if (mcount > 0){

// Loop through the marker list.
for (var i = 1;i < mcount + 1; i++){

   // Print the message to the text area.
   MTIMES.value += "Marker number " + i + " occurs at ";
   MTIMES.value += Player.currentMedia.getMarkerTime(i);
   MTIMES.value += " second(s).";
   MTIMES.value += "\n";
}

```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**Объект мультимедиа**](media-object.md)
</dt> <dt>

[**Media. Жетмаркернаме**](media-getmarkername.md)
</dt> <dt>

[**Media. Маркеркаунт**](media-markercount.md)
</dt> <dt>

[**Параметры. медиаакцессригхтс**](settings-mediaaccessrights.md)
</dt> <dt>

[**Параметры. рекуестмедиаакцессригхтс**](settings-requestmediaaccessrights.md)
</dt> </dl>

 

 





