---
description: Происходит, когда пользователь рисует новый объект Иинкстрокедисп для любого объекта Иинктаблет.
ms.assetid: fac5104d-d0da-40b1-a4a6-00a34718d09f
title: Событие InkEdit. Stroke (рисование. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6d21abde9deb565f207a44ddd44b51681f1bfa6a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127256669"
---
# <a name="inkeditstroke-event"></a>Событие InkEdit. Stroke

Происходит, когда пользователь рисует новый объект [**иинкстрокедисп**](/windows/desktop/api/msinkaut/nn-msinkaut-iinkstrokedisp) для любого объекта [**иинктаблет**](/windows/desktop/api/msinkaut/nn-msinkaut-iinktablet) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Stroke(
  [in]      IInkCursor     *Cursor,
  [in]      IInkStrokeDisp *Stroke,
  [in, out] VARIANT_BOOL   *Cancel
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Курсор* \[ окне\]
</dt> <dd>

Объект [**иинккурсор**](/windows/desktop/api/msinkaut/nn-msinkaut-iinkcursor) .

</dd> <dt>

*Штриховая линия* \[ окне\]
</dt> <dd>

Собранный объект [**иинкстрокедисп**](/windows/desktop/api/msinkaut/nn-msinkaut-iinkstrokedisp) .

</dd> <dt>

*Отмена* \[ в, out\]
</dt> <dd>

**Вариант \_ Значение TRUE** , чтобы отменить коллекцию объекта [**иинкстрокедисп**](/windows/desktop/api/msinkaut/nn-msinkaut-iinkstrokedisp) ; **Вариант \_ Значение FALSE** , чтобы получить объект **иинкстрокедисп** и продолжить **штрих** .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если это событие завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Комментарии

Этот метод события определен в интерфейсе **\_ иинкедитевентс** . Интерфейс **\_ иинкедитевентс** реализует интерфейс [**IDISPATCH**](/windows/win32/api/oaidl/nn-oaidl-idispatch) с идентификатором DISPID \_ иистроке.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                                     |
| Заголовок<br/>                   | <dl> <dt>«С». h (также требует \_ ввода i. c)</dt> </dl> |
| Библиотека<br/>                  | <dl> <dt>InkEd.dll</dt> </dl>                          |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[InkEdit](inkedit-control-reference.md)
</dt> <dt>

[**Интерфейс Иинккурсор**](/windows/desktop/api/msinkaut/nn-msinkaut-iinkcursor)
</dt> <dt>

[**Интерфейс Иинкстрокедисп**](/windows/desktop/api/msinkaut/nn-msinkaut-iinkstrokedisp)
</dt> </dl>

 

