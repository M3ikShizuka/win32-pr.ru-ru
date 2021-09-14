---
title: Элемент Description
description: Обратите внимание, что в этом разделе описываются функции, предназначенные для использования Интернет-магазинами. | Description, элемент
ms.assetid: 4d9ff447-e5a4-46b1-b599-87202077abfb
keywords:
- элемент Description проигрыватель Windows Media
topic_type:
- apiref
api_name:
- Description Element
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 4318a7936f4713d3ff89a2fa73731eea0cdd97db
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126885256"
---
# <a name="description-element"></a>Элемент Description

> [!Note]  
> В этом разделе описываются функции, предназначенные для использования в Интернет-магазинах. Использование этой функции вне контекста Интернет-магазина не поддерживается.

 

элемент **description** указывает маркетинговое описание интернет-магазина, которое отображается при первом запуске пользователя с установкой проигрыватель Windows Media.

``` syntax
<Description>
    text string
</Description>
```

## <a name="attributes"></a>Атрибуты

Этот элемент не содержит атрибуты.

## <a name="parentchild-elements"></a>Родительские и дочерние элементы



| Иерархия       | Элемент         |
|-----------------|-----------------|
| Родительские элементы | **ServiceInfo** |
| Дочерние элементы  | None            |



 

## <a name="remarks"></a>Remarks

Длина описания должна быть меньше или равна 255 символам.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-------------------------------------|
| Версия<br/> | проигрыватель Windows Media 11.<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Пример документа ServiceInfo для Интернет-магазина типа 1**](example-serviceinfo-document-for-a-type-1-online-store.md)
</dt> <dt>

[**Пример документа ServiceInfo для Интернет-магазина типа 2**](example-serviceinfo-document-for-a-type-2-online-store.md)
</dt> <dt>

[**Документ ServiceInfo**](serviceinfo-document.md)
</dt> </dl>

 

 





