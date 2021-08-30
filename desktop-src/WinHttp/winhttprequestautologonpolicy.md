---
description: Включает возможные параметры для политики автоматического входа в систему.
ms.assetid: dad4f6a7-8e84-4f4f-b962-4189e3dc01f7
title: Перечисление Винхттпрекуестаутологонполици
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- WinHttpRequestAutoLogonPolicy
api_type:
- IDLDef
api_location:
- HttpRequest.idl
ms.openlocfilehash: 2db50abfa413fc8ed80724ce2955407624c836a14809da678989753668794f6c
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119899084"
---
# <a name="winhttprequestautologonpolicy-enumeration"></a>Перечисление Винхттпрекуестаутологонполици

Перечисление **винхттпрекуестаутологонполици** включает возможные параметры для [политики автоматического входа в систему](authentication-in-winhttp.md).

## <a name="syntax"></a>Синтаксис


```C++
typedef enum WinHttpRequestAutoLogonPolicy { 
  AutoLogonPolicy_Always             = 0,
  AutoLogonPolicy_OnlyIfBypassProxy  = 1,
  AutoLogonPolicy_Never              = 2
} WinHttpRequestAutoLogonPolicy;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="AutoLogonPolicy_Always"></span><span id="autologonpolicy_always"></span><span id="AUTOLOGONPOLICY_ALWAYS"></span>**Аутологонполици \_ всегда**
</dt> <dd>

Вход с проверкой подлинности с использованием учетных данных по умолчанию выполняется для всех запросов.

</dd> <dt>

<span id="AutoLogonPolicy_OnlyIfBypassProxy"></span><span id="autologonpolicy_onlyifbypassproxy"></span><span id="AUTOLOGONPOLICY_ONLYIFBYPASSPROXY"></span>**Аутологонполици \_ онлифбипасспрокси**
</dt> <dd>

Вход с проверкой подлинности с использованием учетных данных по умолчанию выполняется только для запросов в локальной интрасети. Локальная интрасеть считается любым сервером в списке обхода прокси-сервера в текущей конфигурации прокси-сервера.

</dd> <dt>

<span id="AutoLogonPolicy_Never"></span><span id="autologonpolicy_never"></span><span id="AUTOLOGONPOLICY_NEVER"></span>**Аутологонполици \_ никогда**
</dt> <dd>

Проверка подлинности не используется автоматически.

</dd> </dl>

## <a name="remarks"></a>Remarks

Чтобы задать политику автоматического входа в систему, вызовите метод [**сетаутологонполици**](iwinhttprequest-setautologonpolicy.md) и укажите одну из приведенных выше констант.

> [!Note]  
> сведения о Windows XP и Windows 2000 см. в разделе [требования к времени выполнения](winhttp-start-page.md) на начальной странице WinHTTP.

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP, Windows 2000 Professional с SP3 \[ только для настольных приложений\]<br/>            |
| Минимальная версия сервера<br/> | Windows сервер 2003, Windows 2000 server с пакетом обновления 3 (SP3), \[ только классические приложения\]<br/>         |
| Распространяемые компоненты<br/>          | WinHTTP 5,0 и Internet Explorer 5,01 или более поздней версии в Windows XP и Windows 2000.<br/> |
| IDL<br/>                      | <dl> <dt>HttpRequest. idl</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Версии WinHTTP](winhttp-versions.md)
</dt> </dl>

 

 




