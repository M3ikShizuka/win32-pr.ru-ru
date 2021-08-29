---
description: Этот метод возвращает интерфейс, предоставляющий доступ к звуковым данным.
ms.assetid: 4FA7CC9D-D379-4C08-8D4F-5301ECCDF372
title: 'Метод Иаудиофраменативе:: GetData'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAudioFrameNative.GetData
api_type:
- COM
api_location:
- windows.media.core.interop.h
ms.openlocfilehash: 3d845cef0a4a9f6ee9d19b35705b20bd7e6bf2862a84ce4118acb92a5c66f37d
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119642124"
---
# <a name="iaudioframenativegetdata-method"></a>Метод Иаудиофраменативе:: GetData

Этот метод возвращает интерфейс, предоставляющий доступ к звуковым данным.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetData(
  [in]  REFIID riid,
  [out] LPVOID *ppv
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*riid* \[ окне\]
</dt> <dd>

Тип: **рефиид**

IID получаемого интерфейса.

</dd> <dt>

*ППВ* \[ заполняет\]
</dt> <dd>

Тип: **лпвоид \***

При успешном возврате этого метода содержит указатель интерфейса, запрошенный в параметре *riid* .

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **[ **HRESULT**](https://msdn.microsoft.com/library/Bb401631(v=MSDN.10).aspx)**

Возвращает \_ ОК при успешном завершении. Возвращает E \_ Interface, если не удается найти запрошенный интерфейс.

## <a name="see-also"></a>См. также

<dl> <dt>

[**иаудиофраменативе**](/windows/desktop/api/windows.media.core.interop/nn-windows-media-core-interop-iaudioframenative)
</dt> </dl>

 

 



