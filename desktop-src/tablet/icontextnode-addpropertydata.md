---
description: Добавляет часть данных для конкретного приложения.
ms.assetid: 86ba37ac-8e65-4397-8ed1-37463152bebd
title: 'Метод Иконтекстноде:: Аддпропертидата (Иаком. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IContextNode.AddPropertyData
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: ed318520b8ac83acbc8ed615002fababe2a4b12d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127247816"
---
# <a name="icontextnodeaddpropertydata-method"></a>Метод Иконтекстноде:: Аддпропертидата

Добавляет часть данных для конкретного приложения.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT AddPropertyData(
  [in] const GUID  *pPropertyDataId,
  [in]       ULONG ulPropertyDataSize,
  [in]       BYTE  *pbPropertiesData
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппропертидатаид* \[ окне\]
</dt> <dd>

Глобальный уникальный идентификатор (GUID), используемый для идентификации типа данных.

</dd> <dt>

*улпропертидатасизе* \[ окне\]
</dt> <dd>

Размер данных в байтах.

</dd> <dt>

*пбпропертиесдата* \[ окне\]
</dt> <dd>

\[в, Size \_ имеет размер (улпропертидатасизе)\]

Массив 8-битовых целых чисел без знака, содержащий добавляемые сведения о свойстве.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописного ввода](classes-and-interfaces---ink-analysis.md).

## <a name="remarks"></a>Remarks

Используйте **иконтекстноде:: аддпропертидата** , чтобы связать данные с узлом контекста. Чтобы получить данные позже, используйте [**иконтекстноде:: жетпропертидата**](icontextnode-getpropertydata.md).

Анализатор рукописного ввода может удалить узел как часть анализа рукописного ввода, если только узел контекста не будет подтвержден (см. раздел [**иконтекстноде:: Confirm**](icontextnode-confirm.md)). Дополнительные сведения о синхронизации данных приложения с помощью [**иинканализер**](iinkanalyzer.md)см. в разделе [учетная запись-посредник данных с помощью анализа рукописного ввода](data-proxy-with-ink-analysis.md).

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

[**Иконтекстноде:: Жетпропертидата**](icontextnode-getpropertydata.md)
</dt> <dt>

[**Иконтекстноде:: Жетпропертидатаидс**](icontextnode-getpropertydataids.md)
</dt> <dt>

[**Иконтекстноде:: Контаинспропертидата**](icontextnode-containspropertydata.md)
</dt> <dt>

[**Иконтекстноде:: Лоадпропертиесдата**](icontextnode-loadpropertiesdata.md)
</dt> <dt>

[**Иконтекстноде:: Ремовепропертидата**](icontextnode-removepropertydata.md)
</dt> <dt>

[**Иконтекстноде:: Савепропертиесдата**](icontextnode-savepropertiesdata.md)
</dt> </dl>

 

 




