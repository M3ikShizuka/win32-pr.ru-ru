---
description: Управляет отложенной операцией приостановки приложения.
ms.assetid: 9F40659E-9B16-4FC9-B320-5679BB8A8161
title: Интерфейс Исуспендингдеферрал (Windows. ApplicationModel. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ISuspendingDeferral
api_type:
- COM
api_location:
- Windows.ApplicationModel.h
ms.openlocfilehash: 16a9d61dc68d296d39ab5a76b634d136a8e88b8987ac4990696a43ab396b68e9
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119898664"
---
# <a name="isuspendingdeferral-interface"></a>Интерфейс Исуспендингдеферрал

Управляет отложенной операцией приостановки приложения.

## <a name="members"></a>Элементы

Интерфейс **исуспендингдеферрал** наследует от [**IInspectable**](/windows/win32/api/inspectable/nn-inspectable-iinspectable). **Исуспендингдеферрал** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **исуспендингдеферрал** содержит следующие методы.



| Метод                                           | Описание                                                                                  |
|:-------------------------------------------------|:---------------------------------------------------------------------------------------------|
| [**Завершить**](isuspendingdeferral-complete.md) | Уведомляет систему, что приложение сохранило свои данные и готово к приостановке.<br/> |



 

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ только классические приложения\]<br/>                                                              |
| Минимальная версия сервера<br/> | Windows Server 2012 \[ только классические приложения\]<br/>                                                    |
| Заголовок<br/>                   | <dl> <dt>Windows. ApplicationModel. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Windows. ApplicationModel. idl</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**IInspectable**](/windows/win32/api/inspectable/nn-inspectable-iinspectable)
</dt> <dt>

[**исуспендинжевентаргс**](isuspendingeventargs.md)
</dt> <dt>

[**исуспендингоператион**](isuspendingoperation.md)
</dt> </dl>

 

 
