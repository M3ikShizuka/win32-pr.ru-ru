---
description: Следующие константы могут возвращаться как ошибки.
ms.assetid: 185bd906-c276-4075-9c23-eb112da2a7ca
title: Константы RND_ (Рндерр. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 54a89b6747fb9fef775bbf40fac472081567ff1a
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127462644"
---
# <a name="rnd_-constants"></a>\_Константы Rnd

\[встречи и элементы управления встречными IP-телефонными соединениями недоступны для использования в Windows Vista, Windows Server 2008 и последующих версиях операционной системы. API клиента RTC предоставляет аналогичные функциональные возможности.\]

Следующие константы могут возвращаться как ошибки.

<dl> <dt>

<span id="RND_INVALID_TIME"></span><span id="rnd_invalid_time"></span>**\_недопустимое \_ время Rnd**
</dt> <dd> <dl> <dt>

 0xe0000200
</dt> <dt>



Указано недопустимое значение времени.


</dt> </dl> </dd> <dt>

<span id="RND_NULL_SERVER_NAME"></span><span id="rnd_null_server_name"></span>**\_имя неопределенного \_ сервера \_**
</dt> <dd> <dl> <dt>

 0xe0000201
</dt> <dt>



Имя сервера равно **null**, возможно, из-за того, что [**Итконференцеблоб:: init**](itconferenceblob-init.md) не был запущен или завершился неудачно.


</dt> </dl> </dd> <dt>

<span id="RND_ALREADY_CONNECTED"></span><span id="rnd_already_connected"></span>**Функция RND \_ уже \_ подключена**
</dt> <dd> <dl> <dt>

 0xe0000202
</dt> <dt>



был вызван метод [**итдиректори:: Подключение**](/windows/desktop/api/Rend/nf-rend-itdirectory-connect) , но соединение уже существует.


</dt> </dl> </dd> <dt>

<span id="RND_NOT_CONNECTED"></span><span id="rnd_not_connected"></span>**RND \_ не \_ подключен**
</dt> <dd> <dl> <dt>

 0xe0000203
</dt> <dt>



метод [**итдиректори:: Подключение**](/windows/desktop/api/Rend/nf-rend-itdirectory-connect) не был вызван или завершился ошибкой.


</dt> </dl> </dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------|-------------------------------------------------------------------------------------|
| Версия TAPI<br/> | Требуется TAPI 3,0 или более поздней версии<br/>                                               |
| Заголовок<br/>       | <dl> <dt>Рндерр. h</dt> </dl> |



 

 




