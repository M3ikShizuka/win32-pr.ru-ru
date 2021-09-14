---
title: Структура MCI_GENERIC_PARMS (МЦиапи. h)
description: '\_Общая \_ Структура пармс MCI содержит маркер окна, принимающего сообщения уведомления. Эта структура используется для командных сообщений MCI с пустыми списками параметров.'
ms.assetid: 706e406c-d263-4347-932c-e5f125acfe0f
keywords:
- структура MCI_GENERIC_PARMS Windows мультимедиа
topic_type:
- apiref
api_name:
- MCI_GENERIC_PARMS
api_location:
- mciapi.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: a1f96482ed5ec7e27253f234031cd099600bf1b6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127246034"
---
# <a name="mci_generic_parms-structure"></a>\_Универсальная \_ Структура пармс MCI

**Общая структура \_ \_ пармс MCI** содержит маркер окна, принимающего сообщения уведомления. Эта структура используется для командных сообщений MCI с пустыми списками параметров.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct {
  DWORD_PTR dwCallback;
} MCI_GENERIC_PARMS;
```



## <a name="members"></a>Участники

<dl> <dt>

**двкаллбакк**
</dt> <dd>

Слово нижнего порядка задает маркер окна, используемый для \_ флага уведомления MCI.

</dd> </dl>

## <a name="remarks"></a>Remarks

Пармс и MCI **\_ закрывают \_** структуры **\_ \_ пармс** , идентичные структурам **\_ универсального \_ пармс MCI** .

При назначении данных членам этой структуры установите соответствующие флаги в параметре *фдвкомманд* функции [**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85)) , чтобы проверить элементы.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                          |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>МЦиапи. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**MCI**](mci.md)
</dt> <dt>

[**Структуры MCI**](mci-structures.md)
</dt> <dt>

[**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85))
</dt> </dl>

 

