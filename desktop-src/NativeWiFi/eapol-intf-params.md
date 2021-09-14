---
description: Содержит параметры конфигурации EAPOL.
ms.assetid: 4157a643-86f2-4f6f-8517-6207b11ea9a1
title: Структура EAPOL_INTF_PARAMS (Взксапи. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- EAPOL_INTF_PARAMS
api_type:
- HeaderDef
api_location:
- wzcsapi.h
ms.openlocfilehash: dd9e0664fe41b471162beccd31bf2c22fbfa1640
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065068"
---
# <a name="eapol_intf_params-structure"></a>\_ \_ Структура params EAPOL intf

\[**EAPOL \_ \_параметры INTF** больше не поддерживаются в Windows Vista и Windows Server 2008. Вместо этого используйте [собственный интерфейс API Wi-Fi](native-wifi-reference.md), который предоставляет аналогичные функциональные возможности. Дополнительные сведения см. [в статье о встроенном API Wi-Fi](about-the-native-wifi-api.md).\]

Содержит параметры конфигурации EAPOL.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct _EAPOL_INTF_PARAMS {
  DWORD dwVersion;
  DWORD dwReserved2;
  DWORD dwEapFlags;
  DWORD dwEapType;
  DWORD dwSizeOfSSID;
  BYTE  bSSID[MAX_NETWORK_NAME_LENGTH];
} EAPOL_INTF_PARAMS, *PEAPOL_INTF_PARAMS;
```



## <a name="members"></a>Участники

<dl> <dt>

**двверсион**
</dt> <dd>

Версия вызывающего объекта. Значение по умолчанию — 0.

</dd> <dt>

**dwReserved2**
</dt> <dd>

Зарезервировано для последующего использования.

</dd> <dt>

**двеапфлагс**
</dt> <dd>

Не используется.

</dd> <dt>

**двеаптипе**
</dt> <dd>

Используемый тип расширения EAP. Задайте значение 0x00000013 для EAP-TLS и 0x00000026 для PEAP.

</dd> <dt>

**двсизеофссид**
</dt> <dd>

Размер идентификатора сети.

</dd> <dt>

**bSSID**
</dt> <dd>

Идентификатор сети.

</dd> </dl>

## <a name="remarks"></a>Remarks

файл заголовка взксапи. h недоступен в Windows SDK.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP с пакетом обновления 2 (SP2) \[ только классические приложения\]<br/>                                 |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                 |
| Окончание поддержки клиента<br/>    | Windows XP с пакетом обновления SP3<br/>                                                       |
| Поддержка конца сервера<br/>    | Windows Server 2003<br/>                                                       |
| Заголовок<br/>                   | <dl> <dt>Взксапи. h</dt> </dl> |



 

 




