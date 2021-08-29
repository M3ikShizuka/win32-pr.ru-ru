---
title: Свойство Ribbon. Хелпбуттон
description: Представляет контейнер для кнопки "Справка".
ms.assetid: a64239b2-2440-4bcf-8fd7-079003de6d8c
keywords:
- свойство ribbon. хелпбуттон Windows ленты
topic_type:
- apiref
api_name:
- Ribbon.HelpButton
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0ba568fcd18ab16e1c8bd878dc786b2c415a0329d1bd430e78ec9b03a73424df
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119933198"
---
# <a name="ribbonhelpbutton-property"></a>Свойство Ribbon. Хелпбуттон

Представляет контейнер для [кнопки "Справка"](windowsribbon-controls-helpbutton.md).

## <a name="usage"></a>Использование

``` syntax
<Ribbon.HelpButton>
  child elements
</Ribbon.HelpButton>
```

## <a name="attributes"></a>Атрибуты

Атрибуты отсутствуют.

## <a name="child-elements"></a>Дочерние элементы



| Элемент                                                           | Описание                                   |
|-------------------------------------------------------------------|-----------------------------------------------|
| [**хелпбуттон**](windowsribbon-element-helpbutton.md)<br/> | Может выполняться не более одного раза<br/> <br/> |



## <a name="parent-elements"></a>Родительские элементы



| Элемент                                                   |
|-----------------------------------------------------------|
| [**Лента**](windowsribbon-element-ribbon.md)<br/> |



## <a name="remarks"></a>Remarks

Необязательный элемент.

Может встречаться не более одного раза для каждой [**ленты**](windowsribbon-element-ribbon.md).

## <a name="examples"></a>Примеры

В следующем примере показана базовая разметка, необходимая для реализации кнопки справки на ленте.

В этом разделе кода показано объявление команды **Ribbon. хелпбуттон** .


```XML
<Command Name="cmdHelp"
         Symbol="IDR_CMD_HELP">      
</Command>
```



В этом разделе кода показано объявление элемента управления **Ribbon. хелпбуттон** .


```XML
<Ribbon.HelpButton>
  <HelpButton CommandName="cmdHelp"/>
</Ribbon.HelpButton>
```



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>              |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/> |



 

 





