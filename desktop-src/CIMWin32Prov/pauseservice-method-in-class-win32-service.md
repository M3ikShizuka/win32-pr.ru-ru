---
description: Метод PauseService класса Win32_Service (поставщики WMI CIMWin32) — пытается перевести службу в приостановленное состояние.
ms.assetid: 5382457e-7f9c-48a5-9262-b815a1a4a605
ms.tgt_platform: multiple
title: Метод PauseService класса Win32_Service (поставщики WMI CIMWin32)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Win32_Service.PauseService
api_type:
- COM
api_location:
- CIMWin32.dll
ms.openlocfilehash: 7654feea410564137e98861c4c0b5de2b5e7192e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054939"
---
# <a name="pauseservice-method-of-the-win32_service-class-cimwin32-wmi-providers"></a>Метод PauseService класса Win32_Service (поставщики WMI CIMWin32)

Метод  [класса WMI](/windows/desktop/WmiSdk/retrieving-a-class) PauseService пытается перевести службу в приостановленное состояние.

В этом разделе используется синтаксис MOF-файл (MOF). Дополнительные сведения об использовании этого метода см. [в разделе вызов метода](/windows/desktop/WmiSdk/calling-a-method).

## <a name="syntax"></a>Синтаксис


```mof
uint32 PauseService();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает одно из значений, перечисленных в следующем списке, или любое другое значение, указывающее на ошибку. Дополнительные коды ошибок см. в разделе [**константы WMI Error**](/windows/desktop/WmiSdk/wmi-error-constants) или [**вбемерроренум**](/windows/desktop/api/wbemdisp/ne-wbemdisp-wbemerrorenum). Общие значения **HRESULT** см. в разделе [коды системных ошибок](/windows/desktop/Debug/system-error-codes).

<dl> <dt>

**0**
</dt> <dd>

Запрос принят.

</dd> <dt>

**1**
</dt> <dd>

Запрос не поддерживается.

</dd> <dt>

**2**
</dt> <dd>

У пользователя нет необходимых прав доступа.

</dd> <dt>

**3**
</dt> <dd>

Службу нельзя остановить, так как от нее зависят другие работающие службы.

</dd> <dt>

**4**
</dt> <dd>

Запрошенный управляющий код недопустим или неприемлем для данной службы.

</dd> <dt>

**5**
</dt> <dd>

Запрошенный управляющий код не может быть отправлен в службу, так как это состояние службы ([**Win32 \_ басесервице**](win32-baseservice.md).**Свойство State** ) равно 0, 1 или 2.

</dd> <dt>

**6**
</dt> <dd>

Служба не запущена.

</dd> <dt>

**7**
</dt> <dd>

Служба не ответила на запрос запуска за отведенное время.

</dd> <dt>

**8**
</dt> <dd>

Неизвестный сбой при запуске службы.

</dd> <dt>

**9**
</dt> <dd>

Не найден путь к каталогу исполняемого файла службы.

</dd> <dt>

**10**
</dt> <dd>

Служба уже запущена.

</dd> <dt>

**11**
</dt> <dd>

База данных для добавления новой службы заблокирована.

</dd> <dt>

**12**
</dt> <dd>

Зависимость, от которой зависит эта служба, удалена из системы.

</dd> <dt>

**13**
</dt> <dd>

Этой службе не удалось найти службу, которая необходима зависимой службе.

</dd> <dt>

**14**
</dt> <dd>

Эта служба была отключена в системе.

</dd> <dt>

**15**
</dt> <dd>

Эта служба не поддерживает проверку подлинности, необходимую для работы в системе.

</dd> <dt>

**16**
</dt> <dd>

Эта служба удаляется из системы.

</dd> <dt>

**17**
</dt> <dd>

Служба не имеет потока выполнения.

</dd> <dt>

**стр**
</dt> <dd>

Служба имеет циклические зависимости при запуске.

</dd> <dt>

**19**
</dt> <dd>

Служба выполняется с тем же именем.

</dd> <dt>

**20**
</dt> <dd>

Имя службы содержит недопустимые символы.

</dd> <dt>

**открыт**
</dt> <dd>

Службе переданы недопустимые параметры.

</dd> <dt>

**22**
</dt> <dd>

Учетная запись, под которой работает эта служба, либо недопустима, либо не имеет разрешений на запуск службы.

</dd> <dt>

**23**
</dt> <dd>

Служба существует в базе данных доступных в системе служб.

</dd> <dt>

**24**
</dt> <dd>

Служба в данный момент приостановлена в системе.

</dd> </dl>

## <a name="remarks"></a>Комментарии

Определив, какие службы могут быть остановлены или приостановлены, можно использовать [**методы "**](stopservice-method-in-class-win32-service.md) [**PauseService**](pauseservice-method-in-class-win32-systemdriver.md) " и "приостановить" для остановки и приостановки служб. Решение о прекращении работы службы, а не приостановке или наоборот, зависит от нескольких факторов, включая следующие:

-   Может ли служба быть приостановлена? В противном случае единственным вариантом будет «останавливает службу».
-   Нужно ли продолжать обработку запросов клиентов для всех, кто уже подключен к службе? Если да, то приостановка службы обычно позволяет ей управлять существующими клиентами при запрете доступа к новым клиентам. Напротив, при прекращении службы все клиенты сразу же отключаются.
-   Нужно ли перенастроить службу, чтобы изменения вступили в силу немедленно? Несмотря на то, что свойства службы могут быть изменены, пока служба приостановлена, большинство из них не вступают в силу, пока служба не будет остановлена и перезапущена.

Код скрипта, необходимый для остановки службы, почти идентичен коду, требуемому для приостановки службы.

## <a name="examples"></a>Примеры

[Службы Pause, работающие под конкретной учетной записью,](https://Gallery.TechNet.Microsoft.Com/12a256dd-39da-4690-b3f0-f0adccaf25f1) заостанавливают все службы, работающие под гипотетической учетной записью службы "нетсвк".

В следующем примере кода VBScript показано, как приостановить определенную службу из экземпляров [**\_ службы Win32**](win32-service.md).

> [!Note]  
> Служба должна поддерживать приостановку и выполнение уже запущено.

 


```VB
Set ServiceSet = GetObject("winmgmts:").ExecQuery("select * from Win32_Service where Name='Schedule'")

