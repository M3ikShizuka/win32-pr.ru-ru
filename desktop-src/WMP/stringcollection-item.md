---
title: StringCollection. Item, метод
description: Метод Item извлекает строку по указанному индексу.
ms.assetid: 5f6afff2-3ecc-4b28-8c67-f859f5440d4f
keywords:
- проигрыватель Windows Media метода элемента
- метод item проигрыватель Windows Media, класс StringCollection
- класс StringCollection проигрыватель Windows Media, метод item
topic_type:
- apiref
api_name:
- StringCollection.item
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c4244ad194ff3426dab81baddc0b7188214e0360
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570079"
---
# <a name="stringcollectionitem-method"></a>StringCollection. Item, метод

Метод **Item** извлекает строку по указанному индексу.

## <a name="syntax"></a>Синтаксис


```JScript
strRetVal = StringCollection.item(
  index
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*индекс* \[ окне\]
</dt> <dd>

**Число** (**Long**), содержащее индекс.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает **строку**.

## <a name="remarks"></a>Remarks

Объект **StringCollection** используется для получения набора значений, доступных для атрибута. Например, *медиаколлектион*. метод **жетаттрибутестрингколлектион** можно использовать для получения объекта **StringCollection** , представляющего все значения атрибута жанра в типе мультимедиа. Затем свойство **Item** можно использовать для итерации всех возможных значений атрибута жанра.

Чтобы использовать этот метод, требуется доступ на чтение к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Медиаколлектион. Жетаттрибутестрингколлектион**](mediacollection-getattributestringcollection.md)
</dt> <dt>

[**Параметры. медиаакцессригхтс**](settings-mediaaccessrights.md)
</dt> <dt>

[**Параметры. рекуестмедиаакцессригхтс**](settings-requestmediaaccessrights.md)
</dt> <dt>

[**Объект StringCollection**](stringcollection-object.md)
</dt> </dl>

 

 





