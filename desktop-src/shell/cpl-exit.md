---
description: Отправляется один раз в функцию Кплапплет приложения панели управления до выпуска библиотеки DLL, содержащей приложение панели управления.
ms.assetid: 1afcb0d3-41a7-4fd8-9561-d96e1e8f0ddb
title: Сообщение CPL_EXIT (CPL. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 9007c05de134b32e3c4dfd7b256f2392f547d298b2d654dddc256b6ed711bb9e
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119715606"
---
# <a name="cpl_exit-message"></a>\_Сообщение выхода CPL

Отправляется один раз в функцию [**кплапплет**](/windows/win32/api/cpl/nc-cpl-applet_proc) приложения панели управления до выпуска библиотеки DLL, содержащей приложение панели управления.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>Должен равняться нулю.</dd> <dt>

*lParam* 
</dt> <dd>Должен равняться нулю.</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если функция [**кплапплет**](/windows/win32/api/cpl/nc-cpl-applet_proc) успешно обрабатывает это сообщение, оно должно вернуть ноль.

## <a name="remarks"></a>Remarks

Это сообщение отправляется после отправки последнего сообщения об ошибке [**CPL \_**](cpl-stop.md) .

В ответ на это сообщение приложение панели управления должно освободить выделенную память и выполнить очистку на глобальном уровне.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                      |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                             |
| Заголовок<br/>                   | <dl> <dt>CPL. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**FreeLibrary**](/windows/win32/api/libloaderapi/nf-libloaderapi-freelibrary)
</dt> </dl>

 

 
