---
title: Сообщение ICM_COMPRESS_GET_FORMAT (VFW. h)
description: Сообщение ICM \_ \_ Get \_ Format запрашивает выходной формат сжатых данных из драйвера сжатия видео. Это сообщение можно отправить явно или с помощью макроса Иккомпрессжетформат.
ms.assetid: ac12d415-bad5-4838-b206-09c8097d3fd9
keywords:
- сообщение ICM_COMPRESS_GET_FORMAT Windows мультимедиа
topic_type:
- apiref
api_name:
- ICM_COMPRESS_GET_FORMAT
api_location:
- Vfw.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: d096ceafa382bdbae5e4efe16975b3518735e773
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124370425"
---
# <a name="icm_compress_get_format-message"></a>ICM \_ сжимать \_ Получение \_ формата сообщения

Сообщение **ICM \_ \_ Get \_ Format** запрашивает выходной формат сжатых данных из драйвера сжатия видео. Это сообщение можно отправить явно или с помощью макроса [**иккомпрессжетформат**](/windows/desktop/api/Vfw/nf-vfw-iccompressgetformat) .


```C++
ICM_COMPRESS_GET_FORMAT 
wParam = (DWORD_PTR) (LPVOID) lpbiInput; 
lParam = (DWORD_PTR) (LPVOID) lpbiOutput; 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="lpbiInput"></span><span id="lpbiinput"></span><span id="LPBIINPUT"></span>*лпбиинпут*
</dt> <dd>

Указатель на структуру [**битмапинфо**](/windows/win32/api/wingdi/ns-wingdi-bitmapinfo) , содержащую входной формат.

</dd> <dt>

<span id="lpbiOutput"></span><span id="lpbioutput"></span><span id="LPBIOUTPUT"></span>*лпбиаутпут*
</dt> <dd>

Указатель на структуру [**битмапинфо**](/windows/win32/api/wingdi/ns-wingdi-bitmapinfo) , в которой будет содержаться выходной формат. Для этого параметра можно указать ноль, чтобы запросить только размер выходного формата, как в макросе [**иккомпрессжетформатсизе**](/windows/desktop/api/Vfw/nf-vfw-iccompressgetformatsize) .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если *лпбиаутпут* равен нулю, возвращает размер структуры.

Если *лпбиаутпут* имеет ненулевое значение, функция ВОЗВРАЩАЕТ значение ицерр \_ ОК в случае успеха или ошибку в противном случае.

## <a name="remarks"></a>Remarks

Если *лпбиаутпут* имеет ненулевое значение, драйвер должен заполнить структуру [**битмапинфо**](/windows/win32/api/wingdi/ns-wingdi-bitmapinfo) с выходным форматом по умолчанию, соответствующим формату входных данных, указанному для *лпбиинпут*. Если программа сжатия может создать несколько форматов, то форматом по умолчанию должен быть тот, который сохраняет максимальный объем информации.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                       |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>VFW. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Диспетчер сжатия видео](video-compression-manager.md)
</dt> <dt>

[Сообщения о сжатии видео](video-compression-messages.md)
</dt> </dl>

 

