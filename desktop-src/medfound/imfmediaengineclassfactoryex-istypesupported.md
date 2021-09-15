---
description: Возвращает значение, указывающее, поддерживает ли указанная система ключей указанный тип носителя.
ms.assetid: 6f4f50db-e491-46c2-a8b2-1b8e51033b5b
title: 'Метод Имфмедиаенгинеклассфакторекс:: Истипесуппортед'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IMFMediaEngineClassFactoryEx.IsTypeSupported
api_type:
- COM
api_location:
- mfmediaengine.h
ms.openlocfilehash: 92bf3d64d36c043e9e33b897294ff74a3fda0445
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460999"
---
# <a name="imfmediaengineclassfactoryexistypesupported-method"></a>Метод Имфмедиаенгинеклассфакторекс:: Истипесуппортед

Возвращает значение, указывающее, поддерживает ли указанная система ключей указанный тип носителя.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT IsTypeSupported(
   BSTR type,
   BSTR keySystem,
   BOOL *isSupported
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*type* 
</dt> <dd>

Тип MIME для проверки поддержки.

</dd> <dt>

*кэйсистем* 
</dt> <dd>

Основная система для проверки поддержки.

</dd> <dt>

*isSupported* 
</dt> <dd>

**значение true** , если тип поддерживается *кэйсистем*; в противном случае — **значение false.**

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8.1 \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Windows Server 2012 \[Только классические приложения R2\]<br/>                                      |
| IDL<br/>                      | <dl> <dt>Мфмедиаенгине. idl</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**имфмедиаенгинеклассфакторекс**](/windows/desktop/api/mfmediaengine/nn-mfmediaengine-imfmediaengineclassfactoryex)
</dt> </dl>

 

 




