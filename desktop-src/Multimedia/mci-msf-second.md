---
title: Макрос MCI_MSF_SECOND (МЦиапи. h)
description: '\_ \_ Второй макрос MCI MSF получает компонент секунд из параметра, содержащего Упакованные минуты/секунды/кадры (MSF).'
ms.assetid: 2d455ce3-1823-46fa-a59e-b9c5c2fe5eb9
keywords:
- MCI_MSF_SECOND макрос Windows мультимедиа
topic_type:
- apiref
api_name:
- MCI_MSF_SECOND
api_location:
- mciapi.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 85dffd36354b335818079ea5b0c88d16752b4501
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370218"
---
# <a name="mci_msf_second-macro"></a>\_ \_ Второй макрос MCI MSF

**\_ \_ Второй макрос MCI MSF** получает компонент секунд из параметра, содержащего Упакованные минуты/секунды/кадры (MSF).

## <a name="syntax"></a>Синтаксис


```C++
BYTE MCI_MSF_SECOND(
   DWORD dwMSF
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*двмсф* 
</dt> <dd>

Время в формате MSF.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает компонент секунд указанной информации MSF.

## <a name="remarks"></a>Remarks

Время в формате MSF выражается в виде значения **типа DWORD** с наименьшим значащим байтом, содержащим минуты, следующим наименее значащим байтом, содержащим секунды, и следующим наименьшим значащим байтом, содержащим кадры. Наиболее значимый байт не используется.

**\_ \_ Второй макрос MCI MSF** может быть определен следующим образом:


```C++
#define MCI_MSF_SECOND(msf) ((BYTE)(((WORD)(msf)) >> 8)) 
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

 

 





