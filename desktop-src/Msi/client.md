---
description: Клиентский объект представляет связь между компонентом и клиентским продуктом.
ms.assetid: ac1fbd74-fbc4-4f76-8e14-af48443a8528
title: Клиентский объект
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Client
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 75cb21a4149d8e6758ab24796949777b8052b120
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127142469"
---
# <a name="client-object"></a>Клиентский объект

Клиентский объект представляет связь между компонентом и клиентским продуктом.

**[установщик Windows 4,5 или более ранней версии](not-supported-in-windows-installer-4-5.md):** Не поддерживается. этот объект доступен, начиная с установщик Windows 5,0.

## <a name="members"></a>Элементы

**Клиентский** объект имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

**Клиентский** объект имеет эти свойства.



| Свойство.                                                 | Описание                                                 |
|:---------------------------------------------------------|:------------------------------------------------------------|
| [**компоненткоде**](client-componentcode.md)<br/> | Код компонента рассматриваемого компонента.<br/> |
| [**Локального**](client-context.md)<br/>             | Контекст продукта.<br/>                      |
| [**ProductCode**](client-productcode.md)<br/>     | Клиентское программное произведение рассматриваемого компонента.<br/> |
| [**UserSID**](client-usersid.md)<br/>             | Идентификатор безопасности пользователя для компонента.<br/>                  |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | Windows Установщик 5,0 или более поздней версии.<br/>                                         |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl> |
| IID<br/>     | IID \_ иклиент определен как 000C1098-0000-0000-C000-000000000046<br/>         |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Использование интерфейса автоматизации](using-the-automation-interface.md)
</dt> <dt>

[Windows Примеры сценариев для установщика](windows-installer-scripting-examples.md)
</dt> </dl>

 

 




