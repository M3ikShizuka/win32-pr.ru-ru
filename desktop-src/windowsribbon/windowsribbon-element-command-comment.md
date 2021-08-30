---
title: Свойство Command. Comment
description: Представляет комментарий или аннотацию для команды.
ms.assetid: 4ac5c7d4-9627-4703-bd3c-594d9497ba24
keywords:
- свойство Command. Comment Windows лента
topic_type:
- apiref
api_name:
- Command.Comment
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4eef6b5366f61f15fda808ca60264de5d28322b8b41a2d6e986e36282a95fbd6
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119931644"
---
# <a name="commandcomment-property"></a>Свойство Command. Comment

Представляет комментарий или аннотацию для команды.

## <a name="usage"></a>Использование

``` syntax
<Command.Comment/>
```

## <a name="attributes"></a>Атрибуты

Атрибуты отсутствуют.

## <a name="child-elements"></a>Дочерние элементы

Нет дочерних элементов.

## <a name="parent-elements"></a>Родительские элементы



| Элемент                                                     |
|-------------------------------------------------------------|
| [**Команда**](windowsribbon-element-command.md)<br/> |



## <a name="remarks"></a>Remarks

Необязательный элемент.

Для каждой [**команды**](windowsribbon-element-command.md)может выполняться не более одного раза.

Комментарий связан с определением команды в файле заголовка ленты, например `#define cmdSave 25003 /* Save */` .

Этот элемент содержит значение типа *xs: String*.

Максимальная длина составляет 250 символов.

## <a name="examples"></a>Примеры

В следующем примере показана разметка для элемента [**Command**](windowsribbon-element-command.md) с объявлением **Command. Comment** .


```XML
<Command>
  <Command.Name>cmdSave</Command.Name>
  <Command.Symbol>ID_FILE_SAVE</Command.Symbol>
  <Command.Comment>Save</Command.Comment>
  <Command.Id>25003</Command.Id>
  <Command.LabelTitle>
    <String>
      <String.Content>Label for Save</String.Content>
      <String.Id>59999</String.Id>
      <String.Symbol>strSave</String.Symbol>
    </String>
  </Command.LabelTitle>
  <Command.TooltipTitle>Tooltip title with &amp;&amp; for Save Command</Command.TooltipTitle>
  <Command.TooltipDescription>Tooltip description for Save Command.</Command.TooltipDescription>
  <Command.Keytip>s1</Command.Keytip>
</Command>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>              |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/> |



 

 





