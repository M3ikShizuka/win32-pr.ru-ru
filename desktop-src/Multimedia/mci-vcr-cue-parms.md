---
title: Структура MCI_VCR_CUE_PARMS (видеомагнитофон. h)
description: '\_Структура Cue пармс на магнитофоне MCI \_ \_ содержит параметры для \_ команды MCI CUE для устройств записи видеокассет.'
ms.assetid: b2ac0c43-93ea-41c9-b886-542bda57b59e
keywords:
- структура MCI_VCR_CUE_PARMS Windows мультимедиа
topic_type:
- apiref
api_name:
- MCI_VCR_CUE_PARMS
api_location:
- Vcr.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8eeae20495281640718f95066476f0f3ac89dc6f
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369978"
---
# <a name="mci_vcr_cue_parms-structure"></a>\_ \_ Структура Cue пармс для видеомагнитофона \_ MCI

Структура **\_ \_ Cue \_ Пармс на магнитофоне MCI** содержит параметры для команды [**MCI \_ Cue**](mci-cue.md) для устройств записи видеокассет.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct tagMCI_VCR_CUE_PARMS {
  DWORD_PTR dwCallback;
  DWORD     dwFrom;
  DWORD     dwTo;
} MCI_VCR_CUE_PARMS;
```



## <a name="members"></a>Участники

<dl> <dt>

**двкаллбакк**
</dt> <dd>

Слово нижнего порядка задает маркер окна, используемый для \_ флага уведомления MCI.

</dd> <dt>

**двфром**
</dt> <dd>

Разместить в подсказке.

</dd> <dt>

**двто**
</dt> <dd>

Разместить в подсказке.

</dd> </dl>

## <a name="remarks"></a>Remarks

При назначении данных членам этой структуры установите соответствующие флаги в параметре *фдвкомманд* функции [**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85)) , чтобы проверить элементы.

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

[**\_Подсказка MCI**](mci-cue.md)
</dt> <dt>

[**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85))
</dt> </dl>

 

