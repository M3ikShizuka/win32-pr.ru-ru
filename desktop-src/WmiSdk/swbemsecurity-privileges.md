---
description: Свойство Privileges является объектом Свбемпривилежесет. это свойство используется для включения или отключения специальных привилегий Windows. может потребоваться установить одно из этих привилегий для выполнения конкретных задач с помощью API инструментарий управления Windows (WMI) (WMI).
ms.assetid: 6e4cae22-23d6-4981-b38c-d298654e59ab
ms.tgt_platform: multiple
title: Свойство Свбемсекурити. Privileges (Wbemdisp. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SWbemSecurity.Privileges
- ISWbemSecurity.Privileges
- ISWbemSecurity.get_Privileges
api_type:
- COM
api_location:
- Wbemdisp.dll
ms.openlocfilehash: a4b2ca68f0377616d693c677281b90f2e4650fcacc941e205e1732ae5a91e4b1
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119897504"
---
# <a name="swbemsecurityprivileges-property"></a>Свбемсекурити. Privileges, свойство

Свойство **Privileges** является объектом [**свбемпривилежесет**](swbemprivilegeset.md) . это свойство используется для включения или отключения специальных привилегий Windows. может потребоваться установить одно из этих привилегий для выполнения конкретных задач с помощью API инструментарий управления Windows (WMI) (WMI).

Описание этого синтаксиса см. в разделе [соглашения о документе для API скриптов](document-conventions-for-the-scripting-api.md).

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```VB
SWbemSecurity.Privileges As Object
```



## <a name="property-value"></a>Значение свойства

## <a name="remarks"></a>Remarks

Этот параметр позволяет предоставлять или отзывать привилегии как часть строки моникера WMI. Полный список применимых значений см. в разделе константы [**вбемпривилежеенум**](/windows/desktop/api/Wbemdisp/ne-wbemdisp-wbemprivilegeenum) и [**Privileges**](privilege-constants.md).

Можно изменить привилегии, определенные для объектов [**SwbemServices**](swbemservices.md), [**SWbemObject**](swbemobject.md), [**SWbemObjectSet**](swbemobjectset.md), [**свбемобжектпас**](swbemobjectpath.md)и [**SwbemLocator**](swbemlocator.md) , добавив [**свбемпривилеже**](swbemprivilege.md) объекты в свойство **Privileges** .

существуют фундаментальные различия в том, как различные версии Windows обрабатывают изменения в привилегиях. если вы разрабатываете приложение, которое используется только на платформах Windows, вы можете установить или отозвать привилегии в любое время.

В следующем примере задается **SeDebugPrivilege** для первого подключения моникера, чтобы получить объект [**SwbemServices**](swbemservices.md) .


```VB
Set Service = GetObject( _
    "winmgmts:{impersonationLevel=impersonate, (Debug)}")
```



Дополнительные сведения о форматировании строки безопасности для подключения моникера см. в разделе [**константы прав**](privilege-constants.md).

В следующем примере выполняется та же задача, но она устанавливает привилегию после первоначального входа в WMI.


```VB
Set Service = GetObject( _
    "winmgmts:{impersonationLevel=impersonate}")
Service.Security_.Privileges.AddAsString "SeDebugPrivilege", True
```



Обратите внимание, что для вызовов [**свбемпривилежесет. аддасстринг**](swbemprivilegeset-addasstring.md)необходимо использовать полное имя права доступа, например "SeDebugPrivilege", а не "Debug".

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Wbemdisp. h</dt> </dl>   |
| Библиотека типов<br/>             | <dl> <dt>Wbemdisp. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Wbemdisp.dll</dt> </dl> |
| CLSID<br/>                    | \_СВБЕМСЕКУРИТИ CLSID<br/>                                                         |
| IID<br/>                      | IID \_ исвбемсекурити<br/>                                                          |



## <a name="see-also"></a>См. также

<dl> <dt>

[**свбемсекурити**](swbemsecurity.md)
</dt> <dt>

[Выполнение привилегированных операций](executing-privileged-operations.md)
</dt> <dt>

[**свбемпривилежесет**](swbemprivilegeset.md)
</dt> </dl>

 

 




