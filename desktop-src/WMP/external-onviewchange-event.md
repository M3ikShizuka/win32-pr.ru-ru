---
title: Внешнее событие Онвиевчанже
description: Обратите внимание, что в этом разделе описываются функции, предназначенные для использования в Интернет-магазинах. Использование этой функции вне контекста Интернет-магазина не поддерживается. событие онвиевчанже возникает при изменении представления в проигрыватель Windows Media.
ms.assetid: aa1378ad-8b84-4592-85c5-5e284be05ea6
keywords:
- проигрыватель Windows Media события External. онвиевчанже
topic_type:
- apiref
api_name:
- External.OnViewChange Event
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6c7144e03955fb67ed90cad4a4336bf782ca1566
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127241885"
---
# <a name="externalonviewchange-event"></a>Внешнее событие Онвиевчанже

> [!Note]  
> В этом разделе описываются функции, предназначенные для использования в Интернет-магазинах. Использование этой функции вне контекста Интернет-магазина не поддерживается.

 

событие **онвиевчанже** возникает при изменении представления в проигрыватель Windows Media.

``` syntax
window.external.OnViewChange = FunctionName
```

## <a name="possible-values"></a>Возможные значения

это свойство только для записи, которое указывает имя функции в скрипте, проигрыватель Windows Media вызывается при возникновении события.

## <a name="parameters"></a>Параметры

Функция, обрабатывающая это событие, не имеет параметров.

## <a name="remarks"></a>Remarks

представление в проигрыватель Windows Media может измениться по любой из следующих причин:

-   пользователь взаимодействует с проигрыватель Windows Media пользовательским интерфейсом.
-   Пользователь взаимодействует со страницей обнаружения, а скрипт на странице обнаружения вызывает [External. чанжевиев](external-changeview.md).
-   Пользователь взаимодействует со страницей обнаружения, а скрипт на странице обнаружения вызывает [External. чанжевиевонлинелист](external-changeviewonlinelist.md).

когда представление изменяется в проигрыватель Windows Media, проигрыватель вызывает [ивмпконтентпартнер::-template](/previous-versions/windows/desktop/api/contentpartner/nf-contentpartner-iwmpcontentpartner-gettemplate) , чтобы получить URL-адрес следующей отображаемой страницы обнаружения. Однако до того, как проигрыватель отобразит новую страницу обнаружения, он вызывает событие **онвиевчанже** . если обработчик событий **онвиевчанже** вызывает [External. канцелнавигате](external-cancelnavigate.md), проигрыватель Windows Media не отображает новую страницу обнаружения. Вместо этого будет отображаться текущая страница обнаружения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 11<br/>                                                 |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Внешний объект для Интернет-магазинов типа 1**](external-object-for-type-1-online-stores.md)
</dt> <dt>

[**External. Чанжевиев**](external-changeview.md)
</dt> <dt>

[**External. Чанжевиевонлинелист**](external-changeviewonlinelist.md)
</dt> </dl>

 

 





