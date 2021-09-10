---
title: Макрос MCI_HMS_SECOND (МЦиапи. h)
description: '\_ \_ Второй макрос MCI ХМс извлекает компонент секунд из параметра, содержащего Упакованные данные о часах/минутах/секундах (ХМс).'
ms.assetid: b6895bec-524f-4345-ae65-e75168855df2
keywords:
- MCI_HMS_SECOND макрос Windows мультимедиа
topic_type:
- apiref
api_name:
- MCI_HMS_SECOND
api_location:
- mciapi.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 30b869141d6480ba0d986450ce950097ba240009
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370200"
---
# <a name="mci_hms_second-macro"></a>\_ \_ Второй макрос MCI ХМс

**\_ \_ Второй макрос MCI ХМс** извлекает компонент секунд из параметра, содержащего Упакованные данные о часах/минутах/секундах (ХМс).

## <a name="syntax"></a>Синтаксис


```C++
BYTE MCI_HMS_SECOND(
   DWORD dwHMS
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*двхмс* 
</dt> <dd>

Время в формате ХМС.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает компонент секунд указанной информации ХМС.

## <a name="remarks"></a>Remarks

Время в формате ХМС выражается как значение **DWORD** с наименьшим значащим байтом, содержащим часы, следующий младший значащий байт, содержащий минуты, и следующий младший значащий байт, содержащий секунды. Наиболее значимый байт не используется.

**Второй макрос \_ ХМс \_ MCI** определяется следующим образом:


```C++
#define MCI_HMS_SECOND(hms) ((BYTE)((hms) >> 16)) 
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>МЦиапи. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[MCI](mci.md)
</dt> <dt>

[Макросы MCI](mci-macros.md)
</dt> </dl>

 

 





