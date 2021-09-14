---
title: External. Либрарилокатионтипе
description: Обратите внимание, что в этом разделе описываются функции, предназначенные для использования в Интернет-магазинах. | External. Либрарилокатионтипе
ms.assetid: aaf20147-8331-40bd-a5cd-5ee9b8e2d022
keywords:
- External. либрарилокатионтипе проигрыватель Windows Media
topic_type:
- apiref
api_name:
- External.libraryLocationType
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a2c2f14940a2ad41bed24493396e2bacfba2f0a1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127241933"
---
# <a name="externallibrarylocationtype"></a>External. Либрарилокатионтипе

> [!Note]  
> В этом разделе описываются функции, предназначенные для использования в Интернет-магазинах. Использование этой функции вне контекста Интернет-магазина не поддерживается.

 

свойство **либрарилокатионтипе** извлекает [константу расположения библиотеки](library-location-constants.md) , которая указывает тип текущего представления в проигрыватель Windows Media.

``` syntax
window.external.libraryLocationType
      
```

## <a name="possible-values"></a>Возможные значения

Это свойство является **строкой** только для чтения, содержащей одну из констант расположения библиотеки.

## <a name="remarks"></a>Remarks

Это свойство работает в сочетании со свойством [External. либрарилокатионид](external-librarylocationid.md) . Например, предположим, что **либрарилокатионтипе** равен кпалбумид, а **либрарилокатионид** равен 3. это означает, что в текущем представлении в проигрыватель Windows Media отображается альбом с идентификатором 3. дополнительные сведения о том, как проигрыватель Windows Media характеризует представления содержимого интернет-магазина, см. в разделе [расположение и выбранный элемент](location-and-selected-item.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 11.<br/>                                                |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Внешний объект для Интернет-магазинов типа 1**](external-object-for-type-1-online-stores.md)
</dt> <dt>

[**External. Либрарилокатионид**](external-librarylocationid.md)
</dt> <dt>

[**Расположение и выбранный элемент**](location-and-selected-item.md)
</dt> </dl>

 

 





