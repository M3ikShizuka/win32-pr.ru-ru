---
title: Свойство Ribbon. Аппликатионмену
description: Представляет меню приложения. | Свойство Ribbon. Аппликатионмену
ms.assetid: 6945e976-8ac8-40fa-8e71-31812871b496
keywords:
- свойство ribbon. аппликатионмену Windows ленты
topic_type:
- apiref
api_name:
- Ribbon.ApplicationMenu
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c9e6546e39690888b5ee4375fbeeb812450b18d05b77ddb2fd6d6c283fdf4e1b
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119710494"
---
# <a name="ribbonapplicationmenu-property"></a>Свойство Ribbon. Аппликатионмену

Представляет меню приложения.

## <a name="usage"></a>Использование

``` syntax
<Ribbon.ApplicationMenu>
  child elements
</Ribbon.ApplicationMenu>
```

## <a name="attributes"></a>Атрибуты

Атрибуты отсутствуют.

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                     | Описание                                    |
|-----------------------------------------------------------------------------|------------------------------------------------|
| [**аппликатионмену**](windowsribbon-element-applicationmenu.md)<br/> | Должно выполняться только один раз<br/> <br/> |



## <a name="parent-elements"></a>Родительские элементы



| Элемент                                                   |
|-----------------------------------------------------------|
| [**Лента**](windowsribbon-element-ribbon.md)<br/> |



## <a name="remarks"></a>Remarks

Обязательный.

Может встречаться не более одного раза для каждой [**ленты**](windowsribbon-element-ribbon.md).

## <a name="examples"></a>Примеры

В следующем примере показана базовая разметка для элемента **Ribbon. аппликатионмену** .

В этом разделе кода показано объявление элемента управления **Ribbon. аппликатионмену** .


```XML
<!-- Control declarations for Application Menu items. -->
<Ribbon.ApplicationMenu>
  <ApplicationMenu CommandName="cmdFileMenu">
    <!-- Most recently used items collection. -->
    <ApplicationMenu.RecentItems>
      <RecentItems CommandName="cmdMRUItems"/>
    </ApplicationMenu.RecentItems>
    <!-- Menu items collection. -->
    <MenuGroup>
      <Button CommandName="cmdNew" />
      <Button CommandName="cmdOpen" />
      <Button CommandName="cmdSave" />
    </MenuGroup>
    <MenuGroup>
      <Button CommandName="cmdPrint" />
      <Button CommandName="cmdExit" />
    </MenuGroup>
  </ApplicationMenu>
</Ribbon.ApplicationMenu>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>              |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/> |



 

 





