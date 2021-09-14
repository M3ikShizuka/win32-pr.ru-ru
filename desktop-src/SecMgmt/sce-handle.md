---
description: '\_Тип данных Handle обработчика SCE является непрозрачным маркером, предоставляемым набором средств настройки безопасности. Он используется в ПФСЦЕ \_ запроса \_ info и \_ \_ функциях поддержки пфсце Set info для передачи информации между вложением и базой данных безопасности.'
ms.assetid: 8db91e6f-b31e-40c6-a158-b4b3b00ba0c0
title: SCE_HANDLE (Сцесвк. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3fef21dbe03d97dfa14537d5df132ba3cb222643
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064581"
---
# <a name="sce_handle"></a>\_обработчик SCE

Тип **данных \_ Handle обработчика SCE** является непрозрачным маркером, предоставляемым набором средств настройки безопасности. Он используется в [**пфсце \_ запроса \_ info**](/windows/win32/api/scesvc/nc-scesvc-pfsce_query_info) и функциях поддержки [**пфсце \_ Set \_ info**](/windows/win32/api/scesvc/nc-scesvc-pfsce_set_info) для передачи информации между вложением и базой данных безопасности.


```C++
typedef PVOID SCE_HANDLE;
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                         |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Сцесвк. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_ \_ сведения о запросе пфсце**](/windows/win32/api/scesvc/nc-scesvc-pfsce_query_info)
</dt> <dt>

[**\_сведения о наборе пфсце \_**](/windows/win32/api/scesvc/nc-scesvc-pfsce_set_info)
</dt> </dl>

 

