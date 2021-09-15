---
description: Извлекает идентификатор штриха для штриха, на который ссылается значение индекса в объекте Иконтекстноде.
ms.assetid: faac142e-cac1-45f9-9b40-76c50ac7006b
title: 'Метод Иконтекстноде:: Жетстрокеид (Иаком. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IContextNode.GetStrokeId
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: b193b3719ac6b67284e3ff8c4297455888f6c9cd
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572419"
---
# <a name="icontextnodegetstrokeid-method"></a>Метод Иконтекстноде:: Жетстрокеид

Извлекает идентификатор штриха для штриха, на который ссылается значение индекса в объекте [**иконтекстноде**](icontextnode.md) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetStrokeId(
  [in]  ULONG ulIndex,
  [out] LONG  *plStrokeId
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*улиндекс* \[ окне\]
</dt> <dd>

Индекс возвращаемого элемента Stroke.

</dd> <dt>

*плстрокеид* \[ заполняет\]
</dt> <dd>

Идентификатор штриха для штриха, на который ссылается параметр *улиндекс* в текущем объекте [**иконтекстноде**](icontextnode.md) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописного ввода](classes-and-interfaces---ink-analysis.md).

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

[**Иконтекстноде:: Жетстрокеидс**](icontextnode-getstrokeids.md)
</dt> <dt>

[**Иконтекстноде:: Жетстрокекаунт**](icontextnode-getstrokecount.md)
</dt> <dt>

[Справочник по анализу рукописного ввода](ink-analysis-reference.md)
</dt> </dl>

 

 




