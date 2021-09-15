---
title: Дропдовнгаллери. Менулайаут, свойство
description: Представляет контейнер для раскрывающихся раскрывающихся меню Дропдовнгаллери.
ms.assetid: 7251e889-377d-4d7f-b049-bd81a202774d
keywords:
- дропдовнгаллери. менулайаут, свойство Windows лента
topic_type:
- apiref
api_name:
- DropDownGallery.MenuLayout
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 7d1b6ad3f07f369dfef90b1e6c52c34793e60520
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570306"
---
# <a name="dropdowngallerymenulayout-property"></a>Дропдовнгаллери. Менулайаут, свойство

Представляет контейнер для раскрывающихся раскрывающихся меню [**дропдовнгаллери**](windowsribbon-element-dropdowngallery.md) .

## <a name="usage"></a>Использование

``` syntax
<DropDownGallery.MenuLayout>
  child elements
</DropDownGallery.MenuLayout>
```

## <a name="attributes"></a>Атрибуты

Атрибуты отсутствуют.

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                                           | Описание                                    |
|-----------------------------------------------------------------------------------|------------------------------------------------|
| [**фловменулайаут**](windowsribbon-element-flowmenulayout.md)<br/>         | Должно выполняться только один раз<br/> <br/> |
| [**вертикалменулайаут**](windowsribbon-element-verticalmenulayout.md)<br/> | Должно выполняться только один раз<br/> <br/> |



## <a name="parent-elements"></a>Родительские элементы



| Элемент                                                                     |
|-----------------------------------------------------------------------------|
| [**дропдовнгаллери**](windowsribbon-element-dropdowngallery.md)<br/> |



## <a name="remarks"></a>Remarks

Необязательный параметр.

Может встречаться не более одного раза для каждого элемента [**дропдовнгаллери**](windowsribbon-element-dropdowngallery.md) .

> [!Note]  
> Допускается не более одного дочернего элемента ([**вертикалменулайаут**](windowsribbon-element-verticalmenulayout.md) или [**фловменулайаут**](windowsribbon-element-flowmenulayout.md)).

 

## <a name="examples"></a>Примеры

В следующем примере показана базовая разметка для [**дропдовнгаллери**](windowsribbon-element-dropdowngallery.md).

В этом разделе кода показано объявление элемента управления **дропдовнгаллери. менулайаут** .


```XML
<!-- DropDownGallery -->
<Group CommandName="cmdDropDownGalleryGroup">
  <DropDownGallery CommandName="cmdDropDownGallery"
                   TextPosition="Hide"
                   Type="Commands"
                   ItemHeight="32"
                   ItemWidth="32">
    <DropDownGallery.MenuLayout>
      <FlowMenuLayout Rows="2"
                      Columns="3"
                      Gripper="None"/>
    </DropDownGallery.MenuLayout>
    <DropDownGallery.MenuGroups>
      <MenuGroup>
        <Button CommandName="cmdButton1"></Button>
        <Button CommandName="cmdButton2"></Button>
       </MenuGroup>
       <MenuGroup>
        <Button CommandName="cmdButton3"></Button>
      </MenuGroup>
    </DropDownGallery.MenuGroups>
  </DropDownGallery>
</Group>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>              |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Элемент управления "раскрывающийся список"**](windowsribbon-element-dropdowngallery.md)
</dt> <dt>

[Работа с коллекциями](ribbon-controls-galleries.md)
</dt> </dl>

 

 





