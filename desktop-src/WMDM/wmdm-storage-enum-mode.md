---
title: Перечисление WMDM_STORAGE_ENUM_MODE
description: '\_Тип перечисления "режим перечисления хранилища вмдм" \_ \_ определяет способ перечисления содержимого в хранилище. Это перечисление используется IWMDMStorage3 Сетенумпреференце.'
ms.assetid: 38293e54-92e4-4f0a-bdea-5dc684a9548b
keywords:
- WMDM_STORAGE_ENUM_MODE перечисление Windows Media диспетчер устройств
topic_type:
- apiref
api_name:
- WMDM_STORAGE_ENUM_MODE
api_location:
- wmdm.idl
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8ba8b524618ebc0c5d40f9f4e9f0ad0871b7c8c39a0919d594a39248bc2d6dc6
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120004774"
---
# <a name="wmdm_storage_enum_mode-enumeration"></a>\_ \_ Перечисление режима перечисления вмдм в хранилище \_

Тип перечисления " **\_ \_ \_ режим перечисления хранилища вмдм** " определяет способ перечисления содержимого в хранилище. Это перечисление используется [**IWMDMStorage3:: сетенумпреференце**](/windows/desktop/api/mswmdm/nf-mswmdm-iwmdmstorage3-setenumpreference).

## <a name="syntax"></a>Синтаксис


```C++
typedef enum tagWMDM_STORAGE_ENUM_MODE { 
  ENUM_MODE_RAW,
  ENUM_MODE_USE_DEVICE_PREF,
  ENUM_MODE_METADATA_VIEWS
} WMDM_STORAGE_ENUM_MODE;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="ENUM_MODE_RAW"></span><span id="enum_mode_raw"></span>**\_режим перечисления \_ RAW**
</dt> <dd>

Перечисляет содержимое в хранилище так же, как оно организовано в файловой системе хранилища.

**\_режим перечисления \_ использование \_ \_ префа устройства**

Перечисляет содержимое хранилища на основе настроек устройства, как указано в параметре устройства *усеметадатавиевс* .

**\_ \_ представления метаданных в режиме перечисления \_**

Перечисляет содержимое в хранилище, организуя содержимое на основе представления метаданных.

</dd> <dt>

<span id="ENUM_MODE_USE_DEVICE_PREF"></span><span id="enum_mode_use_device_pref"></span>**\_режим перечисления \_ использование \_ \_ префа устройства**
</dt> <dd>

Перечисляет содержимое хранилища на основе настроек устройства, как указано в параметре устройства *усеметадатавиевс* .

**\_ \_ представления метаданных в режиме перечисления \_**

Перечисляет содержимое в хранилище, организуя содержимое на основе представления метаданных.

</dd> <dt>

<span id="ENUM_MODE_METADATA_VIEWS"></span><span id="enum_mode_metadata_views"></span>**\_ \_ представления метаданных в режиме перечисления \_**
</dt> <dd>

Перечисляет содержимое в хранилище, организуя содержимое на основе представления метаданных.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|-------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Вмдм. idl</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Типы перечислений**](enumeration-types.md)
</dt> </dl>

 

 





