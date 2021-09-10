---
title: Структура MCI_VD_ESCAPE_PARMS (МЦиапи. h)
description: '\_ \_ Структура escape-пармс MCI VD \_ содержит команду, отправленную на устройство для \_ управляющей команды MCI для устройств видеодиск.'
ms.assetid: 7c735943-b67a-4be5-82b5-6a058349623e
keywords:
- структура MCI_VD_ESCAPE_PARMS Windows мультимедиа
topic_type:
- apiref
api_name:
- MCI_VD_ESCAPE_PARMS
api_location:
- mciapi.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a80712cd693e2c7ebe290be6b9827c1e051dd86a
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369996"
---
# <a name="mci_vd_escape_parms-structure"></a>\_ \_ Структура пармс escape-VD MCI \_

Структура **\_ Escape- \_ \_ пармс MCI VD** содержит команду, отправленную на устройство для [**\_ управляющей команды MCI**](mci-escape.md) для устройств видеодиск.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct {
  DWORD_PTR dwCallback;
  LPCTSTR   lpstrCommand;
} MCI_VD_ESCAPE_PARMS;
```



## <a name="members"></a>Участники

<dl> <dt>

**двкаллбакк**
</dt> <dd>

Слово нижнего порядка задает маркер окна, используемый для \_ флага уведомления MCI.

</dd> <dt>

**лпстркомманд**
</dt> <dd>

Команда для отправки на устройство.

</dd> </dl>

## <a name="remarks"></a>Remarks

При назначении данных членам этой структуры установите соответствующие флаги в параметре *фдвкомманд* функции [**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85)) , чтобы проверить элементы.

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

[**\_escape-последовательность MCI**](mci-escape.md)
</dt> <dt>

[**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85))
</dt> </dl>

 

