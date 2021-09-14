---
title: Внешнее событие Ончанжевиевонлинелистеррор
description: Обратите внимание, что в этом разделе описываются функции, предназначенные для использования в Интернет-магазинах. | Внешнее событие Ончанжевиевонлинелистеррор
ms.assetid: f53dfc80-a7d7-42b1-b390-e90aa108145f
keywords:
- проигрыватель Windows Media события External. ончанжевиевонлинелистеррор
topic_type:
- apiref
api_name:
- External.OnChangeViewOnlineListError Event
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 09e9ff854893268a00cb7b5f2fb35409be2e70e8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127241897"
---
# <a name="externalonchangeviewonlinelisterror-event"></a>Внешнее событие Ончанжевиевонлинелистеррор

> [!Note]  
> В этом разделе описываются функции, предназначенные для использования в Интернет-магазинах. Использование этой функции вне контекста Интернет-магазина не поддерживается.

 

Событие **ончанжевиевонлинелистеррор** возникает, когда вызов метода [External. чанжевиевонлинелист](external-changeviewonlinelist.md) приводит к ошибке.

``` syntax
window.external.OnChangeViewOnlineListError = functionname
```

## <a name="possible-values"></a>Возможные значения

это свойство только для записи, которое указывает имя функции в скрипте, проигрыватель Windows Media вызывается при возникновении события.

## <a name="parameters"></a>Параметры

Функция, обрабатывающая эту ошибку, имеет следующие параметры.

<dl> <dt>

<span id="hr"></span><span id="HR"></span>*кадров*
</dt> <dd>

Код ошибки **HRESULT** , указывающий причину сбоя.

</dd> <dt>

<span id="LibraryLocationType"></span><span id="librarylocationtype"></span><span id="LIBRARYLOCATIONTYPE"></span>*либрарилокатионтипе*
</dt> <dd>

Та же строка, которая была передана в параметре **либрарилокатионтипе** объекта **чанжевиевонлинелист**.

</dd> <dt>

<span id="LibraryLocationID"></span><span id="librarylocationid"></span><span id="LIBRARYLOCATIONID"></span>*либрарилокатионид*
</dt> <dd>

Та же строка, которая была передана в параметре **либрарилокатионид** объекта **чанжевиевонлинелист**.

</dd> <dt>

<span id="Params"></span><span id="params"></span><span id="PARAMS"></span>*Params*
</dt> <dd>

Та же строка, которая была передана в параметре **params** объекта **чанжевиевонлинелист**.

</dd> <dt>

<span id="FriendlyName"></span><span id="friendlyname"></span><span id="FRIENDLYNAME"></span>*FriendlyName*
</dt> <dd>

Та же строка, которая была передана в параметре **FriendlyName** параметра **чанжевиевонлинелист**.

</dd> <dt>

<span id="ListType"></span><span id="listtype"></span><span id="LISTTYPE"></span>*листтипе*
</dt> <dd>

Та же строка, которая была передана в параметре **листтипе** объекта **чанжевиевонлинелист**.

</dd> <dt>

<span id="ViewMode"></span><span id="viewmode"></span><span id="VIEWMODE"></span>*ViewMode*
</dt> <dd>

Та же строка, которая была передана в параметре **ViewMode** объекта **чанжевиевонлинелист**.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 11<br/>                                                 |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Внешний объект для Интернет-магазинов типа 1**](external-object-for-type-1-online-stores.md)
</dt> </dl>

 

 





