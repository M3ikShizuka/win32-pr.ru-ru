---
title: Интерфейс Ибаккграундкоперрор (Deliveryoptimization. h)
description: Используйте интерфейс Ибаккграундкоперрор, чтобы определить причину ошибки, и если процесс перемещения может быть продолжен.
ms.assetid: 7DCB63CF-4180-4DC3-9093-07C4F8CF7A8E
keywords:
- Интерфейс Ибаккграундкоперрор
- Интерфейс Ибаккграундкоперрор, описание
topic_type:
- apiref
api_name:
- IBackgroundCopyError
api_location:
- dosvc.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 853ce5b6c1dfb9c90b7a5800f41a8a54fe094c0f
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128520266"
---
# <a name="ibackgroundcopyerror-interface"></a>Интерфейс Ибаккграундкоперрор

Используйте интерфейс **ибаккграундкоперрор** , чтобы определить причину ошибки, и если процесс перемещения может быть продолжен.

Оптимизация доставки создает объект Error только в том случае, если состояние задания — BG_JOB_STATE_ERROR или BG_JOB_STATE_TRANSIENT_ERROR. Оптимизация доставки не создает объект Error при сбое метода интерфейса **ибаккграундкопикскскскс** . Объект Error доступен до тех пор, пока оптимизация доставки не начнет передачу данных (состояние задания меняется на BG_JOB_STATE_TRANSFERRING) для задания.

Чтобы получить объект **ибаккграундкоперрор** , вызовите метод [**использованием метода ibackgroundcopyjob::**](ibackgroundcopyjob-geterror.md) GetObject.

## <a name="members"></a>Элементы

Интерфейс **ибаккграундкоперрор** наследует от интерфейса [**IUnknown**](/windows/desktop/api/unknwn/nn-unknwn-iunknown) . **Ибаккграундкоперрор** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **ибаккграундкоперрор** содержит следующие методы.



| Метод                                                   | Описание                                                                                 |
|:---------------------------------------------------------|:--------------------------------------------------------------------------------------------|
| [**Ошибка**](ibackgroundcopyerror-geterror-method.md) | Извлекает код ошибки и определяет контекст, в котором произошла ошибка.<br/> |
| [**Файл.**](ibackgroundcopyerror-getfile-method.md)   | Извлекает указатель интерфейса на объект File, связанный с ошибкой.<br/>     |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, только для \[ настольных приложений версии 1709\]<br/>                                           |
| Минимальная версия сервера<br/> | Windows Server, только для \[ настольных приложений версии 1709\]<br/>                                       |
| Заголовок<br/>                   | <dl> <dt>Deliveryoptimization. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>DeliveryOptimization. idl</dt> </dl> |
| Библиотека<br/>                  | <dl> <dt>Досвк. lib</dt> </dl>                |
| DLL<br/>                      | <dl> <dt>Dosvc.dll</dt> </dl>                |
| IID<br/>                      | IID_IBackgroundCopyError определен как 19C613A0-FCB8-4F28-81AE-897C3D078F81<br/>             |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**BG_JOB_STATE**](bg-job-state-.md)
</dt> <dt>

[**Использованием метода ibackgroundcopyjob:: возникла ошибка**](ibackgroundcopyjob-geterror.md)
</dt> <dt>

[**Использованием метода ibackgroundcopyjob:: State**](ibackgroundcopyjob-getstate.md)
</dt> <dt>

[**Ибаккграундкопикаллбакк:: Жоберрор**](ibackgroundcopycallback-joberror-method.md)
</dt> </dl>

 

