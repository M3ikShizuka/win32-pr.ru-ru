---
title: Сообщение WM_CAP_GET_AUDIOFORMAT (VFW. h)
description: Сообщение о \_ получении крепления WM \_ \_ аудиоформат получает звуковой формат или размер звукового формата. Это сообщение можно отправить явно или с помощью макросов Капжетаудиоформат и Капжетаудиоформатсизе.
ms.assetid: 25e58863-2b1e-4ed8-9f34-c39617a15bc1
keywords:
- сообщение WM_CAP_GET_AUDIOFORMAT Windows мультимедиа
topic_type:
- apiref
api_name:
- WM_CAP_GET_AUDIOFORMAT
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f9508972c173c9e189bdc092a63d849adf3be739
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124371445"
---
# <a name="wm_cap_get_audioformat-message"></a>\_Сообщение о \_ получении крепления WM \_ аудиоформат

Сообщение **о \_ получении крепления WM \_ \_ аудиоформат** получает звуковой формат или размер звукового формата. Это сообщение можно отправить явно или с помощью макросов [**капжетаудиоформат**](/windows/desktop/api/Vfw/nf-vfw-capgetaudioformat) и [**капжетаудиоформатсизе**](/windows/desktop/api/Vfw/nf-vfw-capgetaudioformatsize) .


```C++
WM_CAP_GET_AUDIOFORMAT 
wParam = (WPARAM) (wSize); 
lParam = (LPARAM) (LPVOID) (LPWAVEFORMATEX) (psAudioFormat); 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="wSize"></span><span id="wsize"></span><span id="WSIZE"></span>*всизе*
</dt> <dd>

Размер (в байтах) структуры, на которую ссылается **s**.

</dd> <dt>

<span id="psAudioFormat"></span><span id="psaudioformat"></span><span id="PSAUDIOFORMAT"></span>*псаудиоформат*
</dt> <dd>

Указатель на структуру [**вавеформатекс**](/windows/win32/api/mmeapi/ns-mmeapi-waveformatex) или **значение NULL**. Если значение равно **null**, возвращается размер (в байтах), необходимый для хранения структуры.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает размер звукового формата в байтах.

## <a name="remarks"></a>Remarks

Так как сжатые аудио форматы зависят от требований к размеру, приложения должны сначала получить размер, затем выделить память и, наконец, запросить данные в звуковом формате.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Видеозапись](video-capture.md)
</dt> <dt>

[Сообщения видеозаписи](video-capture-messages.md)
</dt> </dl>

 

