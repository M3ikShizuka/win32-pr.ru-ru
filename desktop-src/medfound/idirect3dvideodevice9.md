---
description: Включает аппаратное ускорение декодирования устройства Direct3D 9 с помощью ускорения видео DirectX (ДКСВА) версии 1,0.
ms.assetid: abe3beac-f3f8-413d-8b83-9da3340b19ac
title: Интерфейс IDirect3DVideoDevice9 (Дксва. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IDirect3DVideoDevice9
api_type:
- COM
api_location:
- dxva.h
ms.openlocfilehash: 89afef6f39b3aa196d8b1013e3d8873e329ce6ef
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570626"
---
# <a name="idirect3dvideodevice9-interface"></a>Интерфейс IDirect3DVideoDevice9

Включает аппаратное ускорение декодирования устройства Direct3D 9 с помощью ускорения видео DirectX (ДКСВА) версии 1,0.

## <a name="when-to-use"></a>Назначение

Этот интерфейс не предназначен для общего использования приложением. DirectShow фильтры декодера должны использовать интерфейс [**иамвидеоакцелератор**](/previous-versions/windows/desktop/api/videoacc/nn-videoacc-iamvideoaccelerator) , а не **IDirect3DVideoDevice9**. входные контакты фильтра "микширование видео" (VMR) и Mixerного фильтра раскрывают **иамвидеоакцелератор**.

## <a name="members"></a>Элементы

Интерфейс **IDirect3DVideoDevice9** наследует от интерфейса [**IUnknown**](/windows/win32/api/unknwn/nn-unknwn-iunknown) . **IDirect3DVideoDevice9** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **IDirect3DVideoDevice9** содержит следующие методы.



| Метод                                                                                   | Описание                                                                                                                       |
|:-----------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------|
| [**креатедксвадевице**](idirect3dvideodevice9-createdxvadevice.md)                       | Создает устройство декодера ДКСВА.<br/>                                                                                         |
| [**креатесурфаце**](idirect3dvideodevice9-createsurface.md)                             | Создает сжатую поверхность для декодирования ДКСВА.<br/>                                                                        |
| [**жетдксвакомпресседбуфферинфо**](idirect3dvideodevice9-getdxvacompressedbufferinfo.md) | Возвращает сведения о сжатых буферах, необходимых для декодирования с аппаратным ускорением.<br/>                                |
| [**жетдксвагуидс**](idirect3dvideodevice9-getdxvaguids.md)                               | Возвращает список профилей ДКСВА, поддерживаемых драйвером экрана.<br/>                                             |
| [**жетдксваинтерналинфо**](idirect3dvideodevice9-getdxvainternalinfo.md)                 | Запрашивает объем вспомогательной памяти, выделяемой слоем абстрагирования оборудования (HAL) для частного использования. <br/> |
| [**жетункомпресседдксваформатс**](idirect3dvideodevice9-getuncompresseddxvaformats.md)   | Возвращает список несжатых форматов пикселей, которые могут быть отображены с помощью указанного профиля ДКСВА.<br/>                         |



 

## <a name="remarks"></a>Remarks

Чтобы получить указатель на этот интерфейс, вызовите метод **QueryInterface** для указателя [**IDirect3DDevice9**](/windows/win32/api/d3d9helper/nn-d3d9helper-idirect3ddevice9) или [**IDirect3DDevice9Ex**](/windows/win32/api/d3d9/nn-d3d9-idirect3ddevice9ex) .

Этот интерфейс поддерживает только ДКСВА 1,0. Он не поддерживает ДКСВА 2,0.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                    |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                              |
| Заголовок<br/>                   | <dl> <dt>Дксва. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Интерфейсы видео Direct3D](direct3d-video-interfaces.md)
</dt> <dt>

[Ускорение видео DirectX 2,0](directx-video-acceleration-2-0.md)
</dt> <dt>

[Спецификация ДКСВА 1,0](/windows-hardware/drivers/display/directx-video-acceleration)
</dt> </dl>

 

 
