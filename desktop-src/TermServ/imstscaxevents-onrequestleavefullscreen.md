---
title: Имстскаксевентс Онрекуестлеавефуллскрин, метод
description: Вызывается, когда клиент запрашивает, чтобы выйти из полноэкранного режима, а свойству Имстскадванцедсеттингс помещается \_ контаинерхандледфуллскрин присвоено ненулевое значение.
ms.assetid: db6ee012-8288-4360-98b2-12858ea65baa
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Онрекуестлеавефуллскрин
- Службы удаленных рабочих столов метода Онрекуестлеавефуллскрин, интерфейс Имстскаксевентс
- Службы удаленных рабочих столов интерфейса Имстскаксевентс, метод Онрекуестлеавефуллскрин
topic_type:
- apiref
api_name:
- IMsTscAxEvents.OnRequestLeaveFullScreen
api_location:
- MsTscAx.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e814d6153e32fdf4fa498a6630fc9ca2908510e2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127259067"
---
# <a name="imstscaxeventsonrequestleavefullscreen-method"></a>Метод Имстскаксевентс:: Онрекуестлеавефуллскрин

Вызывается, когда клиент запрашивает, чтобы выйти из полноэкранного режима, а свойство [**имстскадванцедсеттингс::p UT \_ контаинерхандледфуллскрин**](imstscadvancedsettings-containerhandledfullscreen.md) установлено в ненулевое значение.

## <a name="syntax"></a>Синтаксис


```C++
void OnRequestLeaveFullScreen();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

В полноэкранном режиме, поддерживающем контейнеры, контейнер должен оставить стандартный полноэкранный режим в ответ на это событие.

Дополнительные сведения о веб-подключение к удаленному рабочему столу см. в разделе [требования для веб-подключение к удаленному рабочему столу](requirements-for-remote-desktop-web-connection.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                               |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                         |
| Библиотека типов<br/>             | <dl> <dt>MsTscAx.dll</dt> </dl> |
| DLL<br/>                      | <dl> <dt>MsTscAx.dll</dt> </dl> |
| IID<br/>                      | Имстскаксевентс определяется как 336d5562-efa8-482e-8cb3-c5c0fc7a7db6<br/>           |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**имстскаксевентс**](imstscaxevents-interface.md)
</dt> </dl>

 

 





