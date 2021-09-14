---
title: THEME. closeView
description: Метод closeView закрывает открытое представление.
ms.assetid: 37b56a7d-8031-4055-95ad-0510105e1c1f
keywords:
- проигрыватель Windows Media THEME. closeView
topic_type:
- apiref
api_name:
- THEME.closeView
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: b39083979809fc2e747c54569db8d03298a951c6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066660"
---
# <a name="themecloseview"></a>THEME. closeView

Метод **closeView** закрывает открытое **представление**.

``` syntax
        theme.closeView(theView)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="theView"></span><span id="theview"></span><span id="THEVIEW"></span>*севиев*
</dt> <dd>

**Строка** , указывающая **идентификатор** закрытого **представления** .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="examples"></a>Примеры


```C++
<THEME>
  <VIEW>
    <TEXT value="open" 
        onclick="jscript:theme.openView('newView')"/>
    <TEXT top="30" value="close"
        onclick="jscript:theme.closeView('newView')"/>
  </VIEW>
  <VIEW id="newView"/>
</THEME>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Элемент THEME**](theme-element.md)
</dt> <dt>

[**THEME. openView**](theme-openview.md)
</dt> </dl>

 

 





