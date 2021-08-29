---
description: Происходит при изменении оперативного состояния отчета.
ms.assetid: f0c4e678-1666-4f99-89de-85879eacd0ac
title: Событие Статусчанжед
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- StatusChanged
api_type:
- COM
api_location: ''
ms.openlocfilehash: 1d1babe150920bb587d24b0b16be0cf662feba252b2b38bc05dc53e3670dd49b
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119067934"
---
# <a name="statuschanged-event"></a>Событие Статусчанжед

\[Объектная модель API расположения доступна для использования в операционных системах, указанных в разделе требования. В последующих версиях он может быть изменен или недоступен. Вместо этого для доступа к расположению с веб-сайта используйте [API географического расположения W3C](/previous-versions/windows/internet-explorer/ie-developer/samples/gg589513(v=vs.85)). Чтобы получить доступ к расположению из классического приложения, используйте [**Windows. API Devices. Географическое расположение**](/uwp/api/Windows.Devices.Geolocation) .\]

Происходит при изменении оперативного состояния отчета.

## <a name="syntax"></a>Синтаксис


```JScript
.StatusChanged(
  status
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*status* 
</dt> <dd>

Новое состояние.



| Состояние                                                                                               | Значение                          |
|------------------------------------------------------------------------------------------------------|----------------------------------|
| <span id="0"></span><dl> <dt>**0**</dt> </dl> | Отчет не поддерживается.<br/> |
| <span id="1"></span><dl> <dt>**1**</dt> </dl> | Ошибка.<br/>                |
| <span id="2"></span><dl> <dt>**2**</dt> </dl> | Доступ запрещен.<br/>        |
| <span id="3"></span><dl> <dt>**3**</dt> </dl> | Инициализация.<br/>         |
| <span id="4"></span><dl> <dt>**4**</dt> </dl> | Выполняется.<br/>              |



 

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это событие не возвращает значение.

## <a name="remarks"></a>Remarks

Необходимо реализовать отдельные обработчики отчетов об изменении состояния для отчетов об административном адресе и в отчетах широты и долготы.

## <a name="examples"></a>Примеры

Пример использования этого события см. в разделе [Listening for LatLong Reports Events](/uwp/api/Windows.Devices.Geolocation).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------|
| Минимальная версия клиента<br/> | только Windows 7 \[ настольных приложений\]<br/> |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                  |



 