for each Service in ServiceSet
 SupportsPause = Service.AcceptPause
 if SupportsPause = true then
  RetVal = Service.PauseService()
  if RetVal = 0 then 
   WScript.Echo "Service paused"   
  else
   if RetVal = 1 then 
    WScript.Echo "Pause not supported" 
   else WScript.Echo "An error occurred:" & RetVal
   End If
  End If
 else
  WScript.Echo "Service does not support pause"
 end if
next
```



В следующем образце кода Perl показано, как приостановить определенную службу из [**экземпляров \_ службы Win32**](win32-service.md).

> [!Note]  
> Служба должна поддерживать приостановку и выполнение уже запущено.

 


```
use strict;
use Win32::OLE;

my ($ServiceSet, $SupportsPause, $RetVal);  
eval {$ServiceSet = Win32::OLE->GetObject("winmgmts:{impersonationLevel=impersonate}!\\\\.\\Root\\CIMv2")->
 ExecQuery("SELECT * FROM Win32_Service WHERE Name='Schedule'"); };
unless($@)
{
 foreach my $ServiceInst (in $ServiceSet)
 {
  if ($ServiceInst->{AcceptPause})
  {
   $RetVal = $ServiceInst->PauseService();
   if ($RetVal == 0)
   {
    print "\nService paused\n";
   }
   else
   {
    if ($RetVal == 1)
    {
     print "\nPause not supported\n" ;
    }
    else 
    {
     print "\nAn error occurred:", $RetVal, "\n";
    }
   } 
  }
  else
  {
   print "\nService does not support pause\n";
  }
 }
}
else
{
 print STDERR "\n", Win32::OLE->LastError, "\n";
}
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                          |
| Пространство имен<br/>                | Root\\CIMv2<br/>                                                                  |
| MOF<br/>                      | <dl> <dt>CIMWin32. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>CIMWin32.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Классы операционной системы](/previous-versions//aa392727(v=vs.85))
</dt> <dt>

[**\_Служба Win32**](win32-service.md)
</dt> <dt>

[Задачи WMI: службы](/windows/desktop/WmiSdk/wmi-tasks--services)
</dt> <dt>

[**StopService**](stopservice-method-in-class-win32-service.md)
</dt> </dl>

 

