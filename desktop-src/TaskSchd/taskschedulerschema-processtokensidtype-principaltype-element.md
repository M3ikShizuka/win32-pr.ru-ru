---
title: Процесстокенсидтипе (ПринЦипалтипе), элемент
description: Указывает тип задачи «определение безопасности процесса» (SID).
ms.assetid: d9bffa92-c0dc-4332-a29c-7f2710ec34e3
keywords:
- планировщик задач элемента Процесстокенсидтипе
topic_type:
- apiref
api_name:
- ProcessTokenSidType
api_type:
- Schema
ms.topic: reference
ms.date: 05/31/2018
api_location: ''
ms.openlocfilehash: 1875da055f2719afca454d225c3bebd13b404b3a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126891485"
---
# <a name="processtokensidtype-principaltype-element"></a>Процесстокенсидтипе (ПринЦипалтипе), элемент

Указывает тип задачи «определение безопасности процесса» (SID).

``` syntax
<xs:element name="ProcessTokenSidType"
    type="processTokenSidType"
    maxOccurs="1"
    minOccurs="0"
 />
```

Элемент **процесстокенсидтипе** определяется сложным типом [**принЦипалтипе**](taskschedulerschema-principaltype-complextype.md) .

## <a name="parent-element"></a>Родительский элемент



| Элемент                                                                  | Унаследован от                                                           | Описание                                                    |
|--------------------------------------------------------------------------|------------------------------------------------------------------------|----------------------------------------------------------------|
| [**Основного**](taskschedulerschema-principal-principaltype-element.md) | [**principalType**](taskschedulerschema-principaltype-complextype.md) | Указывает учетные данные безопасности для участника.<br/> |



## <a name="remarks"></a>Комментарии

Для разработки на C++ тип идентификатора безопасности процесса указывается с помощью свойства [**IPrincipal2::P роцесстокенсидтипе**](/windows/desktop/api/taskschd/nf-taskschd-iprincipal2-get_processtokensidtype) .

## <a name="examples"></a>Примеры

Следующий XML-код определяет тип идентификатора безопасности процесса задачи.


```XML
<Principal>
    <GroupId>NT AUTHORITY\LOCAL SERVICE</GroupId>
    <ProcessTokenSidType>None</ProcessTokenSidType>
</Principal>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/>              |
| Минимальная версия сервера<br/> | Windows \[Только для настольных приложений сервера 2008 R2\]<br/> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Планировщик заданий](task-scheduler-start-page.md)
</dt> </dl>

 

 





