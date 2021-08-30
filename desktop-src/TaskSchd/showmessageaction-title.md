---
title: Шовмессажеактион. Title, свойство
description: Для создания скриптов Возвращает или задает заголовок окна сообщения.
ms.assetid: f61177fc-287c-4da9-9bdc-88aaa6868204
keywords:
- планировщик задач свойства Title
- Свойство Title планировщик задач, объект Шовмессажеактион
- Планировщик задач объекта Шовмессажеактион, свойство Title
topic_type:
- apiref
api_name:
- ShowMessageAction.Title
api_location:
- taskschd.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: c4297bf3d845495e1783d3d8c65f64fc5df85a555b58d9afeb4a80c0fe96b517
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120072614"
---
# <a name="showmessageactiontitle-property"></a>Шовмессажеактион. Title, свойство

\[Этот объект больше не поддерживается. для отображения сообщения в сеансе пользователя можно использовать иексекактион с функцией Windows scripting [**MsgBox**](/previous-versions/sfw6660x(v=vs.80)) .\]

Для создания скриптов Возвращает или задает заголовок окна сообщения.

## <a name="syntax"></a>Синтаксис


```VB
ShowMessageAction.Title As String
```



## <a name="property-value"></a>Значение свойства

Название окна сообщения.

## <a name="remarks"></a>Remarks

Параметризованные строки можно использовать в тексте заголовка окна сообщения. Дополнительные сведения см. в разделе "примеры" в [**EventTrigger. валуекуериес**](eventtrigger-valuequeries.md).

При задании значения этого свойства значением может быть текст, полученный из файла .dll ресурсов. Для ссылки на текст из файла ресурсов используется специализированная строка. Строка имеет формат $ (@ \[ DLL \] , \[ ResourceId \] ), где \[ Dll — это \] путь к .dll файлу, содержащему ресурс, а \[ ResourceId \] — идентификатор для текста ресурса. Например, при установке значения этого свойства в $ (@% SystemRoot% \\ System32 \\ResourceName.dll,-101) свойству будет присвоено значение текста ресурса с идентификатором, равным-101, в файле% SystemRoot% \\ system32 \\ResourceName.dll.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                    |
| Окончание поддержки клиента<br/>    | Windows 7<br/>                                                                    |
| Поддержка конца сервера<br/>    | Windows Server 2008 R2<br/>                                                       |
| Библиотека типов<br/>             | <dl> <dt>Тасксчд. tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Taskschd.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**шовмессажеактион**](showmessageaction.md)
</dt> </dl>

 

