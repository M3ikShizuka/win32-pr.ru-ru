---
description: Свойство безопасности объекта Свбемобжектпас используется для получения или задания компонентов безопасности пути к объекту.
ms.assetid: 26e5e990-3b78-41b6-83c4-ba0d8b0d2f00
ms.tgt_platform: multiple
title: Свойство SWbemObjectPath.Security_ (Wbemdisp. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- SWbemObjectPath.Security_
- ISWbemObjectPath.Security_
- ISWbemObjectPath.get_Security_
api_type:
- COM
api_location:
- Wbemdisp.dll
ms.openlocfilehash: 000f3f5e334ef0eba3dbd687d7bdc4b594442305
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967057"
---
# <a name="swbemobjectpathsecurity_-property"></a>Свбемобжектпас. Security, \_ свойство

Свойство **безопасности** объекта [**свбемобжектпас**](swbemobjectpath.md) используется для получения или задания компонентов безопасности пути к объекту. Обратите внимание, что он не используется для установки атрибутов безопасности самого объекта **свбемобжектпас** . Он используется только для представления компонентов безопасности пути к объекту [**SWbemLocator**](swbemlocator.md) . Это свойство является объектом [**свбемсекурити**](swbemsecurity.md) .

> [!Note]  
> Установка свойства [**безопасности \_**](swbemobject-security-.md) объекта [**свбемобжектпас**](swbemobjectset.md) в **значение NULL** предоставляет всем пользователям неограниченный доступ. Дополнительные сведения см. в разделе [**свбемсекурити**](swbemsecurity.md).

 

Дополнительные сведения см. [в разделе соглашения о документе для API скриптов](document-conventions-for-the-scripting-api.md).

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```VB
SWbemObjectPath.Security_ As Object
```



## <a name="property-value"></a>Значение свойства

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Wbemdisp. h</dt> </dl>   |
| Библиотека типов<br/>             | <dl> <dt>Wbemdisp. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Wbemdisp.dll</dt> </dl> |
| CLSID<br/>                    | \_СВБЕМОБЖЕКТПАС CLSID<br/>                                                       |
| IID<br/>                      | IID \_ исвбемобжектпас<br/>                                                        |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**свбемобжектпас**](swbemobjectpath.md)
</dt> <dt>

[Создание приложения или скрипта WMI](creating-a-wmi-application-or-script.md)
</dt> <dt>

[Настройка \_ \_ безопасности процесса клиентского приложения](setting-client-application-process-security.md)
</dt> </dl>

 

 




