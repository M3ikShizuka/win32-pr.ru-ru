---
description: Отображает пользовательский интерфейс выбора, позволяющий выбрать имя пользователя.
ms.assetid: 0a02d9e5-b2cf-4818-a2e1-89e6019e53d4
title: 'Метод Искрденр:: Селектусернаме'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ISCrdEnr.selectUserName
- SCrdEnr.selectUserName
api_type:
- COM
api_location:
- Scrdenrl.dll
ms.openlocfilehash: 13059775abc8520c39a0ad3dea2d604fc8d65455
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127170976"
---
# <a name="iscrdenrselectusername-method"></a>Метод Искрденр:: Селектусернаме

Метод **селектусернаме** отображает пользовательский интерфейс **выбора** , позволяющий выбрать имя пользователя.

Имя пользователя применяется к пользователю, от имени которого предназначена регистрация сертификата.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT selectUserName(
  [in] DWORD dwFlags
);
```


```VB

SCrdEnr.selectUserName( _
  ByVal dwFlags _
)
```





## <a name="parameters"></a>Параметры

<dl> <dt>

*dwFlags* \[ окне\]
</dt> <dd>

Зарезервировано для последующего использования. Присвойте этому параметру значение 0.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

### <a name="vb"></a>VB

Если метод завершается успешно, метод возвращает значение S \_ ОК.

Если метод завершается с ошибкой, возвращается значение **HRESULT** , указывающее на ошибку. Список распространенных кодов ошибок см. в разделе [Общие значения HRESULT](common-hresult-values.md).

## <a name="remarks"></a>Комментарии

Используйте этот метод, чтобы выбрать имя пользователя. После выбора имени пользователя его значение можно получить, вызвав метод [**искрденр::-username**](iscrdenr-getusername.md) .

Альтернативой использованию интерфейса "Выбор пользователя" является указание пользователя путем вызова метода [**искрденр:: сетусернаме**](iscrdenr-setusername.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                               |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                    |
| DLL<br/>                      | <dl> <dt>Scrdenrl.dll</dt> </dl> |
| IID<br/>                      | IID \_ искрденр определен как 753988a1-1357-436d-9cf5-f089bdd67d64<br/>             |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**искрденр**](iscrdenr.md)
</dt> <dt>

[**Искрденр:: имя пользователя**](iscrdenr-getusername.md)
</dt> <dt>

[**Искрденр:: Ресетусер**](iscrdenr-resetuser.md)
</dt> <dt>

[**Искрденр:: Сетусернаме**](iscrdenr-setusername.md)
</dt> </dl>

 

 




