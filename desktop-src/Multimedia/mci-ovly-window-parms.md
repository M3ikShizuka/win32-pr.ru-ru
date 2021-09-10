---
title: Структура MCI_OVLY_WINDOW_PARMS (МЦиапи. h)
description: '\_ \_ Структура ПАРМС окна MCI овли \_ содержит отображаемую информацию для \_ команды окна MCI для устройств наложения видео.'
ms.assetid: 1189f31e-6e54-4279-a23d-b4e21c6cd276
keywords:
- структура MCI_OVLY_WINDOW_PARMS Windows мультимедиа
topic_type:
- apiref
api_name:
- MCI_OVLY_WINDOW_PARMS
api_location:
- mciapi.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a554c9ed4e4869eab333b93736a0400ef93053cc
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370071"
---
# <a name="mci_ovly_window_parms-structure"></a>\_ \_ Структура ПАРМС окна MCI овли \_

Структура **\_ \_ \_ пармс окна MCI овли** содержит отображаемую информацию для команды [**\_ окна MCI**](mci-window.md) для устройств наложения видео.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct {
  DWORD_PTR dwCallback;
  HWND      hWnd;
  UINT      nCmdShow;
  LPCTSTR   lpstrText;
} MCI_OVLY_WINDOW_PARMS;
```



## <a name="members"></a>Участники

<dl> <dt>

**двкаллбакк**
</dt> <dd>

Слово нижнего порядка задает маркер окна, используемый для \_ флага уведомления MCI.

</dd> <dt>

**hWnd**
</dt> <dd>

Маркер для отображаемого окна.

</dd> <dt>

**нкмдшов**
</dt> <dd>

Команда для вывода окна.

</dd> <dt>

**лпстртекст**
</dt> <dd>

Заголовок окна.

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

[**\_окно MCI**](mci-window.md)
</dt> <dt>

[**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85))
</dt> </dl>

 

