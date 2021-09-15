---
title: '\_ \_ Центр ОТВ для EAP (еаптипес. h)'
description: Хранит учетные данные безопасности EAP в \_ \_ структуре массива входных полей конфигурации EAP \_ \_ . | \_ \_ Центр ОТВ для EAP (еаптипес. h)
ms.assetid: 714c75d8-71c7-4c3f-802a-a5e4f6ca65c2
keywords:
- EAP_CRED_RESP
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e5c2176377dbde0f7c02d2a7d8083ad1bcff9e71
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127571890"
---
# <a name="eap_cred_resp"></a>подотчетное от EAP \_ cred \_

Структура **\_ \_ ОТВ** для удостоверения EAP хранит учетные данные безопасности EAP в структуре [**\_ \_ \_ \_ массива входных полей конфигурации EAP**](/windows/desktop/api/eaptypes/ns-eaptypes-eap_config_input_field_array) .


```C++
typedef EAP_CONFIG_INPUT_FIELD_ARRAY EAP_CRED_RESP;
```



<dl> <dt>

**подотчетное от EAP \_ cred \_**
</dt> <dd>

В структуре "удостоверение для удостоверения EAP" хранятся как старые, так и новые учетные данные безопасности EAP, на которые указывает параметр *пбуидата* структуры [**\_ данных интерактивного \_ пользовательского интерфейса \_ EAP**](/windows/desktop/api/eaptypes/ns-eaptypes-eap_interactive_ui_data) , если параметр *Двдататипе* [**\_ \_ \_ \_ типа данных "интерактивный пользовательский интерфейс EAP**](/windows/desktop/api/eaptypes/ne-eaptypes-eap_interactive_ui_data_type) " указывает тип ответа учетных данных. **\_ \_**

</dd> </dl>

## <a name="remarks"></a>Комментарии

Структура **\_ \_ ОТВ** для идентификации EAP используется для поддержки единого входа (SSO).

Структура **\_ \_ ОТВ** для правил для EAP идентична структуре запросов на назначение [**EAP \_ \_**](eap-cred-req.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Еаптипес. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Структуры запрашивающего сторона EAPHost](eap-host-supplicant-structures.md)
</dt> <dt>

[**Заявка на для EAP \_ cred \_**](eap-cred-req.md)
</dt> <dt>

[**запрос \_ на \_ истечение срока действия CRED EAP \_**](/windows/desktop/api/eaptypes/ns-eaptypes-eap_cred_expiry_req)
</dt> <dt>

[**\_отв. \_ истечение срока действия для истечения EAP \_**](/previous-versions/windows/desktop/legacy/bb530539(v=vs.85))
</dt> <dt>

[**\_Интерактивные \_ данные ПОЛЬЗОВАТЕЛЬСКОГО интерфейса EAP \_**](/windows/desktop/api/eaptypes/ns-eaptypes-eap_interactive_ui_data)
</dt> <dt>

[Единый вход и PLAP](understanding-sso-and-plap.md)
</dt> </dl>

 

