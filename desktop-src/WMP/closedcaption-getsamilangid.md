---
title: Клоседкаптион. Жетсамилангид, метод
description: Метод Жетсамилангид извлекает идентификатор локали (LCID) языка, поддерживаемого текущим файлом SAMI.
ms.assetid: 35f8379a-a2f5-4b22-b1ad-3c5cc5bc5e3d
keywords:
- проигрыватель Windows Media метода жетсамилангид
- проигрыватель Windows Media метода жетсамилангид, класс клоседкаптион
- класс клоседкаптион проигрыватель Windows Media, метод жетсамилангид
topic_type:
- apiref
api_name:
- ClosedCaption.getSAMILangID
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8cd543c9cb9d884022d78a875a2f8de078c479b3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126885269"
---
# <a name="closedcaptiongetsamilangid-method"></a>Клоседкаптион. Жетсамилангид, метод

Метод **жетсамилангид** извлекает идентификатор локали (LCID) языка, поддерживаемого текущим файлом Sami.

## <a name="syntax"></a>Синтаксис


```JScript
retVal = ClosedCaption.getSAMILangID(
  index
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*индекс* \[ окне\]
</dt> <dd>

**Число** (**Long**), указывающее индекс извлекаемого кода языка.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает **число** (**Long**), содержащее LCID языка с указанным индексом.

## <a name="remarks"></a>Комментарии

Языки в файле SAMI индексируются в порядке, указанном в файле, начиная с нуля.

Этот метод нельзя использовать до открытия файла цифрового мультимедиа (*Player*.**Опенстате** равен 13).

**проигрыватель Windows Media 10 Mobile:** Этот метод не поддерживается.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 9 Series или более поздней версии.<br/>                                 |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Добавление субтитров к цифровым носителям**](adding-closed-captions-to-digital-media.md)
</dt> <dt>

[**Объект Клоседкаптион**](closedcaption-object.md)
</dt> </dl>

 

 





