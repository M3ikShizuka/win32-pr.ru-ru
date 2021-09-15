---
title: StringCollection. getItemInfo, метод
description: Метод getItemInfo извлекает строку, соответствующую указанному индексу и имени элемента StringCollection.
ms.assetid: a031b91e-9d3b-47ac-bc5b-c111d5e3bc12
keywords:
- проигрыватель Windows Media метода getItemInfo
- проигрыватель Windows Media метода getItemInfo, класс StringCollection
- класс StringCollection проигрыватель Windows Media, метод getItemInfo
topic_type:
- apiref
api_name:
- StringCollection.getItemInfo
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1c9552dcebbc7d565ebc797c62ac3bc00ee109fb
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570086"
---
# <a name="stringcollectiongetiteminfo-method"></a>StringCollection. getItemInfo, метод

Метод **getItemInfo** извлекает строку, соответствующую указанному индексу и имени элемента **StringCollection** .

## <a name="syntax"></a>Синтаксис


```JScript
strRetVal = StringCollection.getItemInfo(
  index,
  name
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*индекс* \[ окне\]
</dt> <dd>

**Число** (**Long**), указывающее Отсчитываемый от нуля индекс элемента **StringCollection** , из которого необходимо получить атрибут.

</dd> <dt>

*имя* \[ окне\]
</dt> <dd>

**Строка** , содержащая имя атрибута.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает **строку** , представляющую значение указанного атрибута. Для атрибутов, базовое значение которых является **логическим**, оно возвращает строку "true" или "false".

## <a name="remarks"></a>Remarks

Чтобы получить атрибуты с несколькими значениями и атрибутами со сложными значениями, используйте метод **жетитеминфобитипе** .

Чтобы использовать этот метод, требуется доступ на чтение к библиотеке. Дополнительные сведения см. в разделе [доступ к библиотеке](library-access.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 11.<br/>                                                |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**StringCollection. Жетитеминфобитипе**](stringcollection-getiteminfobytype.md)
</dt> <dt>

[**Объект StringCollection**](stringcollection-object.md)
</dt> </dl>

 

 





