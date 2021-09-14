---
description: Происходит перед удалением штрихов из свойства рукописного ввода.
ms.assetid: 09468416-ad08-48ea-aa4a-3af0fe553f3d
title: Событие InkOverlay. Строкесделетинг (Мсинкаут. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 64422e61869c633514c3e219e3d090476a693dd6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127256618"
---
# <a name="inkoverlaystrokesdeleting-event"></a>Событие InkOverlay. Строкесделетинг

Происходит перед удалением штрихов из свойства [**рукописного ввода**](/windows/desktop/api/msinkaut/nf-msinkaut-iinkcollector-get_ink) .

## <a name="syntax"></a>Синтаксис


```C++
void StrokesDeleting(
  [in] IInkStrokes *Strokes
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Штрихи* \[ окне\]
</dt> <dd>

Коллекция [инкстрокес](/previous-versions/windows/desktop/legacy/ms703293(v=vs.85)) , удаленная при срабатывании события **строкесделетинг** .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Комментарии

Этот метод события определен в \_ \_ интерфейсах диспетчеризации иинковерлайевентс и иинкпиктуривентс (DISP) с идентификатором DISPID \_ иоестрокесделетинг.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                                                       |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                                           |
| Заголовок<br/>                   | <dl> <dt>Мсинкаут. h (также требуется Мсинкаут \_ i. c)</dt> </dl> |
| Библиотека<br/>                  | <dl> <dt>InkObj.dll</dt> </dl>                               |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс InkOverlay**](inkoverlay-class.md)
</dt> <dt>

[**Свойство рукописного ввода \[ класса InkCollector/InkOverLay\]**](/windows/desktop/api/msinkaut/nf-msinkaut-iinkcollector-get_ink)
</dt> </dl>

 

