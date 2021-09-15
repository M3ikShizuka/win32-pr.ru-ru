---
description: Происходит при добавлении одного или нескольких штрихов в коллекцию Инкстрокес.
ms.assetid: d32dcaef-3beb-4ee1-84d6-5944278936f6
title: Событие Инкстрокес. Строкесаддед (Мсинкаут. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a53bf1f511b5809cfb9a6ca0a2f683f0e85540af
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460240"
---
# <a name="inkstrokesstrokesadded-event"></a>Инкстрокес. Строкесаддед, событие

Происходит при добавлении одного или нескольких штрихов в коллекцию [инкстрокес](/previous-versions/windows/desktop/legacy/ms703293(v=vs.85)) .

## <a name="syntax"></a>Синтаксис


```C++
void StrokesAdded(
  [in] VARIANT StrokeIds
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Строкеидс* \[ окне\]
</dt> <dd>

Целочисленный массив идентификаторов для каждого объекта [**иинкстрокедисп**](/windows/desktop/api/msinkaut/nn-msinkaut-iinkstrokedisp) , добавляемого при возникновении этого события.

Дополнительные сведения о структуре вариантов см. в разделе [Использование библиотеки COM](using-the-com-library.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Remarks

Этот метод события определен в \_ интерфейсе иинкевентс. \_Интерфейс иинкевентс реализует интерфейс [**IDispatch**](/windows/win32/api/oaidl/nn-oaidl-idispatch) с идентификатором DISPID \_ сестрокесаддед.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                                                       |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                                           |
| Заголовок<br/>                   | <dl> <dt>Мсинкаут. h (также требуется Мсинкаут \_ i. c)</dt> </dl> |
| Библиотека<br/>                  | <dl> <dt>InkObj.dll</dt> </dl>                               |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Коллекция Инкстрокес](/previous-versions/windows/desktop/legacy/ms703293(v=vs.85))
</dt> <dt>

[**Добавить метод \[ Инкстрокес Collection\]**](/windows/desktop/api/msinkaut/nf-msinkaut-iinkstrokes-add)
</dt> <dt>

[**Класс Инкдисп**](inkdisp-class.md)
</dt> </dl>

 

