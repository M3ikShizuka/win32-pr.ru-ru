---
description: Удаляет часть данных, зависящих от приложения.
ms.assetid: 41077c2f-39e3-4069-ac05-97f1785e37b7
title: 'Метод Иконтекстноде:: Ремовепропертидата (Иаком. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IContextNode.RemovePropertyData
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: 4c2fd5924b206ee296c066a908d2a59b02019f72
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127256756"
---
# <a name="icontextnoderemovepropertydata-method"></a>Метод Иконтекстноде:: Ремовепропертидата

Удаляет часть данных, зависящих от приложения.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT RemovePropertyData(
  [in] const GUID *pPropertyDataId
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппропертидатаид* \[ окне\]
</dt> <dd>

Идентификатор удаляемых данных.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописного ввода](classes-and-interfaces---ink-analysis.md).

## <a name="remarks"></a>Комментарии

**Д \_ INVALIDARG** возвращается, если параметр *ппропертидатаид* является одной из констант [свойств узла контекста](context-node-properties.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                                     |
| Заголовок<br/>                   | <dl> <dt>Иаком. h (также требуется Иаком \_ i. c)</dt> </dl> |
| DLL<br/>                      | <dl> <dt>IACom.dll</dt> </dl>                          |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**иконтекстноде**](icontextnode.md)
</dt> <dt>

[**Иконтекстноде:: Аддпропертидата**](icontextnode-addpropertydata.md)
</dt> <dt>

[**Иконтекстноде:: Контаинспропертидата**](icontextnode-containspropertydata.md)
</dt> <dt>

[**Иконтекстноде:: Жетпропертидата**](icontextnode-getpropertydata.md)
</dt> <dt>

[**Иконтекстноде:: Жетпропертидатаидс**](icontextnode-getpropertydataids.md)
</dt> <dt>

[**Иконтекстноде:: Лоадпропертиесдата**](icontextnode-loadpropertiesdata.md)
</dt> <dt>

[**Иконтекстноде:: Савепропертиесдата**](icontextnode-savepropertiesdata.md)
</dt> <dt>

[Справочник по анализу рукописного ввода](ink-analysis-reference.md)
</dt> </dl>

 

 




