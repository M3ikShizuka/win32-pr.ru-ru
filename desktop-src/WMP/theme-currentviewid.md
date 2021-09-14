---
title: THEME. Куррентвиевид
description: Атрибут Куррентвиевид указывает или получает отображаемое в данный момент представление.
ms.assetid: 94f23da9-cfda-4dc4-9804-b7daff5ebb8f
keywords:
- проигрыватель Windows Media THEME. куррентвиевид
topic_type:
- apiref
api_name:
- THEME.currentViewID
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1c0c1b52ffdc35abf846987ed459565904938d4e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127066658"
---
# <a name="themecurrentviewid"></a>THEME. Куррентвиевид

Атрибут **куррентвиевид** указывает или получает отображаемое в данный момент **представление**.

``` syntax
theme.currentViewID
```

## <a name="possible-values"></a>Возможные значения

Этот атрибут является **строкой** для чтения и записи, указывающей **идентификатор** текущего **представления**. У него нет значения по умолчанию.

## <a name="remarks"></a>Remarks

При указании **куррентвиевид** автоматически закрывается существующий **куррентвиев** (на который указывает глобальный атрибут **представления** ) и открывается указанное **представление**.

## <a name="examples"></a>Примеры


```C++
<THEME currentViewID="startView">
  <VIEW>
    <TEXT value="this would have been the default view"/>
  </VIEW>
  <VIEW id="startView">
    <TEXT value="go to new view"
        onclick="jscript:theme.currentViewID='newView'"/>
  </VIEW>
  <VIEW id="newView">
    <TEXT value="new view"/>
  </VIEW>
</THEME>

```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Элемент THEME**](theme-element.md)
</dt> </dl>

 

 





