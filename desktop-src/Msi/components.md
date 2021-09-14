---
description: Объект Component представляет уникальный экземпляр компонента, доступного для перечисления.
ms.assetid: cdc99bc3-9e2a-49db-8c01-b9634aefac38
title: Объект Component
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Component
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 5e31d6a7c3d2422111d0d8c3247e022fa35bdc43
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127142326"
---
# <a name="component-object"></a>Объект Component

Объект Component представляет уникальный экземпляр компонента, доступного для перечисления.

**[установщик Windows 4,5 или более ранней версии](not-supported-in-windows-installer-4-5.md):** Не поддерживается. этот объект доступен, начиная с установщик Windows 5,0.

## <a name="members"></a>Элементы

Объект **компонента** имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Объект **компонента** имеет следующие свойства.



| Свойство.                                                    | Описание                                                                               |
|:------------------------------------------------------------|:------------------------------------------------------------------------------------------|
| [**компоненткоде**](component-componentcode.md)<br/> | Код компонента рассматриваемого компонента.<br/>                               |
| [**Локального**](component-context.md)<br/>             | Контекст, который был определен как применимый к рассматриваемому компоненту.<br/> |
| [**UserSID**](component-usersid.md)<br/>             | Идентификатор безопасности пользователя для перечисленного компонента.<br/>                                     |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | Windows Установщик 5,0 или более поздней версии.<br/>                                         |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl> |
| IID<br/>     | IID интерфейса \_ IComponent определяется как 000C1097-0000-0000-C000-000000000046<br/>      |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Использование интерфейса автоматизации](using-the-automation-interface.md)
</dt> <dt>

[Windows Примеры сценариев для установщика](windows-installer-scripting-examples.md)
</dt> </dl>

 

 




