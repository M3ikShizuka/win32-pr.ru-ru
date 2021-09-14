---
title: Сообщение EM_SETTARGETDEVICE (RichEdit. h)
description: Задает целевое устройство и толщину линии, используемые для \ 0034; что вы получаете \ 0034; (WYSIWYG) форматирование в элементе управления Rich Edit.
ms.assetid: dfc829f5-e711-419e-abb5-c1e8df994c4a
keywords:
- элементы управления Windows сообщений EM_SETTARGETDEVICE
topic_type:
- apiref
api_name:
- EM_SETTARGETDEVICE
api_location:
- Richedit.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 8f82d6ee5df86572564cffcf192395ccee1fbd05
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054307"
---
# <a name="em_settargetdevice-message"></a>\_Сообщение СЕТТАРЖЕТДЕВИЦЕ EM

Задает целевое устройство и толщину линии, используемой для "что вы видите" (WYSIWYG) в элементе управления Rich Edit.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

HDC для целевого устройства.

</dd> <dt>

*lParam* 
</dt> <dd>

Толщина линии, используемой для форматирования.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращаемое значение равно нулю, если операция завершается с ошибкой, или ненулевой, если она завершается успешно.

## <a name="remarks"></a>Комментарии

Параметр HDC для принтера по умолчанию можно получить следующим образом.


```
PRINTDLG pd = { sizeof(pd) };
pd.Flags = PD_RETURNDC | PD_RETURNDEFAULT;
if (PrintDlg(&pd))
{
    HDC hdc = pd.hDC;
    ...
}
```



Если значение *lParam* равно нулю, разрывы строк не создаются.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>RichEdit. h</dt> </dl> |



 

 





