---
title: Структура MCI_STATUS_PARMS (МЦиапи. h)
description: '\_ \_ Структура ПАРМС состояния MCI содержит сведения о \_ команде состояния MCI.'
ms.assetid: c4897b34-4184-46aa-af17-2127edfbf82d
keywords:
- структура MCI_STATUS_PARMS Windows мультимедиа
topic_type:
- apiref
api_name:
- MCI_STATUS_PARMS
api_location:
- mciapi.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8295f2e747752889c10083c6bb794ba2df7ac273
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370125"
---
# <a name="mci_status_parms-structure"></a>\_ \_ Структура ПАРМС состояния MCI

Структура **\_ \_ пармс состояния MCI** содержит сведения о команде [**\_ состояния MCI**](mci-status.md) .

## <a name="syntax"></a>Синтаксис


```C++
typedef struct {
  DWORD_PTR dwCallback;
  DWORD_PTR dwReturn;
  DWORD     dwItem;
  DWORD     dwTrack;
} MCI_STATUS_PARMS;
```



## <a name="members"></a>Участники

<dl> <dt>

**двкаллбакк**
</dt> <dd>

Слово нижнего порядка задает маркер окна, используемый для \_ флага уведомления MCI.

</dd> <dt>

**двретурн**
</dt> <dd>

Содержит сведения о возврате.

</dd> <dt>

**двитем**
</dt> <dd>

Запрашиваемая возможность.

</dd> <dt>

**двтракк**
</dt> <dd>

Длина или число дорожек.

</dd> </dl>

## <a name="remarks"></a>Remarks

\_ \_ Флаг элемента состояния MCI должен быть задан в параметре *фдвкомманд* функции [**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85)) для проверки элемента **двитем** , который должен содержать одну из констант, указывающих, какие сведения о состоянии запрашиваются.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>МЦиапи. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**MCI**](mci.md)
</dt> <dt>

[**Структуры MCI**](mci-structures.md)
</dt> <dt>

[**\_состояние MCI**](mci-status.md)
</dt> <dt>

[**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85))
</dt> </dl>

 

