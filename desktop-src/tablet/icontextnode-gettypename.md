---
description: Возвращает удобное для чтения имя типа этого Иконтекстноде.
ms.assetid: 02031efd-1e9c-4e96-8dc1-280cc1a6e58f
title: Метод Иконтекстноде::-TypeName (Иаком. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IContextNode.GetTypeName
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: 741aea01401c9a266a4345a778e691eac49d9de3d41d59bba9d471cdb10c2af7
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120008464"
---
# <a name="icontextnodegettypename-method"></a>Метод Иконтекстноде:: имя_типа

Возвращает удобное для чтения имя типа этого [**иконтекстноде**](icontextnode.md).

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetTypeName(
  [out] BSTR *pbstrContextNodeType
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пбстрконтекстнодетипе* \[ заполняет\]
</dt> <dd>

Понятное для человека имя типа этого [**иконтекстноде**](icontextnode.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописного ввода](classes-and-interfaces---ink-analysis.md).

## <a name="remarks"></a>Remarks

> [!Caution]  
> Чтобы избежать утечки памяти, вызовите [**сисфристринг**](/windows/win32/api/oleauto/nf-oleauto-sysfreestring) для \* *пбстрконтекстнодетипе* , когда больше не нужно использовать строку.

 

Например, этот метод устанавливает *пбстрконтекстнодетипе* в значение "инквордноде" для узла рукописного слова (см. раздел [**Иконтекстноде:: GetType**](icontextnode-gettype.md) и [типы узлов контекста](context-node-types.md)).

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

[**Иконтекстноде:: GetType**](icontextnode-gettype.md)
</dt> <dt>

[Типы узлов контекста](context-node-types.md)
</dt> <dt>

[Справочник по анализу рукописного ввода](ink-analysis-reference.md)
</dt> </dl>

 

