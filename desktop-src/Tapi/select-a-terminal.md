---
description: В следующем примере кода показано, как выбрать терминалы на потоках, связанных с вызовом.
ms.assetid: ff43e81c-ff39-466d-870a-54b75c2938a4
title: Выберите терминал
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b77ee3bb889f5372ae024b29867b6c9d418c5924b4e626be70aa5d49ad72c9c9
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119991844"
---
# <a name="select-a-terminal"></a>Выберите терминал

В следующем примере кода показано, как выбрать терминалы на потоках, связанных с вызовом.

Перед использованием этого примера кода необходимо выполнить операции в оснастке [инициализации TAPI](initialize-tapi.md) и [выбрать адрес](select-an-address.md).

Кроме того, в этом примере требуется, чтобы приложение уже имело указатель на интерфейс [**итбасиккаллконтрол**](/windows/desktop/api/tapi3if/nn-tapi3if-itbasiccallcontrol) входящего или исходящего вызова. Чтобы получить этот указатель, см. статью [выполнение вызова](make-a-call.md) или [получение вызова](receive-a-call.md) для примеров кода.

> [!Note]  
> В этом примере отсутствует проверка ошибок и выпуски, соответствующие рабочему коду.

 

``` syntax
// pAddress is an ITAddress interface pointer.
// pBasicCall is an ITBasicCallControl interface pointer.

// Get the ITStreamControl interface.
ITStreamControl * pStreamControl;
HRESULT hr = pBasicCall->QueryInterface(
        IID_ITStreamControl,
        (void **) &pStreamControl
        );
// If ( hr != S_OK ) process the error here. 

// Enumerate the streams and select 
// terminals onto them.
IEnumStream * pEnumStreams;
ITStream    * pStream;
hr = pStreamControl->EnumerateStreams(&pEnumStreams);
// If ( hr != S_OK ) process the error here. 

while ( S_OK == pEnumStreams->Next(1, &pStream, NULL) )
{
    // Get the media type and direction of this stream.
    long                lMediaType;
    TERMINAL_DIRECTION  dir;
    hr = pStream->get_MediaType( &lMediaType );
    // If ( hr != S_OK ) process the error here. 
    hr = pStream->get_Direction( &dir );
    // If ( hr != S_OK ) process the error here. 

    // Create the default terminal for this media type and direction.
    //   If lMediaType == TAPIMEDIATYPE_VIDEO and
    //   dir == TD_RENDER, a dynamic video render terminal
    //   is required. Please see Incoming.cpp in 
    //   the samples section of the SDK. 
    // For all other terminals, get the default static terminal.
    ITTerminal * pTerminal;
    ITTerminalSupport * pTerminalSupport;
    hr = pAddress->QueryInterface( 
            IID_ITTerminalSupport, 
            (void **)&pTerminalSupport
         );
    // If ( hr != S_OK ) process the error here. 
    hr = pTerminalSupport->GetDefaultStaticTerminal(
            lMediaType,
            dir,
            pTerminal
         );
    // If ( hr != S_OK ) process the error here. 
    // Select the terminal on the stream.
    hr = pStream->SelectTerminal(pTerminal);
    // If ( hr != S_OK ) process the error here. 
}
```

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**итаддресс**](/windows/desktop/api/tapi3if/nn-tapi3if-itaddress)
</dt> <dt>

[**итбасиккаллконтрол**](/windows/desktop/api/tapi3if/nn-tapi3if-itbasiccallcontrol)
</dt> <dt>

[**итстреамконтрол**](/windows/win32/api/tapi3if/nn-tapi3if-itstreamcontrol)
</dt> <dt>

[**итстреам**](/windows/win32/api/tapi3if/nn-tapi3if-itstream)
</dt> <dt>

[**иенумстреам**](/windows/desktop/api/tapi3if/nn-tapi3if-ienumstream)
</dt> <dt>

[**иттерминал**](/windows/win32/api/tapi3if/nn-tapi3if-itterminal)
</dt> <dt>

[**иттерминалсуппорт**](/windows/win32/api/tapi3if/nn-tapi3if-itterminalsupport)
</dt> </dl>

 

 
