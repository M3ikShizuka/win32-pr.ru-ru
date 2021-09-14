---
description: Происходит, когда класс Инкрекогнизерконтекст создает результаты после вызова метода метода Баккграундрекогнизевисалтернатес.
ms.assetid: 5e86a4d5-c0a7-4283-81cc-ec3a26f74880
title: Событие Инкрекогнизерконтекст. Рекогнитионвисалтернатес (Мсинкаут. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e4a7d35d8281305b0cb5f84114bb2f2fa0e718c8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127247759"
---
# <a name="inkrecognizercontextrecognitionwithalternates-event"></a>Инкрекогнизерконтекст. Рекогнитионвисалтернатес, событие

Происходит, когда [**класс инкрекогнизерконтекст**](inkrecognizercontext-class.md) создает результаты после вызова метода [**метода баккграундрекогнизевисалтернатес**](/windows/desktop/api/msinkaut/nf-msinkaut-iinkrecognizercontext-backgroundrecognizewithalternates) .

## <a name="syntax"></a>Синтаксис


```C++
void RecognitionWithAlternates(
  [in] IInkRecognitionResult *RecognitionResult,
  [in] VARIANT               CustomData,
  [in] InkRecognitionStatus  RecognitionStatus
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Рекогнитионресулт* \[ окне\]
</dt> <dd>

Результат распознавания события.

</dd> <dt>

*CustomData* \[ окне\]
</dt> <dd>

Пользовательские данные для результата распознавания.

Дополнительные сведения о структуре вариантов см. в разделе [Использование библиотеки COM](using-the-com-library.md).

</dd> <dt>

*Рекогнитионстатус* \[ окне\]
</dt> <dd>

Состояние распознавания на самый последний результат распознавания.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Remarks

Поведение прикладного программного интерфейса (API) непредсказуемо, если вы попытаетесь получить доступ к исходному объекту [**инкрекогнизерконтекст**](inkrecognizercontext-class.md) из обработчика событий распознавания. Не пытайтесь это сделать. Вместо этого, если это необходимо, создайте флаг и задайте его в обработчике событий [**распознавания**](inkrecognizercontext-recognition.md) . Затем можно опросить этот флаг, чтобы определить, когда следует изменять свойства **инкрекогнизерконтекст** за пределами обработчика событий.

Этот метод события определен в \_ интерфейсе иинкевентс. \_Интерфейс иинкевентс реализует интерфейс [**IDispatch**](/windows/win32/api/oaidl/nn-oaidl-idispatch) с идентификатором DISPID \_ иререкогнитионвисалтернатес.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                                                       |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                                           |
| Заголовок<br/>                   | <dl> <dt>Мсинкаут. h (также требуется Мсинкаут \_ i. c)</dt> </dl> |
| Библиотека<br/>                  | <dl> <dt>InkObj.dll</dt> </dl>                               |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Класс Инкрекогнизерконтекст**](inkrecognizercontext-class.md)
</dt> <dt>

[**Метод Баккграундрекогнизевисалтернатес**](/windows/desktop/api/msinkaut/nf-msinkaut-iinkrecognizercontext-backgroundrecognizewithalternates)
</dt> <dt>

[**Метод распознавания**](/windows/desktop/api/msinkaut/nf-msinkaut-iinkrecognizercontext-recognize)
</dt> <dt>

[**Интерфейс Иинкрекогнитионресулт**](/windows/desktop/api/msinkaut/nn-msinkaut-iinkrecognitionresult)
</dt> </dl>

 

