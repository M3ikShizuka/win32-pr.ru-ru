---
description: Извлекает текущее состояние смарт-карты.
ms.assetid: 0e6e4a8f-ecad-4a82-8804-aaf58f13f7ca
title: Метод get_Status. h.
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ISCard.get_Status
api_type:
- COM
api_location:
- Scardssp.dll
ms.openlocfilehash: f0daa47653779b3aa4b5e7cb65c0c56410b19ab9
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064720"
---
# <a name="iscardget_status-method"></a>Метод карточки:: Get \_ status

\[Метод **Get \_ Status** доступен для использования в операционных системах, указанных в разделе требования. он недоступен для использования в Windows Server 2003 с пакетом обновления 1 (SP1) и более поздних версий, Windows Vista, Windows Server 2008 и последующих версиях операционной системы. [Модули смарт-карт](/previous-versions/windows/desktop/secsmart/smart-card-modules) предоставляют аналогичные функции.\]

Метод **Get \_ Status** извлекает текущее [*состояние*](../secgloss/s-gly.md) [*смарт-карты*](../secgloss/s-gly.md).

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_Status(
  [out] SCARD_STATES *pStatus
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пстатус* \[ заполняет\]
</dt> <dd>

Указатель на переменную состояния.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Метод возвращает одно из следующих возможных значений.



| Код возврата                                                                                  | Описание                                       |
|----------------------------------------------------------------------------------------------|---------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>         | Operation completed successfully (Операция выполнена успешно).<br/>      |
| <dl> <dt>**E \_ INVALIDARG**</dt> </dl> | Недопустимый параметр *пстатус* .<br/>  |
| <dl> <dt>**\_указатель E**</dt> </dl>    | В *пстатус* был передан неверный указатель.<br/> |



 

## <a name="remarks"></a>Remarks

Кроме приведенных выше кодов ошибок COM, этот интерфейс может возвращать код ошибки смарт-карты, если для завершения запроса была вызвана функция смарт-карты. Дополнительные сведения см. в статье [возвращаемые значения смарт-карты](authentication-return-values.md).

## <a name="examples"></a>Примеры

В следующем примере показано получение текущего состояния смарт-карты.


```C++
SCARD_STATES    scState;
HRESULT         hr;

// Determine the current state of the smart card.
hr = pISCard->get_Status(&scState);
if (FAILED(hr))
{
   printf("Failed get_Status\n");
   exit(1);  // Or other error handling action.
}
// Use the retrieved value. (This example merely displays it.)
switch (scState)
{
    case ABSENT:
        printf("Absent state\n");
        break;
    case PRESENT:
        printf("Present state\n");
        break;
    case SWALLOWED:
        printf("Swallowed state\n");
        break;
    case POWERED:
        printf("Powered state\n");
        break;
    case NEGOTIABLEMODE:
        printf("Negotiable mode state\n");
        break;
    case SPECIFICMODE:
        printf("Specific mode state\n");
        break;
    default:
        printf("Unexpected state\n");
        break;
}
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                    |
| Окончание поддержки клиента<br/>    | Windows XP<br/>                                                                   |
| Поддержка конца сервера<br/>    | Windows Server 2003<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Скардмгр. h</dt> </dl>   |
| Библиотека типов<br/>             | <dl> <dt>Скардмгр. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Scardssp.dll</dt> </dl> |
| IID<br/>                      | Идентификатор IID \_ -карты определен как 1461AAC3-6810-11D0-918F-00AA00C18068<br/>               |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**получение \_ ATR**](iscard-get-atr.md)
</dt> <dt>

[**получить \_ кардхандле**](iscard-get-cardhandle.md)
</dt> <dt>

[**получить \_ контекст**](iscard-get-context.md)
</dt> <dt>

[**получить \_ протокол**](iscard-get-protocol.md)
</dt> <dt>

[**Карточка**](iscard.md)
</dt> </dl>

 

 
