---
description: Shell. Иссервицеруннинг-метод — возвращает значение, указывающее, запущена ли определенная служба.
ms.assetid: FDC41C2D-7462-458f-BBE6-D97260C26B6C
title: Метод Shell. Иссервицеруннинг (Шлдисп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Shell.IsServiceRunning
api_type:
- COM
api_location:
- Shell32.dll
ms.openlocfilehash: 01af900bb7930ec7b6dde0b0700c83f211733dc3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127460352"
---
# <a name="shellisservicerunning-method"></a>Shell. Иссервицеруннинг, метод

Возвращает значение, указывающее, запущена ли определенная служба.

## <a name="syntax"></a>Синтаксис


```JScript
retVal = Shell.IsServiceRunning(
  sServiceName
)
```


```VB

Shell.IsServiceRunning( _
  ByVal sServiceName As BSTR _
) As Variant
```





## <a name="parameters"></a>Параметры

<dl> <dt>

*ссервиценаме* \[ окне\]
</dt> <dd>

Тип: **[ **BSTR**](/previous-versions/windows/desktop/automat/bstr)**

**Строка** , содержащая имя службы.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

### <a name="jscript"></a>Язык JScript

Тип: **Variant \***

Возвращает **значение true** , если служба, указанная параметром *ссервиценаме* , запущена. в противном случае — **значение false**.

### <a name="vb"></a>VB

Тип: **Variant \***

Возвращает **значение true** , если служба, указанная параметром *ссервиценаме* , запущена. в противном случае — **значение false**.

## <a name="remarks"></a>Remarks

Этот метод в настоящее время недоступен в Microsoft Visual Basic.

## <a name="examples"></a>Примеры

В следующих примерах показано использование **иссервицеруннинг** для определения того, запущена ли служба "темы" для приложения. для JScript и VBScript отображается использование.

JScript:


```JScript
function fnIsServiceRunningJ()
{
    var objShell = new ActiveXObject("shell.application");
    var bReturn;

    bReturn = objShell.IsServiceRunning("Themes");
}
```



Сценариев


```VB
function fnIsServiceRunningVB()
    dim objShell
    dim bReturn

    set objShell = CreateObject("shell.application")

    bReturn = objShell.IsServiceRunning("Themes")

    set objShell = nothing
end function
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional, только для \[ настольных приложений Windows XP\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Шлдисп. h</dt> </dl>                          |
| IDL<br/>                      | <dl> <dt>Шлдисп. idl</dt> </dl>                        |
| DLL<br/>                      | <dl> <dt>Shell32.dll (версия 5,0 или более поздняя)</dt> </dl> |



 

 
