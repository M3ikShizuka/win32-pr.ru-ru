---
title: Макрос MCI_TMSF_FRAME (МЦиапи. h)
description: '\_Макрос ТМСФ MCI \_ получает компонент frames из параметра, содержащего данные упакованных дорожек/минут/секунд/кадров (тмсф).'
ms.assetid: 1ba78d4f-4537-4955-abcc-842976b6b5b9
keywords:
- MCI_TMSF_FRAME макрос Windows мультимедиа
topic_type:
- apiref
api_name:
- MCI_TMSF_FRAME
api_location:
- mciapi.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 90872f0a9391d30d7ec3af17e85203cebe433a4c24bde35e3a27db9b40ca30aa
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119784234"
---
# <a name="mci_tmsf_frame-macro"></a>\_Макрос ТМСФ \_ MCI

Макрос **\_ тмсф MCI \_** получает компонент frames из параметра, содержащего данные упакованных дорожек/минут/секунд/кадров (тмсф).

## <a name="syntax"></a>Синтаксис


```C++
BYTE MCI_TMSF_FRAME(
   DWORD dwTMSF
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*двтмсф* 
</dt> <dd>

Время в формате ТМСФ.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает компонент frames указанной ТМСФ информации.

## <a name="remarks"></a>Remarks

Время в формате ТМСФ выражается как значение **DWORD** с наименьшим значащим байтом, содержащим дорожки, следующий младший значащий байт, содержащий минуты, следующий младший значащий байт, содержащий секунды, и самый значащий байт, содержащий кадры.

Макрос **\_ \_ тмсф MCI** определяется следующим образом:


```C++
#define MCI_TMSF_FRAME(tmsf) ((BYTE)((tmsf) >> 24)) 
```



## <a name="requirements"></a>Requirements (Требования)



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

 

 





