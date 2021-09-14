---
title: Перечисление Клиентспек
description: Используется со свойством Клиентпротоколспек для указания протокола удаленного рабочего стола, используемого между клиентом и сервером.
ms.assetid: BFB2CD3C-04BF-4CB3-B156-8B08AE697327
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов перечисления Клиентспек
topic_type:
- apiref
api_name:
- ClientSpec
api_location:
- MsTscAx.dll
api_type:
- LibDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1f52fbdbaa37c392de727dd2640580800d813d51
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126891261"
---
# <a name="clientspec-enumeration"></a>Перечисление Клиентспек

Используется со свойством [**клиентпротоколспек**](imsrdpclientadvancedsettings8-clientprotocolspec.md) для указания протокола удаленного рабочего стола, используемого между клиентом и сервером.

## <a name="syntax"></a>Синтаксис


```C++
typedef enum  { 
  FullMode        = 0,
  ThinClientMode,
  SmallCacheMode
} ClientSpec;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="FullMode"></span><span id="fullmode"></span><span id="FULLMODE"></span>**фуллмоде**
</dt> <dd>

протокол полностью Windows 8 удаленный рабочий стол протокол.

</dd> <dt>

<span id="ThinClientMode"></span><span id="thinclientmode"></span><span id="THINCLIENTMODE"></span>**синклиентмоде**
</dt> <dd>

протокол ограничен использованием Windows 7 с пакетом обновления 1 (SP1) RemoteFX кодеком и небольшим кэшем. Все остальные кодеки отключены. Этот протокол имеет наименьший объем памяти.

</dd> <dt>

<span id="SmallCacheMode"></span><span id="smallcachemode"></span><span id="SMALLCACHEMODE"></span>**смаллкачемоде**
</dt> <dd>

Протокол аналогичен **фуллмоде**, за исключением того, что он использует меньший кэш.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8<br/>                                                                   |
| Минимальная версия сервера<br/> | Windows Server 2012<br/>                                                         |
| Библиотека типов<br/>             | <dl> <dt>MsTscAx.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**IMsRdpClientAdvancedSettings8:: Клиентпротоколспек**](imsrdpclientadvancedsettings8-clientprotocolspec.md)
</dt> </dl>

 

 





