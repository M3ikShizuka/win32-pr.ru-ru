---
description: 'Дополнительные сведения о методе: Имфмедиакэйс:: Shutdown'
ms.assetid: 464b598c-5fa7-40af-83ba-8619fbd84b04
title: 'Метод Имфмедиакэйс:: Shutdown'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IMFMediaKeys.Shutdown
api_type:
- COM
api_location:
- mfmediaengine.h
ms.openlocfilehash: 198eea5af6980828f6a85c9f4680812dbf4dbf0e3dbac2c5181c6347ffbf386e
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120114344"
---
# <a name="imfmediakeysshutdown-method"></a>Метод Имфмедиакэйс:: Shutdown

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Shutdown();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

Перед окончательным выпуском должно быть вызвано **Завершение работы** приложения. В этой точке выпускается ссылка на модуль расшифровки содержимого (CDM) и другие ресурсы. Однако связанные сеансы не освобождаются или не закрываются.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Windows Server 2012 \[Только классические приложения R2\]<br/>                                      |
| IDL<br/>                      | <dl> <dt>Мфмедиаенгине. idl</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**имфмедиакэйс**](/windows/desktop/api/mfmediaengine/nn-mfmediaengine-imfmediakeys)
</dt> </dl>

 

 




