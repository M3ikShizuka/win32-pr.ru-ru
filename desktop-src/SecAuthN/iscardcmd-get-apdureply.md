---
description: Извлекает ответ КАТЕГОРИЯХ APDU, помещая его в конкретный буфер байтов.
ms.assetid: ab349e7a-350f-4e72-98b4-4c6431b6e380
title: 'Метод Искардкмд:: get_ApduReply (Скарддат. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ISCardCmd.get_ApduReply
api_type:
- COM
api_location:
- Scardssp.dll
ms.openlocfilehash: b5732d956e28c89ef3fba6d5beeea7077468c9e9154a48e4ffb327a36280d11f
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120015064"
---
# <a name="iscardcmdget_apdureply-method"></a>Метод Искардкмд:: Get \_ апдурепли

\[Метод **Get \_ апдурепли** доступен для использования в операционных системах, указанных в разделе требования. он недоступен для использования в Windows Server 2003 с пакетом обновления 1 (SP1) и более поздних версий, Windows Vista, Windows Server 2008 и последующих версиях операционной системы. [Модули смарт-карт](/previous-versions/windows/desktop/secsmart/smart-card-modules) предоставляют аналогичные функции.\]

Метод **Get \_ апдурепли** извлекает [*ответ категориях APDU*](../secgloss/r-gly.md), помещая его в конкретный буфер байтов. Ответ может быть **равен null** , если в команде категориях APDU не выполнялась [*транзакция*](../secgloss/t-gly.md) .

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_ApduReply(
  [out] LPBYTEBUFFER *ppReplyApdu
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппрепляпду* \[ заполняет\]
</dt> <dd>

Указатель на байтовый буфер (сопоставляется через объект **IStream** ), содержащий ответное сообщение категориях APDU при возврате.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Метод возвращает одно из следующих возможных значений.



| Код возврата                                                                                   | Описание                                           |
|-----------------------------------------------------------------------------------------------|-------------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>          | Operation completed successfully (Операция выполнена успешно).<br/>          |
| <dl> <dt>**E \_ INVALIDARG**</dt> </dl>  | Недопустимый параметр *ппрепляпду* .<br/>  |
| <dl> <dt>**\_указатель E**</dt> </dl>     | В *ппрепляпду* был передан неверный указатель.<br/> |
| <dl> <dt>**E \_ OUTOFMEMORY**</dt> </dl> | Недостаточно памяти.<br/>                             |



 

## <a name="remarks"></a>Remarks

Чтобы определить длину ответа КАТЕГОРИЯХ APDU, вызовите [**Get \_ апдуреплиленгс**](iscardcmd-get-apdureplylength.md).

Чтобы задать новый ответ КАТЕГОРИЯХ APDU, вызовите метод Set [**\_ апдурепли**](iscardcmd-put-apdureply.md).

Список всех методов, предоставляемых этим интерфейсом, см. в разделе [**искардкмд**](iscardcmd.md).

Кроме приведенных выше кодов ошибок COM, этот интерфейс может возвращать код ошибки [*смарт-карты*](../secgloss/s-gly.md) , если для завершения запроса была вызвана функция смарт-карты. Дополнительные сведения см. в статье [возвращаемые значения смарт-карты](authentication-return-values.md).

## <a name="examples"></a>Примеры

В следующем примере показано, как получить данные ответа. В примере предполагается, что лле является переменной типа **Long** , значение которой было задано предыдущим вызовом [**метода искардкмд:: Get \_ апдуреплиленгс**](iscardcmd-get-apdureplylength.md) , пибитерепли является допустимым указателем на экземпляр интерфейса [**ибитебуффер**](ibytebuffer.md) , а пискардкмд является допустимым указателем на экземпляр интерфейса [**искардкмд**](iscardcmd.md) .


```C++
HRESULT      hr;

if (lLe > 0)
{
    // Get reply data if available.
    hr = pISCardCmd->get_ApduReply(&pIByteReply);
    if (FAILED(hr)) 
    {
        printf("Failed ISCardCmd::get_ApduReply.\n");
        // Take other error handling action as needed.
    }
    else
    {
        BYTE byReplyBytes[256];
        LONG lBytesRead;

        hr = pIByteReply->Read(byReplyBytes, lLe, &lBytesRead);
        if (FAILED(hr))
        {
            printf("Failed IByteBuffer::Read.\n");
            // Take other error handling action as needed.
        }
        // Use the bytes in byReplyBytes as needed.
    }
}
```



## <a name="requirements"></a>Требования



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

[**получить \_ апдуреплиленгс**](iscardcmd-get-apdureplylength.md)
</dt> <dt>

[**искардкмд**](iscardcmd.md)
</dt> <dt>

[**разместить \_ апдурепли**](iscardcmd-put-apdureply.md)
</dt> </dl>

 

 
