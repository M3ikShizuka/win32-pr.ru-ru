---
title: Структура MCI_VCR_STEP_PARMS (видеомагнитофон. h)
description: '\_Структура шага пармс видеомагнитофона MCI \_ \_ содержит параметры для \_ команды шага MCI для устройств записи видеокассет.'
ms.assetid: 57751de6-d174-418f-8167-402d3ead4e24
keywords:
- структура MCI_VCR_STEP_PARMS Windows мультимедиа
topic_type:
- apiref
api_name:
- MCI_VCR_STEP_PARMS
api_location:
- Vcr.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a616b31500a2c814edb3dd443586131ed0ffae7d
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370170"
---
# <a name="mci_vcr_step_parms-structure"></a>\_ \_ Пармсная структура шага видеомагнитофона MCI \_

Структура **\_ \_ шага \_ Пармс видеомагнитофона MCI** содержит параметры для [**команды \_ шага MCI**](mci-step.md) для устройств записи видеокассет.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct tagMCI_VCR_STEP_PARMS {
  DWORD_PTR dwCallback;
  DWORD     dwFrames;
} MCI_VCR_STEP_PARMS;
```



## <a name="members"></a>Участники

<dl> <dt>

**двкаллбакк**
</dt> <dd>

Слово нижнего порядка задает маркер окна, используемый для \_ флага уведомления MCI.

</dd> <dt>

**двфрамес**
</dt> <dd>

Число кадров для перехода (длина одного шага) по мере выполнения командой [**\_ шага MCI**](mci-step.md) шага вперед или назад по содержимому.

</dd> </dl>

## <a name="remarks"></a>Remarks

При назначении данных элементам этой структуры установите соответствующие флаги в параметре *Фдвкомманд* [**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85)) , чтобы проверить элементы.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>Видеомагнитофон. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**MCI**](mci.md)
</dt> <dt>

[**Структуры MCI**](mci-structures.md)
</dt> <dt>

[**\_шаг MCI**](mci-step.md)
</dt> <dt>

[**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85))
</dt> </dl>

 

