---
description: Возобновляет процессы пакета, если они в данный момент приостановлены.
ms.assetid: c5376e00-b4b7-4a81-a84c-3a46758fe130
title: 'Метод Ипаккажедебугсеттингс:: Resume'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IPackageDebugSettings.Resume
api_type:
- COM
api_location:
- Shobjidl.idl
ms.openlocfilehash: 6871aea0fc18ce64939fa1bba06946f8a3a1c260e341b1dfa500a71f273a883b
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120121584"
---
# <a name="ipackagedebugsettingsresume-method"></a>Метод Ипаккажедебугсеттингс:: Resume

Возобновляет процессы пакета, если они в данный момент приостановлены.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT Resume(
  [in] LPCWSTR packageFullName
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*полноеимяпакета* \[ окне\]
</dt> <dd>

Тип: **лпквстр**

Полное имя пакета.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Тип: **HRESULT**

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

Каждый процесс получает событие [**возобновления**](/uwp/api/Windows.ApplicationModel.Core.CoreApplication?view=winrt-19041) . Он может быть полезен разработчикам для пошагового указания того, как приложения реагируют на это событие.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8<br/>                                                                    |
| Минимальная версия сервера<br/> | Windows Server 2012<br/>                                                          |
| IDL<br/>                      | <dl> <dt>Shobjidl. idl</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**ипаккажедебугсеттингс**](/previous-versions//hh438393(v=vs.85))
</dt> </dl>

 

 
