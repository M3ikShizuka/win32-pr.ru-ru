---
description: IShellDispatch2. Жетсистеминформатион, метод возвращает сведения о системе.
ms.assetid: 57c066e3-080f-4ecc-b56e-877f0569e901
title: IShellDispatch2. Жетсистеминформатион, метод (Шлдисп. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IShellDispatch2.GetSystemInformation
api_type:
- COM
api_location:
- Shell32.dll
ms.openlocfilehash: a81ac091dc1905c1cbcd2c41575c907ce957e60c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127262539"
---
# <a name="ishelldispatch2getsysteminformation-method"></a>IShellDispatch2. Жетсистеминформатион, метод

Возвращает сведения о системе.

## <a name="syntax"></a>Синтаксис


```JScript
retVal = IShellDispatch2.GetSystemInformation(
  sName
)
```


```VB

IShellDispatch2.GetSystemInformation( _
  ByVal sName As BSTR _
) As Variant
```





## <a name="parameters"></a>Параметры

<dl> <dt>

*sName* \[ окне\]
</dt> <dd>

Тип: **[ **BSTR**](/previous-versions/windows/desktop/automat/bstr)**

**Строка** , указывающая запрашиваемую информацию о системе.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

### <a name="jscript"></a>Язык JScript

Тип: **Variant**

Возвращает значение запрошенной системной информации. Тип возвращаемого значения зависит от того, какие сведения о системе запрашиваются. Подробные сведения см. в разделе "Заметки".

### <a name="vb"></a>VB

Тип: **Variant**

Возвращает значение запрошенной системной информации. Тип возвращаемого значения зависит от того, какие сведения о системе запрашиваются. Подробные сведения см. в разделе "Заметки".

## <a name="remarks"></a>Комментарии

Этот метод реализован и доступен через метод [**Shell. жетсистеминформатион**](./shell-getsysteminformation.md) .

Этот метод можно использовать для запроса многих значений системных сведений. В следующей таблице приводится значение *sName* , которое используется для запроса сведений и связанного типа возвращаемого значения.



*sName*

Возвращаемый тип

Описание

директорисервицеаваилабле

**Boolean**

Задайте **значение true** , если служба каталогов доступна. в противном случае — **значение false**.

даублекликктиме

**Integer**

Время двойного щелчка в миллисекундах.

ProcessorLevel

**Integer**

**Windows Vista и более поздних версий**. Уровень процессора. Возвращает 3, 4 или 5 для процессоров x386, x486 и Pentium-Level соответственно.

ProcessorSpeed

**Integer**

Скорость процессора в мегагерцах (МГц).

ProcessorArchitecture

**Integer**

Архитектура процессора. Дополнительные сведения см. в обсуждении члена **впроцессорарчитектуре** структуры [**System \_ info**](/windows/win32/api/sysinfoapi/ns-sysinfoapi-system_info) .

фисикалмеморинсталлед

**Integer**

Объем установленной физической памяти в байтах.

следующие действия допустимы только в Windows XP.

ISO \_ Professional

**Boolean**

задайте **значение true** , если операционная система работает Windows XP Professional Edition. в противном случае — **значение false**.

ISO \_ персональный

**Boolean**

задайте **значение true** , если операционная система работает Windows XP Home Edition. в противном случае — **значение false**.

следующие действия допустимы только в Windows XP и более поздних версиях.

ISO \_ домаинмембер

**Boolean**

Задайте **значение true** , если компьютер является членом домена. в противном случае — **значение false**.



 

Этот метод в настоящее время недоступен в Microsoft Visual Basic.

## <a name="examples"></a>Примеры

в следующих примерах показано использование **жетсистеминформатион** для JScript и VBScript.

JScript:


```JScript
<script language="JavaScript">
    function fnGetSystemInformationJ()
    {
        var objShell = new ActiveXObject("shell.application");
        var vReturn;

        vReturn = objShell.GetSystemInformation("ProcessorLevel");
        document.write(vReturn);
    }
</script>
```



Сценариев


```VB
<script language="VBScript">
    function fnGetSystemInformationVB()
        dim objShell
        dim vReturn

        set objShell = CreateObject("shell.application")

        vReturn = objShell.GetSystemInformation("ProcessorLevel")
        document.write(vReturn)

        set objShell = nothing
    end function
</script>
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional, только для \[ настольных приложений Windows XP\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Шлдисп. h</dt> </dl>                          |
| IDL<br/>                      | <dl> <dt>Шлдисп. idl</dt> </dl>                        |
| DLL<br/>                      | <dl> <dt>Shell32.dll (версия 5,0 или более поздняя)</dt> </dl> |



 

 
