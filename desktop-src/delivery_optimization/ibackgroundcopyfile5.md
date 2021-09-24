---
title: Интерфейс IBackgroundCopyFile5 (Deliveryoptimization. h)
description: Используйте этот интерфейс для получения или задания общих свойств передачи файлов оптимизации доставки.
ms.assetid: 2D729717-62D2-4C69-92FE-F4289EC48DF1
keywords:
- Интерфейс IBackgroundCopyFile5
- Интерфейс IBackgroundCopyFile5, описание
topic_type:
- apiref
api_name:
- IBackgroundCopyFile5
api_location:
- dosvc.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 8274d256399efbf03f1365e55609bc601590ee47
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128519946"
---
# <a name="ibackgroundcopyfile5-interface"></a>Интерфейс IBackgroundCopyFile5

Используйте этот интерфейс для получения или задания общих свойств передачи файлов оптимизации доставки.

Чтобы получить указатель интерфейса **IBackgroundCopyFile5** , вызовите метод **Ибаккграундкопифиле:: QueryInterface** , используя __uuidof (IBackgroundCopyFile5) для идентификатора интерфейса.

## <a name="members"></a>Элементы

Интерфейс **IBackgroundCopyFile5** наследует от интерфейса [**IUnknown**](/windows/desktop/api/unknwn/nn-unknwn-iunknown) . **IBackgroundCopyFile5** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **IBackgroundCopyFile5** содержит следующие методы.



| Метод                                                  | Описание                                                         |
|:--------------------------------------------------------|:--------------------------------------------------------------------|
| [**GetProperty**](ibackgroundcopyfile5-getproperty.md) | Возвращает значение универсального свойства Баккграундкопифиле.<br/> |
| [**SetProperty**](ibackgroundcopyfile5-setproperty.md) | Задает значение универсального свойства Баккграундкопифиле.<br/> |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, только для \[ настольных приложений версии 1709\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows Server, только для \[ настольных приложений версии 1709\]<br/>                                       |
| Заголовок<br/>                   | <dl> <dt>Deliveryoptimization. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>DeliveryOptimization. idl</dt> </dl> |
| Библиотека<br/>                  | <dl> <dt>Досвк. lib</dt> </dl>                |
| DLL<br/>                      | <dl> <dt>Dosvc.dll</dt> </dl>                |
| IID<br/>                      | IID_IBackgroundCopyFile5 определен как 85C1657F-DAFC-40E8-8834-DF18EA25717E<br/>             |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ибаккграундкопифиле**](ibackgroundcopyfile.md)
</dt> <dt>

[**IBackgroundCopyFile2**](ibackgroundcopyfile2.md)
</dt> </dl>

 

