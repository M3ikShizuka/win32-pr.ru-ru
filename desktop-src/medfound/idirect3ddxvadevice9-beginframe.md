---
description: Начинает обработку для создания декодированного изображения.
ms.assetid: 80471cc6-c66d-49d9-8593-780e41ac39b9
title: 'Метод IDirect3DDXVADevice9:: Бегинфраме (Дксва. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IDirect3DDXVADevice9.BeginFrame
api_type:
- COM
api_location:
- dxva.h
ms.openlocfilehash: 3090d7868316d08fa91f36dffcc938eb31e06a7d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127581066"
---
# <a name="idirect3ddxvadevice9beginframe-method"></a>Метод IDirect3DDXVADevice9:: Бегинфраме

Начинает обработку для создания декодированного изображения.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT BeginFrame(
   IDirect3DSurface9 *pDstSurface,
   DWORD             SizeInputData,
   VOID              *pInputData,
   DWORD             *pSizeOutputData,
   VOID              *pOutputData
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пдстсурфаце* 
</dt> <dd>

Указатель на интерфейс **IDirect3DSurface9** несжатой целевой поверхности.

</dd> <dt>

*сизеинпутдата* 
</dt> <dd>

Размер буфера, заданного параметром *пинпутдата*, в байтах. Значение должно быть равно 2.

</dd> <dt>

*пинпутдата* 
</dt> <dd>

Указатель на буфер, содержащий данные для ускорителя видео. Этот буфер должен содержать индекс кадра (от нуля), указанный в качестве значения **слова** .

</dd> <dt>

*псизеаутпутдата* 
</dt> <dd>

Размер буфера, заданного параметром *паутпутдата*, в байтах. Значение должно быть равно нулю.

</dd> <dt>

*паутпутдата* 
</dt> <dd>

Указатель на буфер, в который может записываться видео-ускоритель. Присвойте этому параметру **значение NULL**.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

Для каждого вызова **бегинфраме** декодер должен выполнить соответствующий вызов [**IDirect3DDXVADevice9:: ендфраме**](idirect3ddxvadevice9-endframe.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                    |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                              |
| Заголовок<br/>                   | <dl> <dt>Дксва. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**IDirect3DDXVADevice9**](idirect3ddxvadevice9.md)
</dt> </dl>

 

 




