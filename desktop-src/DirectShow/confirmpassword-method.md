---
description: Метод Двдадм. ConfirmPassword проверяет, соответствует ли указанный пароль ранее сохраненному паролю.
ms.assetid: 4dddc28d-edf7-45a2-ae1f-1c37b5df2eea
title: Метод ConfirmPassword (Segment. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 5f14b3a40a37828bc978b5dd302a14b4f65053d982ac0da68d43284fe2ac3f3c
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118954223"
---
# <a name="confirmpassword-method"></a>Метод ConfirmPassword

> [!Note]  
> этот компонент доступен для использования в операционных системах Microsoft Windows 2000, Windows XP и Windows Server 2003. В последующих версиях он может быть изменен или недоступен.

 

`DVDAdm.ConfirmPassword`Метод проверяет, соответствует ли указанный пароль ранее сохраненному паролю.

``` syntax
[ bIsConfirmed = ] DVD.DVDAdm.ConfirmPassword(sUserName, sPassword)
```

## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="sUserName"></span><span id="susername"></span><span id="SUSERNAME"></span>*сусернаме*
</dt> <dd>

Указывает имя пользователя в виде строки.

</dd> <dt>

<span id="sPassword"></span><span id="spassword"></span><span id="SPASSWORD"></span>*спассворд*
</dt> <dd>

Указывает новый пароль в виде строки.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение true, если указанный пароль совпадает с существующим паролем, и false в противном случае.

## <a name="remarks"></a>Remarks

В настоящее время параметр *сусернаме* игнорируется на этом и всех связанных методах.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------|--------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Сегмент. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**ChangePassword;**](changepassword-method.md)
</dt> <dt>

[Объект Мсдвдадм](msdvdadm-object.md)
</dt> </dl>

 

 




