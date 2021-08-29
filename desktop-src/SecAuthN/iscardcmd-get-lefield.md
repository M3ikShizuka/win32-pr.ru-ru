---
description: Возвращает поле Le блока данных протокола приложения (КАТЕГОРИЯХ APDU).
ms.assetid: 249e8105-273b-42f0-9427-9b3cda5bf0a1
title: 'Метод Искардкмд:: get_LeField (Скарддат. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ISCardCmd.get_LeField
api_type:
- COM
api_location:
- Scardssp.dll
ms.openlocfilehash: a2a6ad8647f5c3cb579c69b7e54418599853d0bfa777b48ef734974073c8233a
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119577604"
---
# <a name="iscardcmdget_lefield-method"></a>Метод Искардкмд:: Get \_ лефиелд

\[Метод **Get \_ лефиелд** доступен для использования в операционных системах, указанных в разделе требования. он недоступен для использования в Windows Server 2003 с пакетом обновления 1 (SP1) и более поздних версий, Windows Vista, Windows Server 2008 и последующих версиях операционной системы. [Модули смарт-карт](/previous-versions/windows/desktop/secsmart/smart-card-modules) предоставляют аналогичные функции.\]

Метод **Get \_ лефиелд** возвращает поле Le [*блока данных протокола приложения*](../secgloss/a-gly.md) (категориях APDU).

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_LeField(
  [out] LONG *plSize
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*плсизе* \[ заполняет\]
</dt> <dd>

Указатель на значение поля Le при возврате.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Метод возвращает одно из следующих возможных значений.



| Код возврата                                                                                  | Описание                                      |
|----------------------------------------------------------------------------------------------|--------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>         | Операция успешно завершена.<br/> |
| <dl> <dt>**E \_ INVALIDARG**</dt> </dl> | Недопустимый параметр *плсизе* .<br/>  |



 

## <a name="examples"></a>Примеры

В следующем примере показано, как получить значение поля Le из [*блока данных протокола приложения*](../secgloss/a-gly.md) (категориях APDU). В примере предполагается, что Пискардкмд является допустимым указателем на экземпляр интерфейса [**искардкмд**](iscardcmd.md) .


```C++
LONG     lLe;
HRESULT  hr;

// Retrieve the Le field value.
hr = pISCardCmd->get_LeField(&lLe);
if (FAILED(hr))
{
    printf("Failed get_LeField\n");
    // Take other error handling action.
}
else
    printf("Le field value returned is %d\n", lLe);
```



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                    |
| Окончание поддержки клиента<br/>    | Windows XP<br/>                                                                   |
| Поддержка конца сервера<br/>    | Windows Server 2003<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Скарддат. h</dt> </dl>   |
| Библиотека типов<br/>             | <dl> <dt>Скарддат. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Scardssp.dll</dt> </dl> |
| IID<br/>                      | IID \_ искардкмд определен как D5778AE3-43DE-11D0-9171-00AA00C18068<br/>            |



## <a name="see-also"></a>См. также

<dl> <dt>

[**искардкмд**](iscardcmd.md)
</dt> </dl>

 

 
