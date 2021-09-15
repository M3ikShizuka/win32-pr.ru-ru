---
title: Сплитбуттонгаллери. Менуграупс, свойство
description: Представляет контейнер для набора элементов раскрывающегося меню в элементе управления Сплитбуттонгаллери.
ms.assetid: e30fcf9a-488b-423a-8bc4-fccbc78f74de
keywords:
- сплитбуттонгаллери. менуграупс, свойство Windows лента
topic_type:
- apiref
api_name:
- SplitButtonGallery.MenuGroups
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 72176e7d7e79b076c3a7cf4d1fd847aa4f4e0561
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127458770"
---
# <a name="splitbuttongallerymenugroups-property"></a>Сплитбуттонгаллери. Менуграупс, свойство

Представляет контейнер для набора элементов раскрывающегося меню в элементе управления [**сплитбуттонгаллери**](windowsribbon-element-splitbuttongallery.md) .

## <a name="usage"></a>Использование

``` syntax
<SplitButtonGallery.MenuGroups>
  child elements
</SplitButtonGallery.MenuGroups>
```

## <a name="attributes"></a>Атрибуты

Атрибуты отсутствуют.

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                         | Описание                                     |
|-----------------------------------------------------------------|-------------------------------------------------|
| [**менуграуп**](windowsribbon-element-menugroup.md)<br/> | Должен быть хотя бы один раз<br/> <br/> |



## <a name="parent-elements"></a>Родительские элементы



| Элемент                                                                           |
|-----------------------------------------------------------------------------------|
| [**сплитбуттонгаллери**](windowsribbon-element-splitbuttongallery.md)<br/> |



## <a name="remarks"></a>Remarks

Обязательный элемент.

Должен выполняться ровно один раз для каждого элемента [**сплитбуттонгаллери**](windowsribbon-element-splitbuttongallery.md) .

## <a name="examples"></a>Примеры

В следующем примере показана базовая разметка для элемента **сплитбуттонгаллери. менуграупс** .

В этом разделе кода показано объявление элемента управления **сплитбуттонгаллери. менуграупс** .


```XML
<!-- SplitButtonGallery -->
<Group CommandName="cmdSplitButtonGalleryGroup">
  <SplitButtonGallery CommandName="cmdSplitButtonGallery">
    <SplitButtonGallery.MenuLayout>
      <FlowMenuLayout Rows="2"
                      Columns="3"
                      Gripper="None"/>
    </SplitButtonGallery.MenuLayout>
    <SplitButtonGallery.MenuGroups>
      <MenuGroup>
        <Button CommandName="cmdButton1"></Button>
        <Button CommandName="cmdButton2"></Button>
      </MenuGroup>
      <MenuGroup>
        <Button CommandName="cmdButton3"></Button>
      </MenuGroup>
    </SplitButtonGallery.MenuGroups>
  </SplitButtonGallery>
</Group>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>              |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Элемент управления коллекции разделенных кнопок](windowsribbon-controls-splitbuttongallery.md)
</dt> <dt>

[Работа с коллекциями](ribbon-controls-galleries.md)
</dt> </dl>

 

 





