---
description: Метод Clear очищает буферы сообщений протокола приложения (КАТЕГОРИЯХ APDU) и ответов КАТЕГОРИЯХ APDU.
ms.assetid: 5fd3ebb9-b492-4668-9dd8-3ffbcfceb12c
title: 'Метод Искардкмд:: Clear (Скарддат. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ISCardCmd.Clear
api_type:
- COM
api_location:
- Scardssp.dll
ms.openlocfilehash: 0701906c38764ed1b4817f40430dde9b48bfb12e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127259699"
---
# <a name="iscardcmdclear-method"></a>Метод Искардкмд:: Clear

\[Метод **clear** доступен для использования в операционных системах, указанных в разделе требования. он недоступен для использования в Windows Server 2003 с пакетом обновления 1 (SP1) и более поздних версий, Windows Vista, Windows Server 2008 и последующих версиях операционной системы. [Модули смарт-карт](/previous-versions/windows/desktop/secsmart/smart-card-modules) предоставляют аналогичные функции.\]

Метод **clear** очищает буферы сообщений [*протокола приложения*](../secgloss/a-gly.md) (КАТЕГОРИЯХ APDU) и [*ответов категориях APDU*](../secgloss/r-gly.md) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Clear();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Метод возвращает одно из следующих возможных значений.



| Код возврата                                                                             | Описание                                  |
|-----------------------------------------------------------------------------------------|----------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>    | Operation completed successfully (Операция выполнена успешно).<br/> |
| <dl> <dt>**S \_ false**</dt> </dl> | Неизвестная ошибка.<br/>                    |



 

## <a name="remarks"></a>Remarks

Чтобы создать команду КАТЕГОРИЯХ APDU, вызовите [**буилдкмд**](iscardcmd-buildcmd.md).

Список всех методов, предоставляемых этим интерфейсом, см. в разделе [**искардкмд**](iscardcmd.md).

Кроме приведенных выше кодов ошибок COM, этот интерфейс может возвращать код ошибки смарт-карты, если для завершения запроса была вызвана функция смарт-карты. Дополнительные сведения см. в статье [возвращаемые значения смарт-карты](authentication-return-values.md).

## <a name="examples"></a>Примеры

В следующем примере показано, как очистить буферы сообщений КАТЕГОРИЯХ APDU и Reply КАТЕГОРИЯХ APDU.


```C++
HRESULT  hr;

hr = pISCardCmd->Clear();
if (FAILED(hr))
{
    printf("Failed ISCardCmd::Clear\n");
    // Take other error handling action as needed.
}
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                    |
| Окончание поддержки клиента<br/>    | Windows XP<br/>                                                                   |
| Поддержка конца сервера<br/>    | Windows Server 2003<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Скарддат. h</dt> </dl>   |
| Библиотека типов<br/>             | <dl> <dt>Скарддат. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Scardssp.dll</dt> </dl> |
| IID<br/>                      | IID \_ искардкмд определен как D5778AE3-43DE-11D0-9171-00AA00C18068<br/>            |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Искардкмд:: Буилдкмд**](iscardcmd-buildcmd.md)
</dt> <dt>

[**искардкмд**](iscardcmd.md)
</dt> </dl>

 

 
