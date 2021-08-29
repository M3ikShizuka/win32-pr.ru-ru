---
description: Возвращает идентификаторы, для которых имеются данные свойств.
ms.assetid: c9c491b7-95e2-421a-8632-f65844cd5ef9
title: 'Метод Иконтекстноде:: Жетпропертидатаидс (Иаком. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IContextNode.GetPropertyDataIds
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: 94aab2b91a5da9588de65f5a48bf496bdceae71bf4aa90f82f3969cbe6a9e76e
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119935374"
---
# <a name="icontextnodegetpropertydataids-method"></a>Метод Иконтекстноде:: Жетпропертидатаидс

Возвращает идентификаторы, для которых имеются данные свойств.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetPropertyDataIds(
  [out] ULONG *pulGuidCount,
  [out] GUID  **ppGuids
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пулгуидкаунт* \[ заполняет\]
</dt> <dd>

Количество свойств.

</dd> <dt>

*ппгуидс* \[ заполняет\]
</dt> <dd>

Идентификаторы, для которых имеются данные свойств.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописного ввода](classes-and-interfaces---ink-analysis.md).

## <a name="remarks"></a>Remarks

> [!Caution]  
> Чтобы избежать утечки памяти, используйте [**CoTaskMemFree**](/windows/desktop/api/combaseapi/nf-combaseapi-cotaskmemfree) , чтобы освободить память от \* *ппгуидс* , если эта информация больше не нужна.

 

Этот метод возвращает идентификаторы конкретного приложения для добавленных данных свойства. Он также возвращает идентификаторы для внутренних данных свойства, которые описаны константами [свойств узла контекста](context-node-properties.md) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                                     |
| Заголовок<br/>                   | <dl> <dt>Иаком. h (также требуется Иаком \_ i. c)</dt> </dl> |
| DLL<br/>                      | <dl> <dt>IACom.dll</dt> </dl>                          |



## <a name="see-also"></a>См. также

<dl> <dt>

[**иконтекстноде**](icontextnode.md)
</dt> <dt>

[**Иконтекстноде:: Жетпропертидата**](icontextnode-getpropertydata.md)
</dt> <dt>

[**Иконтекстноде:: Контаинспропертидата**](icontextnode-containspropertydata.md)
</dt> <dt>

[**Иконтекстноде:: Ремовепропертидата**](icontextnode-removepropertydata.md)
</dt> <dt>

[Справочник по анализу рукописного ввода](ink-analysis-reference.md)
</dt> </dl>

 

