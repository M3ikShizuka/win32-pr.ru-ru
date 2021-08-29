---
title: Свойство IMsRdpCameraRedirConfig FriendlyName
description: Возвращает понятное имя камеры.
ms.tgt_platform: multiple
keywords:
- Свойство FriendlyName службы удаленных рабочих столов
- Свойство FriendlyName службы удаленных рабочих столов, интерфейс Имсрдпкамераредирконфиг
- Службы удаленных рабочих столов интерфейса Имсрдпкамераредирконфиг, свойство FriendlyName
topic_type:
- apiref
api_name:
- IMsRdpCameraRedirConfig.FriendlyName
- IMsRdpCameraRedirConfig.get_FriendlyName
api_location:
- MsTscAx.dll
api_type:
- COM
ms.topic: reference
ms.date: 12/16/2020
ms.openlocfilehash: 31d6d775310d23cfe8a9cf8ab95ea56e9e2b2d0e418fc9d1a55d3cf26fcce26e
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119737414"
---
# <a name="imsrdpcameraredirconfigfriendlyname-property"></a>Свойство Имсрдпкамераредирконфиг:: FriendlyName

Возвращает понятное имя камеры.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис

```C++
HRESULT get_FriendlyName(
    [out, retval] BSTR* pFriendlyName
);
```

## <a name="property-value"></a>Значение свойства

Понятное имя камеры.

## <a name="requirements"></a>Требования

| Требование | Значение |
|-------------------------------------|---------------------------------------|
| Минимальная версия клиента| Windows 10, версия 1803 (сборка 17134)      |
| Библиотека типов            | MsTscAx.dll                        |
| DLL                  | MsTscAx.dll     |
| IID                      | IID \_ имсрдпкамераредирконфиг определен как 09750604-D625-47C1-9FCD-F09F735705D7            |

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**IMsRdpCameraRedirConfig**](imsrdpcameraredirconfig.md)
</dt> </dl>