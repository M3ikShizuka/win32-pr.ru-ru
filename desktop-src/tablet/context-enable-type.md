---
description: Указывает, должны ли сообщения контекста отправляться в оконную процедуру окна-владельца.
ms.assetid: 57ecf10a-8a02-4353-b916-9080ebc0b270
title: Перечисление CONTEXT_ENABLE_TYPE
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CONTEXT_ENABLE_TYPE
api_type:
- NA
api_location: ''
ms.openlocfilehash: cd741eeff1cc3e2ce055a84dd646c3aa2563f217
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127344927"
---
# <a name="context_enable_type-enumeration"></a>\_ \_ Перечисление типов включения контекста

Указывает, должны ли сообщения контекста отправляться в оконную процедуру окна-владельца.

## <a name="syntax"></a>Синтаксис


```C++
typedef enum _CONTEXT_ENABLE_TYPE { 
  CONTEXT_ENABLE   = 1,
  CONTEXT_DISABLE  = 2
} CONTEXT_ENABLE_TYPE;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="CONTEXT_ENABLE"></span><span id="context_enable"></span>**\_включение контекста**
</dt> <dd>

Необходимо включить контекст планшета, в результате чего сообщения контекста отправляются в оконную процедуру окна-владельца.

</dd> <dt>

<span id="CONTEXT_DISABLE"></span><span id="context_disable"></span>**\_Отключение контекста**
</dt> <dd>

Контекст планшета должен быть отключен, предотвращая дальнейшую отправку сообщений контекста в процедуру окна или приемник событий окна-владельца.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/> |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                     |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Метод Итаблет:: CreateContext**](itablet-createcontext.md)
</dt> </dl>

 

 




